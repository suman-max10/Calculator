# Tip Calculator

A simple and responsive tip calculator built with plain HTML, CSS, and JavaScript.

## Features

- Enter a bill amount and calculate tip instantly
- Adjust tip percentage using a range slider
- Split total bill among multiple people
- Displays:
  - Total tip amount
  - Total bill amount (bill + tip)
  - Tip per person
  - Total per person
- Clean UI with gradient styling and basic animations

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript (no frameworks)

## Project Structure

```text
.
|- index.html   # App markup
|- style.css    # App styling and animations
|- script.js    # Tip calculation logic and DOM updates
```

## How to Run Locally

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` in your browser.

No build tools or dependencies are required.

## Calculation Logic

The app calculates values using:

- `totalTip = bill * (tipPercent / 100)`
- `total = bill + totalTip`
- `tipPerPerson = totalTip / noOfPeople`
- `totalPerPerson = total / noOfPeople`

Values are displayed in the UI and updated whenever sliders or the bill input change.

## Notes

- The app currently uses slider minimums to avoid division by zero.
- Input values are formatted to two decimal places for currency display.

## Future Improvements

- Add input validation for empty/invalid bill values
- Format currency using `Intl.NumberFormat`
- Improve accessibility labels and keyboard interactions
- Add unit tests for calculation logic
