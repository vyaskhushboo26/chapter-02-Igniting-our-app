## Summary of today's class:

1. Intro about the namaste react course 

2. Environment needed : Editor -  vs code, Browser - google chrome

3. Extensions for VS code :
better comments
bracket pair colorization toggler
es7+ react/redux/react-native snippet
gitlens
prettier-code
prettify JSON
vs-code icons

4. Created html boiler template in vs code using emmet and wrote html for printing some text.

5. Wrote a simple js program to print Namaste Everyone in h1 tag inside div container with id root and this is called the DOM maniupulation.

  const heading = document.createElement("h1");
  heading.innerHTML = "Namaste Everyone";
  const root = document.getElementById("root);
  root.appendChild(heading);

6. How does Browser know about document, createElement, appendChild etc ?
  -> used JS engine's browser API called document to create h1 element and appendChild to append it to root div.
  Js engine gives all the functionality, browser also know about window he has a JS engine. 


7. Sortest program of Js is a EMPTY file. 

8. Inject REACT in your code is a sortest program of react.
  
9. Wrote the same program using React 

  -> Add script for react CDN link in body of index.hmtl 
  -> create app.js and move our js script there
  -> Now, write the same script in react

  A `react element` is nothing but an object with properties which is created by React library.
  const heading = React.createElement("h1", {}, "Namaste Everyone");

  const root = ReactDOM.createRoot(document.getElementById("root"));
  root.render(heading);

  10. render() method takes an react element and modify our DOM.

  React will override whatever is inside your root and it will replace whatever you give inside render.
  so until the root is rendered, if we want to display some error message, it can be written in html (Not Rendered).

  what if we need to put more elements inside the root container - pass array of react elements to the container creation

  const heading1 = React.createElement("h1", {id : "title"}, "Namaste Everyone");
  const heading2 = React.createElement("h2", {id : "sub_title"}, "Welcome");

  const container = React.createElement("div", {}, [heading1, heading2]);
  const root = ReactDOM.createRoot(document.getElementById("root"));
  root.render(container);

7. Created a style.css file and linked to index.html 

8. Learn about arrow function for tomorrow's class