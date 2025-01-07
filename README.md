# Uncommon CSS Bug: Missing Spaces in `calc()` Function

This repository demonstrates a subtle yet common error in CSS: forgetting to include spaces around the arithmetic operators (+, -, *, /) within the `calc()` function.  This seemingly small mistake can lead to unexpected layout problems and prevent styles from being applied correctly.

## The Bug

The `calc()` function in CSS allows for dynamic calculations of values. However, if spaces are omitted around the operators, the calculation fails. For instance:

```css
/* Incorrect */
#myElement { width:calc(100%-50px); }
```

This code will likely not produce the expected result. 

## The Solution

The correct syntax requires spaces around the operators:

```css
/* Correct */
#myElement { width: calc(100% - 50px); }
```

Ensure you always include spaces to avoid this common pitfall.