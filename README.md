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

### About Event Listeners in JavaScript

- **event:** text
- **event listener:**: text

```javascript
document.querySelector("#colorButton").addEventListener("click", () => {
    document.documentElement.style.setProperty('--text-color', 'blue');
});

```
