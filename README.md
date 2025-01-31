# Tailwind CSS: Subtle Errors and Debugging

This repository demonstrates two uncommon error scenarios in Tailwind CSS and their solutions.  The errors relate to the `@apply` directive and issues with unused CSS purging.

## Error 1: `@apply` with Undefined Classes

Using `@apply` with a class that hasn't been defined or isn't included in your `content` array in `tailwind.config.js` can lead to build errors or unexpected behavior (styles not appearing). 

## Error 2: Missing Styles After Purging (Non-JIT)

When using Tailwind without JIT mode, forgetting to properly configure the `content` array for purging can cause some of your classes to be unexpectedly removed, resulting in missing styles.

## Solutions

The solutions are provided in the `bugSolution.html` file.  Key steps include double-checking class definitions and ensuring your `content` array correctly points to your HTML files to prevent the purging of necessary styles.