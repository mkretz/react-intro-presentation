*   you can also use Typescript
*   JSX turns into TSX

```typescript
/// <reference path="../typing/react.d.ts" />

import * as React from 'react';

class DemoProps {
  public name:string;
  public age:number;
}

class Demo extends React.Component<DemoProps, any> {
  private foo:number;
  constructor(props:DemoProps) {
    super(props);
    this.foo = 42;
  }
  render() {
    return <div>Hello world!</div>
  }
}```
