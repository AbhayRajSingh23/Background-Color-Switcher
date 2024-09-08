# Background Color Changer

This project is a simple web-based application that changes the background color of the webpage based on user interaction. The application utilizes JavaScript to add event listeners to buttons, allowing the user to dynamically change the background color by clicking on different color buttons.

## Features

- Four color options (grey, white, blue, and yellow) to change the background color.
- Responsive and dynamic color change with the click of a button.
- Simple and clean user interface.

## Technologies Used

- **HTML**: For creating the structure of the webpage.
- **CSS**: For styling the webpage elements.
- **JavaScript**: For adding interactivity to the webpage.

## How to Use

1. Clone or download the project files to your local machine.
2. Open the `index.html` file in any web browser.
3. Click on any of the buttons labeled "Grey," "White," "Blue," or "Yellow" to change the background color of the page.

## Code Explanation

The JavaScript code selects all buttons with the class `.button` and adds an event listener to each button. When a button is clicked, the background color of the page changes to the color corresponding to the button's `id`.

```javascript
const buttons = document.querySelectorAll(".button");
const body = document.querySelector("body");

buttons.forEach(function(button) {
    button.addEventListener('click', function(e) {
        if (e.target.id === 'grey') {
            body.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'white') {
            body.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'blue') {
            body.style.backgroundColor = e.target.id;
        }
        if (e.target.id === 'yellow') {
            body.style.backgroundColor = e.target.id;
        }
    });
});
