# Halo 2 Circuit Design: a + b = c

This document describes a circuit designed to prove that `a + b = c` using Halo 2's circuit and constraint system.

## Circuit Description

The circuit uses three advice columns to represent the inputs:

- `a`: First input
- `b`: Second input
- `c`: Result

## Constraint

The circuit enforces the following constraint:

```
a + b = c
```

This constraint ensures that the sum of `a` and `b` equals `c`.

## Synthesize Method

In the `synthesize` method, we assign values to the columns `a`, `b`, and `c`. The proof system will then verify the constraint without revealing the actual values of these inputs.

## Privacy

This zero-knowledge proof allows us to prove that the equation `a + b = c` holds true for some values of `a`, `b`, and `c`, without disclosing the actual values of these variables.

## Use Case

This simple circuit can be used as a building block for more complex zero-knowledge proofs or as an educational example to understand the basics of Halo 2's constraint system.