<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a real [continuous function](../../../../../../continuous-function.md) $f$, the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) asserts that a polynomial $p\in\mathcal P_n$ is a [best uniform approximation](../../../../../../best-uniform-approximation.md) exactly when either it is exact or its residual $r=f-p$ has $n+2$ ordered alternating extrema:

$$
\boxed{0\le x_0<\cdots<x_{n+1}\le1,\qquad
r(x_j)=s(-1)^j\|r\|_\infty,\quad s\in\{1,-1\}.}
$$

Here $\mathcal P_n$ means degree at most $n$, as required for a [linear subspace](../../../../../../vector-subspace.md).

For sufficiency, if a polynomial perturbation $v\in\mathcal P_n$ violated the [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md), then $r(x_j)v(x_j)>0$ at every displayed point. Thus $v(x_j)$ would alternate signs, forcing a distinct zero in each of the $n+1$ intervals $(x_j,x_{j+1})$ by the [intermediate value theorem](../../../../../../intermediate-value-theorem.md). A nonzero polynomial of degree at most $n$ cannot have that many zeros; the zero polynomial does not violate the criterion either.

For necessity, assume $M=\|r\|_\infty>0$ and no such alternating sequence exists. The two compact sets $E_+=\{r=M\}$ and $E_-=\{r=-M\}$ are disjoint and, when both are nonempty, have positive separation. Hence the extremal set has finitely many successive sign runs: infinitely many alternations would contradict that separation on the bounded interval. If there are $m$ changes of sign between those runs, then selecting one point from each run gives an alternating sequence of length $m+1$, so $m\le n$. Choose a point $z_j$ in the gap between each pair of consecutive opposite-sign runs, and set

$$
v(x)=C\prod_{j=1}^m(x-z_j).
$$

Choose the sign of $C$ so that $v$ agrees with $r$ on the first run. The roots lie outside the extremal set and each changes the sign, so $rv>0$ at every extremal point. Since $\deg v=m\le n$, this contradicts the [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md). Therefore a best polynomial must have the required alternation.

Existence also holds: a minimizing sequence has bounded [supremum norms](../../../../../../supremum-norm.md), hence bounded coefficients by evaluating at $n+1$ fixed distinct points and inverting the resulting [Vandermonde matrix](../../../../../../vandermonde-matrix.md). A convergent subsequence of coefficients yields a minimizer. Finally, if $p$ and $q$ are both best, their average is best; at its alternating extrema both individual residuals must equal the same extremal value. Consequently $p-q$ has at least $n+2$ zeros and is identically zero. **The best polynomial exists, is unique, and is characterized by alternation.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
