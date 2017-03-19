## Server-side rendering

*   Motivation
    *   (search engine friendliness)
    *   fast initial load

*   in your Node backend, call

    ```javascript
    import { renderToString } from 'react-dom/server'

    const html = renderToString(
      <Provider store={store}>
        <App />
      </Provider>

    res.send(html)
    ```
