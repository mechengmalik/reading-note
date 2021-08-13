# React: Component Lifecycle Events

![cycle](https://i2.wp.com/programmingwithmosh.com/wp-content/uploads/2018/10/Screen-Shot-2018-10-31-at-1.44.28-PM.png?resize=1024%2C567&ssl=1)

**Every component in React goes through a lifecycle of events. I like to think of them as going through a cycle of birth, growth, and death.**

* **Mounting :** Birth of your component.
* **Update :** Growth of your component.
* **Unmount :** Death of your component.

## Common React Lifecycle Methods

## render()

**The _render()_ method is the most used lifecycle method. You will see it in all React classes. This is because _render()_ is the only required method within a class component in React.**

As the name suggests it handles the rendering of your component to the UI. It happens during the **mounting** and **updating** of your component.

**A_render()_ method has to be pure with no side-effects.**

## componentDidMount()

**_componentDidMount()_is called as soon as the component is mounted and ready. This is a good place to initiate API calls, if you need to load data from a remote endpoint.**

**Unlike the _render()_ method, _componentDidMount()_ allows the use of _setState()._ Calling the _setState()_ here will update state and cause another rendering but it will happen before the browser updates the UI. This is to ensure that the user will not see any UI updates with the double rendering.**

## componentDidUpdate()

**This lifecycle method is invoked as soon as the updating happens. The most common use case for the _componentDidUpdate()_ method is updating the DOM in response to prop or state changes.**

**You can call _setState()_ in this lifecycle, but keep in mind that you will need to wrap it in a condition to check for state or prop changes from previous state. Incorrect usage of _setState()_ can lead to an infinite loop.**

____________________________________________________

## **Props vs State**

### **"props"** (short for "properties")

**_is an object of arbitrary inputs a React function component accepts as the first argument._**

_props as arguments to a function. React components are functions which return JSX (or more generally something that's renderable like React elements, null, a string, etc.). Typically when you have a piece of code that you would like to reuse, you can place that code into a function and any dynamic values that code used before can be accepted as arguments (for example const five = 2 + 3 could be extracted to a function and accept arguments like so const five = add(2, 3))._

### **"state"**

**_is data that changes over the lifetime of a specific instance of a React component._**

_State is data that changes over time, and this is precisely what React state is intended to be used for. It's intended to track data values over the lifetime of the component._
_owever, users of the AddWithInput component can no longer set the initial value of n2 anymore. With the way that component is implemented currently, it's not referencing props.n2 at all._