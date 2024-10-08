# **REACT**
![Alt Text](https://github.com/codeDeviator/React.js/blob/main/assets/intro.webp)


## Table of Content  
- Some terminologies you should know before starting documentation
- Introduction to React
- Advantages of React
- Getting Started with React
- Namaste React
- Core Concepts of React
- React Router
- State Management 
- Event Handling 
- Hooks 

## Some terminologies you should know before starting documentation
- HTML : Understanding the basic structure of HTML (e.g., tags, attributes) is important since JSX (React’s 
  templating language) is similar to HTML
- CSS Styling: Basic knowledge of CSS for styling components is useful. You should understand how to apply styles through 
  classes and inline styles
- Library : A library is a collection of pre-written code that you can use to perform specific tasks
- UI : User Interface means the things which user sees when he/she opens the Web app
- Rendering : Rendering in React refers to the process of generating the user interface (UI) that the user sees on the screen 
  based on the state and data of the application
- Single Web Page application : A Single Page Application is a type of web application that loads a single HTML page and 
  dynamically updates the content as the user interacts with the app, without requiring a full page reload.
- Jsx : JavaScript Xml is a syntax extension for javascript in react where we can write html code within javascript making 
  code look more clean and readable

## Introduction to React
A well-liked JavaScript package called React.js is used to create user interfaces, especially for single-page apps where the user interface (UI) refreshes dynamically without requiring a page reload. React is a framework created and maintained by Facebook that is simple, fast, and scalable. It enables developers to create sophisticated user interfaces (UIs) out of discrete, small pieces of code known as "components."  

![Alt Text](https://github.com/codeDeviator/React.js/blob/main/assets/facebook-1024x542.png)

## Advantages of React  

### Reusability  

Creating components or sections of code that may be reused repeatedly in other applications or projects is known as reusability in React. 

### Flexibility

Flexibility in React means the code is easier to work with and update because it's built in small, separate pieces called components. This makes React code easier to understand and maintain compared to other frontend frameworks.

### Single Web Page Application

React offers a quick and responsive user experience, therefore creating a single-page application might be seen as a benefit. 
  
### Easy to Learn

It's considerably simpler to understand and use ReactJS. There is no shortage of training materials, tutorials, or documentation included with it. In a few days, any developer with a background in JavaScript can quickly grasp React and begin building online applications.

### Unidirectional Data Flow

Predictable Data Management: React enforces a unidirectional data flow, meaning that data flows in a single direction from parent components to child components through props. This predictable flow makes it easier to manage state and debug applications
Simplified Debugging: Since data flows in one direction, tracking down issues and understanding how state changes affect the application becomes simpler

### Component-Based Architecture  

Reusability: React allows you to build UI components that can be reused across your application, reducing duplication and speeding up development
Maintainability: Components are self-contained, making the code more modular and easier to maintain or update independently


## Getting Started with React  

With the help of contemporary tools, creating user interfaces with the popular JavaScript package React.js is simple. This is a detailed how-to for configuring your React development environment.  

A React application can be created using one of two methods: the first is the conventional method, which we used to create the app by selecting "Create React App," which installs a lot of extra files and dependencies. The other method was recently implemented and is called "React Vite," which is renowned for its lightning-fast development and only installs the necessary number of files or dependencies. Here, we'll learn how to use Create React App (CRA) to create a React application.  

![Alt Text](https://github.com/codeDeviator/React.js/blob/main/assets/reactvite.png)
## Installation

To start using React, you need to set up your development environment. The easiest way to get started is by using Create React App, a tool that sets up a new React project with a good default configuration.

### Prerequisites

Before you begin, make sure you have the following installed on your machine:
- **Node.js** (https://nodejs.org/) - React requires Node.js for building and running your application.
- **npm** (Node Package Manager) - This comes bundled with Node.js and helps manage dependencies.

### Steps

1. **Install Node.js and npm**:
   - Download and install Node.js in linux with help of this command
    ```jsx
     sudo apt install nodejs npm
     ```
   - After downloading Verify the installation by running the following commands in your terminal:
     ```bash
     node -v
     npm -v
     ```

2. **Install Create React App**:
   - Open your terminal and run the following command to install Create React App globally:
     ```bash
     npx create-react-app my-app (You can use any name for your directory instead of my-app just replace my-app with that name)
     ```
     This command creates a new directory called `my-app` with a default React project setup.

3. **Navigate to Your Project Directory**:
   - Change to the newly created directory:
     ```bash
     cd my-app  (Here we use cd to enter the directory . To go out of directory use cd..)
     ```

4. **Start the Development Server**:
   - Run the following command to start the development server:
     ```bash
     npm start
     ```
     Your new React application will open in your default web browser at `http://localhost:3000` (port number can change if port 3000 is busy with some other content)  
     You will see a react logo in browser . Below is the Screen Shot for the webpage which you will see 
![Alt Text](https://github.com/codeDeviator/React.js/blob/main/assets/welcome-to-react.png)

5. **Folder Structure of a simple React Project**
   
![Alt Text](https://github.com/codeDeviator/React.js/blob/main/assets/images.png)  
   
Conclusion
Setting up a React project is straightforward, and Create React App helps you hit the ground running with a default configuration. From here, you can start building your components, managing state, and adding functionality to your app. React's vast ecosystem allows for easy integration with various tools, making it a versatile choice for web development.
## Namaste React

Let's create a simple "Namaste React" component to get a feel for how React works.

### Steps to Write Namaste React 

1. **Open Your Project in a Code Editor**:
   - Use a code editor like Visual Studio Code (VS Code) to open the `my-app` directory.

2. **Edit `src/App.js`**:
   - Replace the content of the `src/App.js` file with the following code:
     ```jsx
     import React from 'react';

     function App() {
       return (
         <div>
           <h1>Namaste, React!</h1>
         </div>
       );
     }

     export default App;
     ```

3. **Run Your Application**:
   - If the development server is not already running, start it by running `npm start` in your terminal.
   - Open your web browser and navigate to `http://localhost:3000`. You should see "Namaste, React!" displayed on the page.

## Core Concepts of React

### JSX 

JavaScript XML, or JSX, is an HTML-like syntax extension for JavaScript. It is used to specify the UI's appearance when used with React. Instead of being a string or HTML, JSX is an XML-like syntax that is converted to standard JavaScript by Babel and other tools before being shown in a browser. In essence, it transforms HTML into React components.   

**Example 1**  
```jsx
function Greeting() {
  const name = "Ayush";
  return (
    <div>
      <h1>Hello, {name}!</h1>
      <p>Welcome to learning React with JSX.</p>
    </div>
  );
}
```

**Example 2**
Write "Hello" if x is less than 10, otherwise "Goodbye":
```jsx
// Import React
import React from 'react';

// Define the functional component
function App() {
  // Define the variables and logic
  const x = 5;
  let text = "Goodbye";
  if (x < 10) {
    text = "Hello";
  }

  // Create the element to be rendered
  const myElement = <h1>{text}</h1>;

  // Return the element to render it
  return (
    <div>
      {myElement}
    </div>
 
  );
}

// Export the component as default
export default App;

```

### Components  
The essential building elements of every React application are React components. They enable developers to divide complicated user interfaces (UIs) into smaller, easier-to-manage components by encapsulating portions of the UI and the logic that powers them. Componets are separate, reusable code segments    
There are 2 types of React componets -

- Functional Components
Functional components are JavaScript functions that return React elements. They are used to build parts of the user interface in a React application. They may or may not recieve data as paramaeters 

**Note**  :- The functional component is also known as a stateless component because they do not hold or manage state.

Example -
```jsx
import React, { useState } from 'react';

// This is a functional component named Counter
function Counter() {
  // Declare a state variable named 'count' with an initial value of 0
  // useState is a hook that returns a stateful value and a function to update it
  const [count, setCount] = useState(0);

  // The return statement defines the component's UI
  return (
    <div>
      {/* Display the current count */}
      <p>You clicked {count} times</p>
      {/* When the button is clicked, update the count state */}
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}

export default Counter;
```

- Class based Components 
React Class Components are JavaScript classes that extend React.Component. They define the UI, manage state, and handle events within your application. Unlike functional components, which are based on function syntax, class components follow the traditional class-based approach.
After introduction of React Hooks use of class components has decreased because react hooks makes the code look clean and syntax is easy to understand
The render() method in react class components returns JSX elements describing the UI of the Application.

Example -
```jsx 
import React, { Component } from 'react';

// Define a class-based component by extending React.Component
class Counter extends Component {
  // Constructor method to initialize state
  constructor(props) {
    super(props); // Call the superclass constructor
    // Initialize the state with a count property
    this.state = {
      count: 0,
    };
  }

  // Method to handle incrementing the count
  increment = () => {
    // Update the state using setState
    this.setState((prevState) => ({
      count: prevState.count + 1,
    }));
  };

  // Method to handle decrementing the count
  decrement = () => {
    // Update the state using setState
    this.setState((prevState) => ({
      count: prevState.count - 1,
    }));
  };

  // The render method returns the JSX to be rendered
  render() {
    return (
      <div>
        {/* Display the current count */}
        <h1>Count: {this.state.count}</h1>
        {/* Button to increment the count */}
        <button onClick={this.increment}>Increment</button>
        {/* Button to decrement the count */}
        <button onClick={this.decrement}>Decrement</button>
      </div>
    );
  }
}

// Export the component to be used in other parts of the app
export default Counter;
```

### Props
Props is short for properties and are used to pass data from one component to another . Props are similiar to function arguments and are passed to components in same was as arguments are passed in a function .  
The child component can't modify the props it recieves and can only read and use the props  

Example using Props-
App.js File (Parent class where we will define Props)
```jsx 
import React from 'react';
import Greeting from './Greeting';


function App() {
  
  const userName = 'Mamania';  // This is the data we want to pass to the child component
  return (
    <div>
      <Greeting name={userName} />  {/* Where Props is userName */}
    </div>
  );
}

export default App;
```
Greeting.js file (Child component where we will pass the Props)
```jsx  
import React from 'react';

function Greeting(props) {
  // Access the name prop from the props object
  const { name } = props;

  // Use the name prop to display a greeting message
  return <h1>Hello, {name}!</h1>;
}

export default Greeting;
```
OutPut -
```jsx
Hello, Mamania!
```
## React Router 
React Router is a crucial tool for routing in React that facilitates navigating between components or between pages. React Router modifies the browser's URL and displays the page indicated by the supplied URL.  
React Router's primary benefit is its ability to assist in the creation of single-page apps with navigation and numerous views that don't require page refreshes.Because the browser doesn't have to request a brand-new document or reassess its CSS and JavaScript assets for each page, users can get speedier experiences. Additionally, it makes user experiences—like animation—more dynamic.  

### Note 
There were many changes made when react router was shifted from react-router v5 to v6 .  
For example:  
Simplified Route Definition  
V5: In React Router v5, routes were nested using Route components with explicit render or component props. Nesting could become complex and cumbersome.  
V6: React Router v6 uses a simpler and more declarative element prop, which replaces the component and render props. Additionally, routes are nested directly inside the Routes component, making the structure more intuitive.  
This documentation contains information for react router v6.  

### How to install React Router
Run the below command in your terminal 
```
npm i react-router-dom 
```

### Main Components of React Router are :-

- BrowserRouter: BrowserRouter is a router implementation that uses the HTML5 history API(pushState, replaceState, and the popstate event) to keep your UI in sync with the URL. It is the parent component that is used to store all of the other components.
- Routes: It’s a new component introduced in the v6 and an upgrade of the component. The main advantages of Routes over Switch Routes are chosen based on the best match instead of being traversed in order.
- Route: Route is the conditionally shown component that renders some UI when its path matches the current URL.
- Link: The link component is used to create links to different routes and implement navigation around the application. It works like an HTML anchor tag.

Example of React Router in React JS

```jsx
import React, { Component } from "react";
import {
    BrowserRouter as Router,
    Routes,
    Route,
    Link,
} from "react-router-dom";
import Home from "./component/home";
import About from "./component/about";
import Contact from "./component/contact";
import "./App.css";

class App extends Component {
    render() {
        return (
            <Router>
                <div className="App">
                    <ul className="App-header">
                        <li>
                            <Link to="/">Home</Link>
                        </li>
                        <li>
                            <Link to="/about">
                                About Us
                            </Link>
                        </li>
                        <li>
                            <Link to="/contact">
                                Contact Us
                            </Link>
                        </li>
                    </ul>
                    <Routes>
                        <Route
                            path="/"
                            element={<Home />}
                        ></Route>
                        <Route
                            path="/about"
                            element={<About />}
                        ></Route>
                        <Route
                            path="/contact"
                            element={<Contact />}
                        ></Route>
                    </Routes>
                </div>
            </Router>
        );
    }
}

export default App;
```
```jsx
import React from "react";
import {
    BrowserRouter as Router,
    Routes,
    Route,
    NavLink,
} from "react-router-dom";
import Home from "./components/Home";
import About from "./components/About";
import Contact from "./components/Contact";
import "./App.css";

const App = () => {
    return (
        <Router>
            <div className="App">
                <nav className="App-header">
                    <ul>
                        <li>
                            <NavLink 
                                to="/" 
                                className={({ isActive }) => isActive ? "active-link" : ""}
                                end>
                                Home
                            </NavLink>
                        </li>
                        <li>
                            <NavLink 
                                to="/about"
                                className={({ isActive }) => isActive ? "active-link" : ""}
                            >
                                About Us
                            </NavLink>
                        </li>
                        <li>
                            <NavLink 
                                to="/contact"
                                className={({ isActive }) => isActive ? "active-link" : ""}
                            >
                                Contact Us
                            </NavLink>
                        </li>
                    </ul>
                </nav>
                <Routes>
                    <Route path="/" element={<Home />} />
                    <Route path="/about" element={<About />} />
                    <Route path="/contact" element={<Contact />} />
                </Routes>
            </div>
        </Router>
    );
};

export default App;
```

The above code shows different route which takes us to different elements. When going from one page to another the whole page does not get loaded again and only the components which are required are loaded which makes the webpage more efficient.

## State Management   

### State
State in React is like an object that stores information about the current state or state of your component. In easy words we can say how it is actually looking like in a given point of time . This information may change over time, and React will update the feature to reflect the latest information.  

- State as a Data Store: Each React component can have its own state, which stores dynamic information that the component can use and display.  

- Accessing State: In class components, you access the state using "this.state".  

- Changing State: When the state changes, React automatically re-renders the component to show the new state.   

### State Management 
Changing State is a part of State Managmenet which allows state to maintain and update state accordingly . For example in a task management app when we add a task , a task is added and is considered as a change of state or state management . 
State management helps in making the webpage look dynamic .
We can change the component state by using the setState() method and passing a new state object as the argument
In React, state management can be managed within components using 'useState' hook for functional component or 'this.state' for class component .  

- Example of Functional Component with State Management   
```jsx
import React, { useState } from 'react';

function Counter() {     //we made a functional called counter
    const [count, setCount] = useState(0);   // count is initial state and setCount is state after changing state and initital state is 0  

    return (
        <div>
            <p>{count}</p>
            <button onClick={() => setCount(count + 1)}>Increment</button> 
        </div>
    );
}
```
In this above code whenever the button will be clicked it's count will increase by 1 number. 

- Class Component with this.state
```jsx
import React, { Component } from 'react';

// Define a class component named Counter
class Counter extends Component {
    // Constructor method to initialize state
    constructor(props) {
        super(props); // Call the parent class's constructor
        this.state = { count: 0 }; // Initialize state with a count property set to 0
    }

    // Arrow function to handle incrementing the count
    increment = () => {
        // Update the state with the new count value
        this.setState({ count: this.state.count + 1 });
    }

    // Render method to define what the UI looks like
    render() {
        return (
            <div>
                {/* Display the current count */}
                <p>{this.state.count}</p>
                {/* Button to trigger the increment method on click */}
                <button onClick={this.increment}>Increment</button>
            </div>
        );
    }
}

export default Counter;
```
The above code will also do same thing . When the button will be clicked it will increase the value by 1 number . Initial State is 0

**Note**
- useState is used in class component 
- this.state is used in functional component

## Event Handling 

### Event   
An event is an action that could be triggered as a result of user action or system generated event . For example a mouse click event which is written as `onClick event`  
It captures and responds to user actions within application.

React uses different ways to handle event 
Some of The most common event handling techniques are 
 1) Mouse Events:
- onClick : Triggered when an element is clicked .
- onDoubleClick : Triggered when an action is doubleClicked . 
- onMouseEnter : Triggered when mouse pointer enters the element .
- onMouseLeave : Triggered when mouse pointer leaves the element .
2) Keyboard Events:
- onKeyDown : Triggered when a key is pressed down .
- onKeyPress : Triggered when a key is pressed and held down .
- onKeyUp : Triggered when a key is released .
3) Form Events :
- onChange : Triggered when the value of an element changes .
- onSubmit : Triggered when a form is submitted .
- onInput : Triggered when the value of an input element is changed .
```jsx
import React, { Component } from 'react';

// Define a React component named ClickButton
class ClickButton extends Component {

  // Define a method to handle the click event
  handleClick = () => {

    // Display an alert when the button is clicked
    alert('Button was clicked!');
  }

  // Render method to output the component's UI
  render() {
    return (
      // Button element with an onClick event handler
      <button onClick={this.handleClick}>
        Click Me
      </button>
    );
  }
}

// Export the component so it can be used in other parts of the application
export default ClickButton;
```
In the above code whenever a button is clicked it shows an alert stating that button was clicked .

### Difference between State Management and Event Handling 

| Aspect       |           State Management                    |          Event Handling                |
|--------------|-----------------------------------------------|----------------------------------------|
|Definition    | Managing state or data of a component         | Capturing and responing to user action |
|Purpose       | To maintain and update Data                   | Allow Components to interact with Ui   |
|Typical Usage | Keeping tracks of form inputs , Toggling UI   | Responding to button Clicks ,  form    |
|              | elements , storing fetched Data               | submissions , Mouse movements          |
|Key Methods   | 'useState', 'setState', 'useReducer'          | Different Event Handler Methods        |
|Trigger       | events , timers , network responses           | Clicks , key presses , Mouse events    | 


## Hooks 
Hooks is an important concept in react and were added in react version 16.8 . Hooks are special functions that let you use state and other react features in functional components and make it easier to manage state and other effects .   
After hooks use of Class components decreased because hooks allow us to use features of class components in functional components making the code look clean 

Commonly Used Hooks:    
- useState: The useState hook is used to add state management to functional components. State allows React components to keep track of changing data, and useState lets you declare state variables in your component.

Example:
```jsx
import React, { useState } from 'react';

function Counter() {
  // Declare a state variable 'count' initialized to 0, and a function 'setCount' to update it.
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>Click me</button>
    </div>
  );
}

export default Counter;
```  

How it works: useState takes an initial value (0 in this case) and returns an array with two elements: the current state value (count) and a function (setCount) to update it. Every time setCount is called, the component re-renders with the updated state.  

- useEffect: The useEffect hook allows you to perform side effects in your components, such as data fetching, setting up subscriptions, or manually updating the DOM. It is the replacement for lifecycle methods like componentDidMount, componentDidUpdate, and componentWillUnmount in class-based components.

Example:
```jsx
import React, { useState, useEffect } from 'react';

function Timer() {
  const [seconds, setSeconds] = useState(0);

  // Effect that runs after the component renders and updates every second
  useEffect(() => {
    const interval = setInterval(() => {
      setSeconds(prevSeconds => prevSeconds + 1);
    }, 1000);

    // Cleanup function to clear the interval when the component unmounts
    return () => clearInterval(interval);
  }, []); // Empty dependency array means this effect runs only once, like componentDidMount

  return <div>Seconds: {seconds}</div>;
}

export default Timer;
```  

How it works: useEffect takes two arguments: a callback function where the side effect code runs, and an optional dependency array that determines when the effect should run. If the dependency array is empty, the effect runs only after the initial render. If it contains variables, the effect will re-run whenever those variables change. You can also return a cleanup function to clean up resources like subscriptions or timers when the component unmounts.

- useContext: The useContext hook provides a way to share data (state, functions, etc.) across components without having to pass props manually through every level of the component tree. It helps avoid "prop drilling."

Example:
```jsx
import React, { useContext } from 'react';

// Create a Context for the app theme
const ThemeContext = React.createContext('light');

function ThemedButton() {
  // Use the context value in this component
  const theme = useContext(ThemeContext);

  return <button className={theme}>I am styled by the theme!</button>;
}

function App() {
  return (
    // Provide the context value to the tree
    <ThemeContext.Provider value="dark">
      <ThemedButton />
    </ThemeContext.Provider>
  );
}

export default App;
```  

How it works: First, you create a Context object with React.createContext(). The useContext hook allows any component to access the context value, as long as it's wrapped in a Context.Provider. In the example above, the ThemedButton component gets the value of "dark" from the context.

- useReducer: The useReducer hook is an alternative to useState for managing more complex state logic. It is similar to useState but provides a more structured way of handling state updates, especially when the state changes involve multiple actions.

Example:
```jsx
import React, { useReducer } from 'react';

// Define the initial state and reducer function
const initialState = { count: 0 };

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return { count: state.count + 1 };
    case 'decrement':
      return { count: state.count - 1 };
    default:
      return state;
  }
}

function Counter() {
  // useReducer takes a reducer function and an initial state
  const [state, dispatch] = useReducer(reducer, initialState);

  return (
    <div>
      <p>Count: {state.count}</p>
      <button onClick={() => dispatch({ type: 'increment' })}>+</button>
      <button onClick={() => dispatch({ type: 'decrement' })}>-</button>
    </div>
  );
}

export default Counter;
```  

How it works: useReducer takes a reducer function and an initial state as arguments. The reducer function defines how the state should change in response to specific actions. You then dispatch actions to trigger state changes. This is particularly useful for more complex state logic where you might have several state variables and actions.
   
- useRef: The useRef hook is used to create a reference to a DOM element or to persist a value across renders without causing a re-render. It provides a way to directly interact with DOM elements, similar to how document.querySelector works in vanilla JavaScript.  

Example:
```jsx
import React, { useRef } from 'react';

function FocusInput() {
  // Create a ref to store the input element
  const inputRef = useRef(null);

  // Function to focus the input field
  const focusInput = () => {
    inputRef.current.focus();
  };

  return (
    <div>
      <input ref={inputRef} type="text" />
      <button onClick={focusInput}>Focus the input</button>
    </div>
  );
}

export default FocusInput;
```  

How it works: useRef creates an object with a current property that holds the reference to the DOM element. The current value persists across renders without causing re-renders, and you can use it to directly manipulate the DOM element (like focusing an input in this example).
   - useNavigate: The useNavigate hook is part of React Router and is used for programmatic navigation within your application. It replaces the older useHistory hook from previous versions of React Router.

Example:
```jsx
import React from 'react';
import { useNavigate } from 'react-router-dom';

function HomePage() {
  const navigate = useNavigate();

  // Function to navigate to the about page
  const goToAboutPage = () => {
    navigate('/about');
  };

  return (
    <div>
      <h1>Welcome to the Home Page</h1>
      <button onClick={goToAboutPage}>Go to About Page</button>
    </div>
  );
}

export default HomePage;
```  

How it works: useNavigate returns a function that can be used to programmatically navigate to different routes in your application. When navigate('/about') is called, React Router will change the URL and render the component associated with the /about route.

Example of hook with help of useState
```jsx
import React, { useState } from 'react';

// Custom hook to manage true or false state also known as boolean stage
// This custom hook manages a boolean state (value). It initializes the state with the provided initialValue (either true or false). 
// It also provides a toggle function to switch the boolean value between true and false.
function useToggle(initialValue) {
  const [value, setValue] = useState(initialValue);

  // Function to toggle the boolean value
  const toggle = () => {
    setValue(!value);
  };

  // Return the boolean value and the toggle function
  return [value, toggle];
}


// Example component using the custom hook
function ToggleButton() {
  // Use the custom hook to get the boolean state and toggle function
  const [isOn, toggleIsOn] = useToggle(false);

  return (
    <div>
      <p>Toggle: {isOn ? 'ON' : 'OFF'}</p>
      <button onClick={toggleIsOn}>Toggle</button>
    </div>
  );
}

export default ToggleButton;
```
Output will be if you run the ToggleButton component provided, the output will be a toggle button displayed on the webpage. Initially, the text will show "Toggle: OFF" and there will be a button labeled "Toggle". When you click the "Toggle" button, the text will change between "Toggle: ON" and "Toggle: OFF" each time you click it, indicating the state of the toggle.

**Hook Rules** -
- Hooks can be only called inside React function components
- Hooks can only be called at top level of components
- Hooks cannot be conditional 

### Custom Hooks 
Custom hooks are user-defined functions in React that utilize one or more built-in React hooks to encapsulate and reuse stateful logic. Custom hooks follow the naming convention of starting with "use" to enable them to leverage React's hook system. They allow developers to extract common logic from components and share it across multiple components. Custom hooks are not built-in; developers create them according to their specific needs.

### Basic difference betweeen State and Hooks 
State is a way to store information in react component that can change over time when components are updated while hooks are special functions provided by React that enable us to use React features, like state, context, and more in function components . Before hooks, these features were only available in class components

## Reference Links 
- https://react.dev/learn
- https://legacy.reactjs.org/docs/getting-started.html
- https://www.youtube.com/watch?v=-mJFZp84TIY&list=PLu0W_9lII9agx66oZnT6IyhcMIbUMNMdt
- https://www.geeksforgeeks.org/react-tutorial/
