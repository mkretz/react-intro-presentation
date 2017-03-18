## Typing
*   out of the box: `propTypes`
*   checks at runtime, warnings in console
*   development mode only

```javascript
NotificationElement.propTypes = {
  notification: React.PropTypes.shape({
    text: React.PropTypes.string,
    visible: React.PropTypes.bool
  }).isRequired,
  onDismiss: React.PropTypes.func.isRequired
};```
