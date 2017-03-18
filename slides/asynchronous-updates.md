*   asynchronous operations dispatch actions when they are started and when they return

```javascript
export function subscribeToUpdates() {
  return (dispatch, getState, socket) => {
    socket.on('connect', function() {
      dispatch(enableEcho());
      socket.on('msg', (msg) => {
        dispatch(createNotification(msg))
      });
    });
    socket.on('disconnect', function() {
      dispatch(disableEcho());
    });
  };
}
```
