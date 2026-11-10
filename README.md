# Numerical Analysis in C

A collection of numerical-method implementations and mathematical computing exercises developed for MATH 304. The project explores root finding, function sampling, and numeric representation using small, inspectable C programs.

## Methods and exercises

| Source | Topic |
| --- | --- |
| `bisectionMethod.c` | Bracketing a root and repeatedly halving the interval |
| `falsePosition.c` | Root approximation using a secant-based estimate within a bracket |
| `newtonMethod.c` | Iterative root approximation using Newton's method |
| `a.c` | Sampling and printing `sin(x)` values |
| `b.c` | Sampling and printing `x + sin(x)` values |
| `c.c` | Numerical calculations and floating-point output formats |

The `MATH 304/` directory also includes `sin.csv` and PDF materials accompanying the exercises.

## Compile and run

Use a C compiler and link the mathematics library. From the repository root:

```bash
gcc "MATH 304/bisectionMethod.c" -lm -o /tmp/bisection
/tmp/bisection

gcc "MATH 304/falsePosition.c" -lm -o /tmp/false-position
/tmp/false-position

gcc "MATH 304/newtonMethod.c" -lm -o /tmp/newton
/tmp/newton
```

Each program contains its own function definition, initialization, and iteration logic. Inspect those values alongside the printed root to follow the numerical steps. The sampling programs print labeled, comma-separated values suitable for plotting or spreadsheet exploration.

## Technical focus

The collection contrasts interval-based and derivative-based root finding, represents convergence through explicit loops and stopping conditions, and connects numerical computation to tabular output. Each method remains independent, making the underlying mathematics easy to trace in the implementation.
