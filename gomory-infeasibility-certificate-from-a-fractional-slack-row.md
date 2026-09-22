# Gomory infeasibility certificate from a fractional slack row

↑ **Parent:** [Gomory fractional cut](gomory-fractional-cut.md)

For a nonnegative all-integer row $x_B+\sum_j a_jx_j=b$ with $a_j>0$, the [Gomory fractional cut](gomory-fractional-cut.md) requires $\sum_j\{a_j\}x_j\geq\{b\}$. The original row gives $\sum_j a_jx_j\leq b$. If a constant $\kappa$ satisfies $\{a_j\}\leq\kappa a_j$ for every $j$ and $\kappa b<\{b\}$, these inequalities contradict the cut. A single row therefore certifies integer infeasibility. Slacks may be used as integer variables when the original constraint coefficients and right sides are integral and the decision variables are integral.

## ↑ Ancestors (7)

1. [Gomory fractional cut](gomory-fractional-cut.md)
2. [Cutting-plane method](cutting-plane-method.md)
3. [Integer programming](integer-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
