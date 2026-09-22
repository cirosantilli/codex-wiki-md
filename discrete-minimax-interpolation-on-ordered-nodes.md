# Discrete minimax interpolation on ordered nodes

↑ **Parent:** [Lagrange polynomial](lagrange-polynomial.md)

For $n+2$ increasingly ordered nodes $y_j$, let $r_j$ be their [Lagrange cardinal polynomials](lagrange-cardinal-polynomial.md), $t=\sum f(y_j)r_j$, and $r=\sum(-1)^jr_j$. The leading coefficient of $r_j$ has sign $(-1)^{n+2-j}$, so all summands in the leading coefficient of $r$ have the same nonzero sign. There is a unique $\lambda$ canceling degree $n+1$ in $t-\lambda r$. Its errors at the nodes are $\lambda(-1)^j$, and a better degree-at-most-$n$ approximation would have a difference polynomial with at least $n+1$ roots. Thus it minimizes the maximum node error. Increasing order matters: for the permutation $(0,1/3,1,2/3)$ the alternating interpolant is already the quadratic $-1+9x(1-x)$, so the leading-coefficient assertion for $n=2$ fails.

## ↑ Ancestors (7)

1. [Lagrange polynomial](lagrange-polynomial.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
