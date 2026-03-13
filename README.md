# Intro to JavaScript
## Dynamic Text Styling

### Objective

You'll learn how to use CSS variables, the JS `querySelector()` method, event listeners and the `setProperty()` method to change the color of text in a web page on demand.

---

### Helpful Resources

- [Creating a CSS variable](https://www.w3schools.com/css/css3_variables.asp)
- [The `querySelector()` method in JavaScript]()
- [The `setProperty()` method in JavaScript]()


---

### Events & Event Listeners in JavaScript

- **event:** In JavaScript, an **event** is like a signal that something happened -- such as a click, a keypress, or the page loading.
  - You can write code to "listen" for these events and make something happen in response, like changing a color or showing a message on your web page!
- **event listener:**: An event listener is like a little helper that waits for something to happen -- such as when the user clicks a button or presses a key on their keyboard. When that thing happens, the event listener runs the code you wrote to make something cool happen, like swapping one image for another or changing the background color of your web page.




```javascript
document.querySelector("#colorButton").addEventListener("click", () => {
    document.documentElement.style.setProperty('--text-color', 'blue');
});

```
---

### Click-Related Events 

Here are three commonly used **click-related events** in JavaScript:

1. **`click`**
   - Triggered when a user clicks (presses and releases) a mouse button on an element.
   - Example: `element.addEventListener("click", () => { ... });`

2. **`dblclick`**
   - Triggered when a user double-clicks an element (two quick clicks in a row).
   - Example: `element.addEventListener("dblclick", () => { ... });`

3. **`mousedown`**
   - Triggered when a user presses (but doesn’t release) a mouse button on an element.
   - Example: `element.addEventListener("mousedown", () => { ... });`

---
