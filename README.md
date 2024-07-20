# REACT

      // To create components and render them, react and reactDOM must be imported.
      //Importing library creates an object React with methods to use the library. Comes from react package
      //Creating components and JSX expressions
      //Import ReactDOM to create an object with methods so react can interact with DOM
      // Name a functional component with Pascal case --> UpperCamelCase
      // Functional components return a react element in JSX
      // React app have 2 core files App.js and index.js
      // Define component in App.js and index.js is entry point.
      // Components in App.js must be exported to index.js to render
      // To export from App.js specify it as a default or named export 
      //  export default MyFunction;
      // To use import to index.js --> import MyFunction from './App';
      // document.getElementById('app') --> returns a DOM element from index.js
      // From DOM library .createRoot() creates a root for the DOM element
      // ReactDOM.createRoot(DOM element argument)
      // .createRoot() then returns a reference to this root to call methods on
      // From DOM library .render(component here) method called on the root --> root.render to display the React component.
      // React will display <Compenent /> in the root while appearing on screen.

      //index.js
      import React from 'react';
      import ReactDOM from 'react-dom/client';
      
      import MyComponent from './App';
      
      ReactDOM.createRoot(document.getElementById('app')).render(<MyComponent />);
      
      //App.js
      import React from 'react';
      
      function MyComponent() {
        return <h1>Hello world</h1>;
      }
      
      export default MyComponent;

      //From index.html
      <main id="app">
      </main>
