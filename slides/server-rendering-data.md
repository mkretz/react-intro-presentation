*   pass application state to the client

```html
  <script>
      window.__APPLICATION_STATE__ = ${JSON.stringify(state)}
  </script>
```

*   initialize Redux with preloaded state

```
import React from 'react'
import { render } from 'react-dom'
import { createStore } from 'redux'
import { Provider } from 'react-redux'
import App from './containers/App'
import counterApp from './reducers'

const preloadedState = window.__APPLICATION_STATE__

const store = createStore(counterApp, preloadedState)

render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root')
)```
