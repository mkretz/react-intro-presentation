*   in your Node backend

```javascript
import { renderToString } from 'react-dom/server'

const html = renderToString(
  <Provider store={store}>
    <App />
  </Provider>

res.send(html)
```
