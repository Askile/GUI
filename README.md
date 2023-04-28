# GUI
GUI for scripts

Example:
```javascript

function sayHello(){
  console.log("Hello World");
};

window.gui.createElements([
    {type: "folder", label: "Visuals"},
    {type: "slider", label: "Lighting", parent: "Visuals", object: settings, property: "lighting", start: 0, end: 1, step: 1},
    {type: "button", label: "Press", parent: "Visuals", description: "saying hello world", action: sayHello}
]);
```
