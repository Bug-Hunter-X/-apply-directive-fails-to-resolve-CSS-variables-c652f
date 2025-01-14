# Tailwind CSS @apply Directive Variable Resolution Bug

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to correctly resolve CSS variables when used within custom styles. 

## Bug Description
When using `@apply` with a style that references a CSS variable, the variable might not be resolved, leading to unexpected styles or rendering errors. This is particularly noticeable when the variable is defined in the `:root` or a similar scope. 

## Reproduction
1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Observe the unexpected styling (or lack thereof) in your browser.

## Solution
The solution involves defining the custom styles within the Tailwind configuration file (`tailwind.config.js`), or by explicitly defining the style with the resolved variable value.

See `bugSolution.css` for the corrected approach.