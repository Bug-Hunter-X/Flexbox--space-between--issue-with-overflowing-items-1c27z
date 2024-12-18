# Flexbox space-between issue with overflowing items

This repository demonstrates an uncommon layout issue that can occur when using flexbox's `space-between` justification and the total width of flex items exceeds the container's width.  The issue is observed in some browsers and stems from the way `space-between` distributes space among items.

## Bug Report

The provided `bug.css` demonstrates the problem.  Notice that the blue boxes do not distribute evenly with space between them when the total width exceeds the container width, instead they either overflow or wrap in some browsers.

## Solution

The `bugSolution.css` demonstrates a solution. Instead of relying solely on `space-between`, it uses a combination of techniques to guarantee proper layout even when items overflow. This typically involves using `flex-wrap: wrap` and other adjustments to manage the item arrangement.