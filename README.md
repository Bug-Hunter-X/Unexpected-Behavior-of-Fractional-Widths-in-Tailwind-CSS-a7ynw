# Unexpected Behavior of Fractional Widths in Tailwind CSS

This repository demonstrates a common issue encountered when using fractional widths in Tailwind CSS.  Fractional widths like `w-1/2` only work correctly if the parent element has an explicit width. Otherwise, they behave unexpectedly.

## The Problem

The `bug.html` file shows a simple flex container with two divs, each having a `w-1/2` class.  Without a defined width on the parent, the fractional width doesn't work as intended. The divs will expand beyond their expected size.

## The Solution

The `solution.html` file demonstrates a solution. Add an explicit width to the parent container (`flex` div). This ensures that the fractional widths are calculated correctly within the defined space. Alternatively, using a flex-basis could also help solve this problem. 
