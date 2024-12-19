# Tailwind CSS @apply Directive Issue with Dynamic Variables

This repository demonstrates a bug where Tailwind's `@apply` directive doesn't work as expected when used with CSS variables or dynamic expressions within the class definition.

## Problem

The `@apply` directive is intended to allow for the composition of utility classes.  However, when used with classes that include variables or calculations, the variable's value isn't correctly resolved at runtime.  The expected behavior is that the variable should be resolved and applied during compilation or runtime, resulting in the correct CSS rules being applied.  Instead, the styles are not being applied correctly, leading to unexpected styling or no styling at all.

## Reproduction

1. Clone this repository.
2. Run your build/development process for your framework (e.g., Next.js, Vite, etc.).
3. Observe that the element intended to have styling using `@apply` appears with no styling or inconsistent styling.