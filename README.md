# Tailwind CSS Gradient Rendering Bug

This repository demonstrates a bug where Tailwind CSS gradient utility classes fail to render correctly due to missing or improperly configured color palettes.  The issue arises when referencing a color palette that isn't defined in your `tailwind.config.js` file.

## Problem

The `bg-gradient-to-r from-blue-500 to-purple-500` class should create a smooth gradient from blue to purple. However, if the `purple` color palette is not included in the `tailwind.config.js` configuration, the gradient won't render correctly, potentially resulting in a solid color or an error.

## Solution

The solution involves ensuring that the required color palettes are defined within your `tailwind.config.js`.  Adding the `purple` color palette solves the rendering issue.  See `bugSolution.html` and the updated `tailwind.config.js` for a working example.
