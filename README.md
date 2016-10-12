

Checkout this repo, install dependencies:

```
	> git clone git@github.com:StephenGrider/ReduxSimpleStarter.git
	> cd ReduxSimpleStarter
	> npm install
	> npm start
```

Higher Order Component
Something that wraps a regular component to provide it with additional functionality.

In this repo, the higher order component  is the require_authentication.js
Its a function and will be called via the ComposedComponent
A class resides within the function. Inside the render fucntion the ComposedComponent is rendered and the props are passed through. 

We use the componentWillMount and componentWillUpdate to redirect the user based on the authenication.

// Inside the router
We wrap the component to be authenticated with the Higher Order Component
   <Route path="resources" component={requireAuth(Resources)} > </Route>



