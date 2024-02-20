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
    An acntion is a plain javascript object that has a type field . <b>Action as an event</b> that describes something that happened in application.