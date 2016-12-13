# react-sublime-tools
A collection of React snippets and other tools for Sublime Text.

Note: these have been tested on OSX / UNIX file system.
Some would probably not work on Windows but you can submit PR.

## Snippets

### es6 constructor

__Trigger__: constructores6

Will insert:

```
constructor (props) {
  super(props)
}
```

### export es6

__Trigger__: exportreact

Will insert:

```
export {default} from './MyComponent'
```

Use in an index.js file. (based on AirBnB code style)
In a code structure like this:

```
MyComponent
|- MyComponent.js
|- index.js
```

### React ES6 component

__Trigger__: reactes6

Will insert:

```
import React, {Component, PropTypes} from 'react'

export default class MyComponent extends Component {
  constructor (props) {
    super(props)
  }

  render () {
    return (
      <div></div>
    )
  }
}

MyComponent.propTypes = {

}

MyComponent.defaultProps = {

}
```

It will use the file name as component name.


### React stateless component

__Trigger__: reactstateless

Will insert:

```
import React, {PropTypes} from 'react'

export default function MultiSelect (props) {
  return (
    <div></div>
  )
}

MultiSelect.propTypes = {

}

MultiSelect.defaultProps = {

}
```

It will use the file name as component name.


## Completions

### Proptypes
Will add the React Proptypes to auto completions.

* .isRequired
* PropTypes
* PropTypes.any
* PropTypes.array
* PropTypes.arrayOf
* PropTypes.bool
* PropTypes.element
* PropTypes.func
* PropTypes.node
* PropTypes.number
* PropTypes.object
* PropTypes.objectOf
* PropTypes.oneOf
* PropTypes.oneOfType
* PropTypes.shape
* PropTypes.string
* PropTypes.symbol