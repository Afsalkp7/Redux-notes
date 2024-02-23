# REDUX Q and A ❓⁉

INTRODUCTION

- What is redux ? <br /> 
    Redux is a pattern or library to managing and updating states in an application using events called "actions" . It serve a centralized store for state , thats need to be used across the entire applicaion.
- What is global state ? <br />
    The state that need to be used across the entire application (many parts of application)
- Why use redux ? 
    The pattern and tools provoided by redux make it easier to under stand how , when , where the state in your application being updated , and how your application behave on those changes occur.
- When should use the redux ? <br />
    * Large amount of application states and that needed in many places in the app
    * App state updated freequently over time
    * Logic to upddate the state maybe complex
    * Apps are medium or large sized code base and might be worked on by meny people
<hr />

- React redux ? <br />
    React redux is a  official packages that let your react component interact with redux by reading pieces of codes and dispatching actions.
- Redux tool kit ? <br />
    Redux tool kit is a recommended approach for writing redux logics , It contain packages and functions that we think are essential for creaing a redux app . It is a best pracrices , simplify most redux tasks , prevent common mistakes , and make it easier to write redux app
- Redux DevTool extension ? <br />
    It show the history of changes to the state , and it used to simply and effectively debugg the applicaiton.

<hr />

- Action ? <br />
    An action is a plain javascript object that has a type field . <b>Action as an event</b> that describes something that happened in application.
- Payload ? <br />
    An action object can have other field with additional information about what happened. we put that information in a field called <mark>payload</mark>.
- Reducers ? <br />
    A reducer is a function that receive the current state and action object that decide how to update the state if necessary and return new state <mark>(state,action)=>newState</mark><br />
    It act like event listener which handles events based on the received action (event) type.
- Store ?<br />
    The current redux application state lives in a object thats called store.
- Dispatch ? <br />
    The only way to update the state by calling state.dispatch() function and pass in an action object.<br />
    It act like triggering an event.
- Selectors ? <br />
    Selectors is a function that know how to extract specific pieces of information from a store state value.
<hr />

- Data flow in redux application ? <br />
    * Store is create using root reducer function.
    * Store call reducer function at once , and return a value as initial state.
    * When the UI is first rendered , the component access the current state of redux store and use that data to decide what to render


    * Something happens in app like click or any other events
    * App code dispatch an actopn to the store
    * The app run the reducer function again with the previous state and current state and return value as the new state
    * The store notify to al parts of application about updation of store
    * Each UI component that needs data from the store checks to see if the parts of the state they need have changed 
    * If any changes occur , the component force to re render with new data , it update what you see on the screen.

    <img src="https://redux.js.org/assets/images/ReduxDataFlowDiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif" />
<hr/>
    
