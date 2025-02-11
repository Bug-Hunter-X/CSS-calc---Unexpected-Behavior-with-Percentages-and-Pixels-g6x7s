# CSS calc() Unexpected Behavior

This repository demonstrates a bug related to the unexpected behavior of the `calc()` function in CSS when combining percentages and fixed units (like pixels).

## Bug Description

The `calc()` function in CSS is intended to allow dynamic calculations of CSS property values. However, when combining percentages and other units, such as pixels, the result might not always be as expected across different browsers or contexts. This inconsistency can lead to layout issues and unexpected rendering.

## Reproduction Steps

1. Open `bug.css` and observe the defined styles.
2. Apply the styles to an HTML element (demonstrated in the example HTML). 
3. Inspect the resulting element's width; it will likely deviate from the expected value due to the incorrect calculation of `calc(50% - 10px);`.

## Solution

To mitigate this issue, consider using alternative approaches or carefully adjusting calculations. Using viewport units (vw, vh) and avoiding mixed units in a single calculation is often recommended.

The `bugSolution.css` file demonstrates alternative methods to achieve similar layout results, providing better cross-browser compatibility and predictability.