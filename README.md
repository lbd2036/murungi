<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TypeScript Front-End Example</title>
</head>
<body>
  <button id="myButton">Click me</button>
  <p id="output"></p>

  <script src="app.js"></script>
</body>
</html>
# murungi
// app.ts
document.addEventListener("DOMContentLoaded", () => {
  const button = document.getElementById("myButton");
  const output = document.getElementById("output");

  if (button && output) {
    let clickCount = 0;

    button.addEventListener("click", () => {
      clickCount++;
      output.textContent = `Button clicked ${clickCount} times`;
    });
  }
});
