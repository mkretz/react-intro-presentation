##  Components
* stateless functional components

```javascript
const NotificationElement = ({notification, onDismiss}) => (
  <div>
    <ListItem
      primaryText={notification.text}
      leftIcon={<ActionGrade />}
      rightIconButton={<IconButton onClick={() => onDismiss(notification)} tooltip="dismiss"><ActionDelete /></IconButton>}/>
    <Divider />
  </div>
)```
