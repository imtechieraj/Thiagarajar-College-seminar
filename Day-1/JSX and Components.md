### JSX


When you write JSX, it gets compiled to regular JavaScript using a tool like Babel. The compiled code uses React's `createElement` function to create DOM elements.

For example, the above JSX code gets compiled to:

JavaScript

```
const element = React.createElement(
  "div",
  null,
  React.createElement("h1", null, "Hello, World!"),
  React.createElement("p", null, "This is a paragraph.")
);
```

**Key features of JSX:**

- **JavaScript expressions**: Use JavaScript expressions inside JSX using curly braces `{}`.


- **Components**: Create reusable components using JSX.


- **Event handling**: Handle events using JavaScript functions.


**Advantages of JSX:**


- **Easy to read and write**: JSX is easy to read and write, especially for developers familiar with HTML.


**Rules of JSX :**

- **JSX attributes**: Use camelCase for attribute names (e.g., `onClick` instead of `onclick`).


### Components 

  
Components are the building blocks of React applications. They are reusable pieces of code that represent a UI element or a part of the application's interface.