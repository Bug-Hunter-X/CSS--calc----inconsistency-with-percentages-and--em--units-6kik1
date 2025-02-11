# CSS `calc()` Inconsistency

This repository demonstrates an uncommon bug related to the CSS `calc()` function when combining percentages and `em` units. The issue arises when the parent element's width is not explicitly defined, leading to inconsistent results across different browsers.

## Problem

The provided CSS attempts to set the width of an element to 50% of its parent's width minus 2em.  If the parent's width isn't explicitly set, the calculation may fail, and the intended layout is not achieved.

## Solution

The solution involves explicitly setting the width of the parent container, or using a different approach that avoids the issues arising from incompatible units within `calc()`. Alternatively, units should be converted to be consistent before using `calc()`. 