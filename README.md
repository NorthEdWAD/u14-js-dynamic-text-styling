# Intro to JavaScript
## Dynamic Text Styling

### Objective

You'll learn how to use CSS variables, the JS `querySelector()` method, event listeners and the `setProperty()` method to change the color of text in a web page on demand.

---

### Helpful Resources

- [Creating a CSS variable](https://www.w3schools.com/css/css3_variables.asp)
- [The `querySelector()` method](https://www.w3schools.com/jsref/met_document_queryselector.asp)

---





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

### The JS `setProperty()` Method

Here’s a simple example of using the `setProperty()` method in JavaScript:

```javascript
// Change the background color of the entire page to light blue
document.documentElement.style.setProperty('--bg-color', 'lightblue');
```

**How it works:**
- This line of JavaScript sets a CSS variable called `--bg-color` to the value `'lightblue'` on the `<html>` element (the root element of the web page).
- In your style sheet, you apply (use) a CSS variable you've already defined like this:
  ```css
  body {
    background-color: var(--bg-color);
  }
  ```
- When your JavaScript runs, the background color of the page will change to light blue!

---

### Adding Buttons

When finished, your page will contain six (6) buttons.

1. For today, though, just add three (3) buttons using the HTML `<button>` element.
2. Give each of the three buttons a unique identity using the HTML `id` attribute.

```html
<button id="button id goes here">Button Text Here</button>
```
- First button id: `colorButton`
  - Button text: Change Color
- Second button id: `sizeButton`
  - Button text: Change Size
- Third button id: `fontButton`
  - Button text: Change Font

**You'll add the other three buttons and button IDs later.**

---

### Events & Event Listeners 

- **event:** In JavaScript, an **event** is like a signal that something happened -- such as a click, a keypress, or the page loading.
  - You can write code to "listen" for these events and make something happen in response, like changing a color or showing a message on your web page!
- **event listener:**: An event listener is like a little helper that waits for something to happen -- such as when the user clicks a button or presses a key on their keyboard. When that thing happens, the event listener runs the code you wrote to make something cool happen, like swapping one image for another or changing the background color of your web page.

```javascript
// Linking an event listener to an HTML element with an `id` of `#colorButton`
document.querySelector("#colorButton").addEventListener();
```

```javascript
// Adding click event and an arrow function to your event listener
document.querySelector("#colorButton").addEventListener("click", () => {   });
```

```javascript
// Change text color
document.querySelector("#colorButton").addEventListener("click", () => {
    document.documentElement.style.setProperty('--text-color', 'blue');
}); // Pay attention to the punctuation and symbols used here!
```




