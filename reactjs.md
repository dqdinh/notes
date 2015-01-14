React.js
===

## Getting started with React.js

### Setting State
- SPA: faster but more complex; render pieces of the webpage using components; use data immutablity to avoid complexity
- getInitalState: function returning object that sets inital state for component; this.state.stateName to access state attr;
- use single brackets to interpolate state into render function with JSX e.g., { this.state.stateName }
- In Console: set state with reactComponent.setState( stateName: attr ); get state with reactComponent.state() 
- everytime state changes react component re-renders (?); reconciliation; creates new virt dom tree + diffs + re-render

### passing state to subcomponents using props =
- if top components state changes it will push down to child components using props and re-render; 
- use setProps
- getDefaultProps: sets init props
- Top component sets props (owner) for child component(s)
- access owner props via this.props.propName
- React.PropTypes.string.isRequired : set prop type validation
- EX: array -> map(array) { return <component message={item} /> } ; more expressive than using templates with JS; run though array to render many subComponents.

### Handle Events
- uses synthetic events instead of real.

##





## Sources
- Getting started with Reactjs -- https://www.youtube.com/playlist?list=PLToJHFcYEZb3wgHC0ewvo5mIpZbY5PDIE
