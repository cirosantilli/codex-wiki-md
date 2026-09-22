<h1 id="12f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Extend the [sequence](../../../../../../sequence.md) by $c_0=1$. Cancelling factorials in consecutive [normalized central binomial coefficients](../../../../../../normalized-central-binomial-coefficients.md) gives

$$
\frac{c_n}{c_{n-1}}=\frac{(2n)(2n-1)}{4n^2}
=1-\frac1{2n},\qquad
c_n=\prod_{j=1}^n\left(1-\frac1{2j}\right).
$$

The given logarithmic inequality therefore implies

$$
\log c_n\leq-\frac12\sum_{j=1}^n\frac1j.
$$

On $[j,j+1]$, $1/t\leq1/j$, so summing its integrals gives $\sum_{j=1}^n1/j\geq\log(n+1)$. Exponentiating yields the explicit bound

$$
\boxed{0<c_n\leq(n+1)^{-1/2}\longrightarrow0.}
$$

Also every consecutive ratio is less than one, so $(c_n)$ is strictly decreasing, a fact needed for the alternating endpoint.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
