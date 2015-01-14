React.js
===

## Getting started with React.js

### Setting State
- SPA: faster but more complex; render pieces of the webpage using components; use data immutablity to avoid complexity
- getInitalState: function returning object that sets inital state for component; this.state.stateName to access state attr;
- use single brackets to interpolate state into render function with JSX e.g., { this.state.stateName }
- In Console: set state with reactComponent.setState( stateName: attr ); get state with reactComponent.state() 
- everytime state changes react component re-renders (?); reconciliation; creates new virt dom tree + diffs + re-render

### passing state to subcomponents using props
- if top components state changes it will push down to child components using props and re-render; 
- use setProps
- getDefaultProps: sets init props
- Top component sets props (owner) for child component(s)
- access owner props via this.props.propName
- React.PropTypes.string.isRequired : set prop type validation
- EX: array -> map(array) { return <component message={item} /> } ; more expressive than using templates with JS; run though array to render many subComponents.
- props are immutable

### Handle Events
- uses synthetic events instead of real. consistent across all browsers 
- addEventHandler.
- you can only log targets not the events itself b/c ?
- react maps all evetns at the top node and react handles their delegation
- react auto binds all events to the component?

### refs - messaging
- returns object for messaging between components
- EX: extract value from a text area component for use by a button to update another component's state?
- cases where you extract data from the DOM

### Data Flow
- one way directional flow of data
- components take in state and props
- send data through props to subcomponents
- subcomponents will send messages via handlers to top level components to change their state which will then run down the subcomponents?
- data binding with mixing using linkedStateMixin to manage state between two components connect to the same state




## Sources
- Getting started with Reactjs -- https://www.youtube.com/playlist?list=PLToJHFcYEZb3wgHC0ewvo5mIpZbY5PDIE
