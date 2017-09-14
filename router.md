
```
import { BrowserRouter, Route } from 'react-router-dom';

export default class App extends Component {
  render() {
    return (
    <BrowserRouter>
      <div>
        <Header/>
        <Route exact path="/" component={Welcome} />
        <Route path="/signin" component={SignIn} />
        <Route path="/signout" component={Signout} />
        <Route path="/signup" component={Signup} />
        <Route path="/feature" component={RequireAuth(Feature)} />
      </div>
    </BrowserRouter>
    );
  }
}
```