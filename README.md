Calculator Web App

A simple and stylish calculator built using HTML, CSS, and JavaScript.
Perfect as a beginner-friendly project for practicing DOM manipulation and UI layout.

Features

Basic arithmetic: add, subtract, multiply, divide

Live display updates

Clean dark UI with highlighted operator buttons

Responsive CSS Grid layout

Simple, readable JavaScript functions

Error handling for invalid expressions

Project Structure

calculator/
├── index.html         # Main calculator layout
├── calculator.css     # Styling & theme
└── calculator.js      # Calculator logic

Built With

HTML5 – Structure

CSS3 – Styling, Flexbox, Grid

JavaScript (ES6) – Logic & updates

How to Use

Clone the repository:

git clone https://github.com/yourusername/calculator.git


Open the project folder:

cd calculator


Open index.html in any web browser.

Code Overview
JavaScript Logic (calculator.js)
const display = document.getElementById("display");

function appendToDisplay(input) {
    display.value += input;
}

function clearDisplay() {
    display.value = "";
}

function calculate() {
    try {
        display.value = eval(display.value);
    } catch {
        display.value = "Error";
    }
}

CSS Grid Layout (calculator.css)
#keys {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    padding: 25px;
}

Notes

eval() is used for simplicity.
It’s fine for a personal project, but not recommended for production apps.

Buttons control all input; keyboard input is optional (but can be added!).

