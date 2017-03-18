*   data always flow from the store to the components

```javascript
import { connect } from 'react-redux';
import Notifications from './notifications.jsx';

const getVisibleNotifications = (notifications) => (notifications ? notifications.filter((n) => n.visible) : undefined);

const mapStateToProps = (state) => {
    return {
        notifications: getVisibleNotifications(state.notifications.notifications),
        echoEnabled: state.notifications.echoFeature
    }
};

const NotificationsContainer = connect(
    mapStateToProps,
    mapDispatchToProps
)(Notifications);

export default NotificationsContainer;
```
