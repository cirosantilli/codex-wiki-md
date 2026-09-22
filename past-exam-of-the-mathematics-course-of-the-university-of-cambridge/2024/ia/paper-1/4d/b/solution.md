<h1 id="4d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the [Cauchy-Hadamard theorem](../../../../../../cauchy-hadamard-theorem.md), put

$$
L=\limsup_{n\to\infty}a_n^{1/n},
\qquad R=\frac1L.
$$

The squared coefficients have root limsup $L^2$, so their radius is $R^2$. Equal finite nonzero radii therefore require $R=R^2$, hence $R=1$. This can happen: for $a_n=n+1$, both $\sum a_nz^n$ and $\sum a_n^2z^n$ have radius one.

For the coefficients $a_n^{a_n}$, the relevant root terms are

$$
\left(a_n^{a_n}\right)^{1/n}
=\exp\left(\frac{a_n\log a_n}{n}\right).
$$

Equality can again occur. For example, take

$$
a_n=\log(n+2).
$$

Then $a_n\to\infty$, $a_n^{1/n}\to1$, and

$$
\frac{a_n\log a_n}{n}\to0.
$$

**Thus both $\sum a_nz^n$ and $\sum a_n^{a_n}z^n$ have radius one. These examples illustrate the [radius of convergence after powering coefficients](../../../../../../radius-of-convergence-after-powering-coefficients.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4D](../../4d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
