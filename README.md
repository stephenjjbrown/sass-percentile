# Sass Percentile
A simple percentile function for sass, with interpolation. First parameter is the percentile, between 0 and 1. Second parameter is the list of values to derive from.

## Examples:

```scss
body {
    width: percentile(0.5, (0%, 150%, 200%));
    // 50th percentile
    // 150%
}

div {
    width: percentile(0.67, 0px 30px 1000px);
    // Interpolates the 67th percentile
    // 359.8px;
}
```