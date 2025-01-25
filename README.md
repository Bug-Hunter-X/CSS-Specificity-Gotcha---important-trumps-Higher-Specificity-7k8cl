# CSS Specificity and !important

This repository demonstrates a subtle CSS specificity issue involving the `!important` flag and inheritance.  The example showcases a scenario where a more specific selector fails to override a declaration with `!important`.

## Bug Description

A parent element sets a color, a child overrides it with `!important`, and a more specific selector attempts to override the child's style.  Despite the higher specificity of the targeted selector, the `!important` declaration remains dominant.

## Solution

The solution involves understanding the precedence of `!important` and avoiding its overuse.  Refactoring the CSS to eliminate unnecessary `!important` flags and carefully managing specificity is recommended.