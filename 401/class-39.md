# Redux Toolkit

> from Redux Toolikt Documentation page https://redux-toolkit.js.org/introduction/getting-started

## Installation

As a new app:

```
# Redux + Plain JS template
npx create-react-app my-app --template redux

# Redux + TypeScript template
npx create-react-app my-app --template redux-typescript
```

An existing app:

```
# NPM
npm install @reduxjs/toolkit
```

## Create a Redux Store

- Create a file named src/app/store.js

``` javascript
import { configureStore } from '@reduxjs/toolkit'

export const store = configureStore({
  reducer: {},
})

// Infer the `RootState` and `AppDispatch` types from the store itself
export type RootState = ReturnType<typeof store.getState>
// Inferred type: {posts: PostsState, comments: CommentsState, users: UsersState}
export type AppDispatch = typeof store.dispatch
```

## Provide store to index.js

 - put a React-Redux <Provider> around our application in `src/index.js.` 
 - import the Redux store we just created, put a `<Provider>` around your `<App>`, and pass the store as a prop:
``` javascript
import React from 'react'
import ReactDOM from 'react-dom'
import './index.css'
import App from './App'
import { store } from './app/store'
import { Provider } from 'react-redux'

ReactDOM.render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root')
)
```

## Create a Redux State Slice
