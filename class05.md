# Making mock and break it

* **The first thing we want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names.**

* **deciding if you should create a new function or object. One such technique is the `single responsibility principle`, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.**
* **UI and data models tend to adhere to the same information architecture. Separate your UI into components, where each component matches one piece of your data model.**

## Build A Static Version in React

**To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.**

## questionsto determine if something is state

* **Is it passed in from a parent via props? If so, it probably isn’t state.**
* **Does it remain unchanged over time?If so, it probably isn’t state.**

* **Can you compute it based on any other state or props in your component? If so, it isn’t state.**


_For each piece of state in your application:_

* **Identify every component that renders something based on that state.**
* **Find a common owner component (a single component above all the components that need the state in the hierarchy).**
* **Either the common owner or another component higher up in the hierarchy should own the state.**

* **If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.**
