1. What problem does the context API help solve?

    The Context API is a component structure provided by the React framework, which enables us to share specific forms of data across all levels of the application. It's aimed at solving the problem of prop drilling.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? 

    Actions: Actions in Redux are packets of information that contain an action type and associated data. Importantly in Redux, reducers are the only place we can update our state. Actions tell our reducers “how” to update the state, and perhaps with what data it should be updated, but only a reducer can actually update the state. 


    Reducers: Reducers calculate the new version of state based on the current state and a given Action. Reducers take in two arguments, the current state from the Redux store, and the action object, sent via action creator functions.


    Store: Everything that changes within your application is represented by a single JavaScript Object known as the store. The store contains our state for our application.

    Why is the store known as a 'single source of truth' in a redux application?

    The only way to change your data in UI is to dispatch redux action which will change state within redux reducer.

3. What is the difference between Application state and Component state? 
    Application State: An application state is simply the state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application.

    Component State: state is managed within the component

    When would be a good time to use one over the other? The more state needs to be shared between different components in your app, the more benefit there is to using the Redux store. 

4. Describe `redux-thunk`, what does it allow us to do? 

    Redux-Thunk: Redux Thunk middleware allows you to write action creators that return a function instead of an action.

    How does it change our `action-creators`?  The action-creator returned thunk has access to the dispatch function. So we can run an async function, like an API call, and inside the .then() we can dispatch an action.

5. What is your favorite state management system you've learned and this sprint? Please explain why!

    Redux - There is always one source of truth, the store, with no confusion about how to sync the current state with actions and other parts of the application.


