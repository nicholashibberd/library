# Redux

Redux is JUST about managing applicaiton state. Nothing to do with rendering

3 principles

Single source of truth - State of whole application is stored within single store. This is just a data file though, no data manipulation takes part in here, like in Flux stores.

State is ready only - Only way to change is to submit an action. Views cannot write directly to state, they can only express an intent to transform the state. 

Changes are made with pure functions - These functions are called reducers. They take the previous state and return the new state, always returning new objects. 

Is it Flux?

Has reducers instead of stores.
Redux has no concept of dispatcher - it uses pure functions
Redux assumes you never mutate data

