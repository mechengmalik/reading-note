# Forms

_Forms are a crucial component of React web applications. They allow users to directly input and submit data in components ranging from a login screen to a checkout page. Since most React applications are single page applications (SPAs), or web applications that load a single page through which new data is displayed dynamically, you won’t submit the information directly from the form to a server. Instead, you’ll capture the form information on the client-side and send or display it using additional JavaScript code._

* React forms present a unique challenge because you can either allow the browser to handle most of the form elements and collect data through React change events, or you can use React to fully control the element by setting and updating the input value directly. The first approach is called an uncontrolled component because React is not setting the value. The second approach is called a controlled component because React is actively updating the input.

## Controlled Components

**In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState().`**

**We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a**`“controlled component”`**.

**Alternatives to Controlled Components**
_It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library. In these situations, you might want to check out uncontrolled components, an alternative technique for implementing input forms._

____________________________________________________

## The Conditional (Ternary) Operator

**allows us to specify that a certain block of code should be executed if a certain condition is met.**

* **The `condition` is what you’re actually testing. The result of your `condition` should be true or false or at least coerce to either boolean value.**

* **A `?` separates our `conditional` from our true value. Anything between the ? and the : is what is executed if the `condition` evaluates to true.**

* **Finally a `:`colon. If your `condition` evaluates to false, any code after the colon is executed.**

`