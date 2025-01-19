# F# Mutable Variable Swap Bug

This repository demonstrates a common error in F# when attempting to swap mutable variables within a function.  The issue arises from how F# handles mutable variables passed as arguments.  The solution demonstrates how to correctly implement a swap function that modifies the original variables.

## Bug Description

The `swap` function attempts to swap the values of two mutable variables.  However, due to F#'s immutability features, the function does not modify the original variables outside its scope.

## Solution

The solution uses tuples to return the swapped values and correctly updates the original variables.