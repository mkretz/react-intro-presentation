* there are no HTML templates or directives

```javascript
class Words extends React.Component {
  render() {
  	return <div>{this.props.values.map((val) => val+' ')}</div>;
  }
}

ReactDOM.render(<Words values={['one', 'two', 'three']} />,
                  mountNode);```
