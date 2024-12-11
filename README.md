# CSS Specificity Issue with !important

This repository demonstrates a common issue in CSS where the `!important` flag can lead to unexpected behavior due to its overriding nature. The example showcases how using `!important` can unintentionally override more specific selectors and lead to unexpected rendering.

The `bug.css` file contains the erroneous CSS, while `bugSolution.css` offers a solution that avoids the unnecessary use of `!important`.

## Bug Description:

The problem lies in the usage of `!important` within the `.element2` class. The expectation is that `.element1.element2` would inherit a width of 500px from its specific selector.  However, the `!important` flag in `.element2` overrides this, resulting in the element retaining the width of 300px.