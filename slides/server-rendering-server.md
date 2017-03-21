*   in your Node backend

```javascript
import { renderToString } from 'react-dom/server'

function handleRender(req, res) {
  const store = createStore(...)
  const html = renderToString(
    <Provider store={store}>
      <App />
    </Provider>
  )
  const preloadedState = store.getState()
  res.send(renderFullPage(html, preloadedState))
}
```
