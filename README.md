# 🎨 Random Color Boxes

This is a simple HTML + JavaScript project that displays five boxes, each with a randomly generated background color. It uses basic DOM manipulation and CSS Flexbox for layout.

## 🚀 Features

- Generates random RGB colors.
- Applies a unique color to each box when the page loads.
- Uses modern JavaScript (ES6+).



## 🧠 How It Works

- `getRandomRgbColor()` generates a random RGB string using `Math.random()` and `Math.floor()`.
- JavaScript selects all elements with the `.box` class and assigns a random background color.
- CSS Flexbox is used to center the boxes and space them evenly.

## 📋 Code Example

### Random Color Function
```js```
function getRandomRgbColor() {
  const r = Math.floor(Math.random() * 256);
  const g = Math.floor(Math.random() * 256);
  const b = Math.floor(Math.random() * 256);
  return `rgb(${r}, ${g}, ${b})`;
} 
### Applying the Color to Boxes

let boxes = document.querySelectorAll(".box");
boxes.forEach((box) => {
  box.style.backgroundColor = getRandomRgbColor();
});

### 📦 How to Run

Clone or download the project.
Open index.html in your browser.
Refresh the page to see different colors.

### 🛠️ Technologies Used

HTML5
CSS3 (Flexbox)
JavaScript (Vanilla JS)
