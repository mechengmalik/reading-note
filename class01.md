# Component And Props

_Component-based architecture focuses on decomposing a design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each of which is associated with component sections._
_The primary objective of component-based architecture is to ensure **component reusability.**_

## What is a Component?

* **A component is  well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.**

* **A component is a software object, interact with other components, encapsulating certain functionality, conforms to a recommended behavior .**

## Characteristics of Components

![comp](https://i.stack.imgur.com/WRZip.png)

* **Reusability :** _it`s reused in different situations in different applications._

* **Replaceable :** _Components may be freely substituted with other similar components._

* **Not context specific :** _Components are designed to operate in different environments and contexts._

* **Extensible :** _A component can be extended from existing components to provide new behavior._

* **Encapsulated :**  _A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state._

* **Independent :** _Components are designed to have minimal dependencies on other components._

## Advantages

* **Ease of deployment :** _As new compatible versions become available, it is easier to replace existing versions with no impact on the other components._

* **Reduced cost :** _The use of third-party components allows the user to spread the cost of development and maintenance._

* **Ease of development :** _Components implement provide defined functionality, allowing impacting other parts of the system._

* **Reusable :** _they can be used to spread the development and maintenance cost across several applications or systems._

* **Modification of technical complexity :** _A component modifies the complexity through the use of a component container and its services._

* **Reliability :** _The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse._

* **System maintenance and evolution :** _Easy to change and update the implementation.

* **Independent :** Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development._

## What is Props?

_React is a component-based library which divides the UI into little reusable pieces. the components send data to each other and the way to pass data each other is by using props._

**Prop** _is a special keyword in React, which stands for_ **properties** _and is being used for passing data from one component to another._

### The Flow Of Data

_data with props are being passed in a uni-directional flow._ **(one way from parent to child)**
_props data is **read-only**, which means that data coming from the parent should not be changed by child components._

![flow](https://miro.medium.com/max/1838/1*bsS8ETUQqgBpAoT2D6tjmw.png)

### Using Props in React

**1- define an attribute and its value(data)**
**2- pass it to child component(s) by using Props**
**3- render the Props Data**

![prop](https://codedaily.io/tutorial_files/C4qKb6D-3b80c7b616.png?width=1712\&height=1048)
