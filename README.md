# Inconsistent Width Calculation using calc() with Percentages and Ems

This repository demonstrates a subtle bug related to the CSS `calc()` function when combining percentages and `em` units. The issue arises from the context-dependent nature of the `em` unit, which can lead to inconsistent width calculations across different browsers or even within the same browser depending on the parent element's font size.

## The Problem
The provided `bug.css` file contains a CSS rule that attempts to set the width of an element to 50% of its parent's width, minus 2em. The inconsistency occurs when the parent element's font size changes, causing the calculated width to deviate from the expected value.

## The Solution
The `bugSolution.css` file offers a solution that addresses the issue by replacing the `em` unit with a fixed pixel value, providing a more consistent result across different contexts.  Using Viewport Units (vw) is another alternative if the width should scale with the viewport.