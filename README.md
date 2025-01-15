# Unexpected Behavior in JavaScript Function Due to Loose Equality

This repository demonstrates a common JavaScript bug caused by using loose equality (`==`) instead of strict equality (`===`) when checking for null values.  The bug leads to unexpected behavior when other falsy values are passed as arguments.

## Bug Description
The `foo` function uses loose equality to check for null values in its arguments.  This means that other falsy values, such as 0, "", or `undefined`, will also cause the function to return 0, even if that's not the intended behavior.

## Solution
The solution involves using strict equality (`===`) to check for null values.  This ensures that only null values will cause the function to return 0. The improved function will correctly handle other falsy values.