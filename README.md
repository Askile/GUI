# GUI
GUI for scripts

Example:
```javascript

let settings = {
  lighting = 0,
  boolean = false;
};

function sayHello(){
  console.log("Hello World");
};

window.gui.createElements([
    {type: "folder", label: "Visuals"},
    {type: "folder", label: "Info"},
    {type: "folder", label: "Functions"},
    {type: "slider", label: "Lighting", parent: "Visuals", object: settings, property: "lighting", start: 0, end: 1, step: 1},
    {type: "display", label: "light level", parent: "Info", object: settings, property: "lighting"},
    {type: "button", label: "Press", parent: "Functions", description: "saying hello world", action: sayHello},
    {type: "switch", label: "Press", parent: "Functions", object: settings, property: "boolean"}
]);
```
