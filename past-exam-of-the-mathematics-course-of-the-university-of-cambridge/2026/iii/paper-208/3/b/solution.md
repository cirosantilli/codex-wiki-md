<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The lower-tail form of the [entropy method for certifiable functions](../../../../../../entropy-method-for-certifiable-functions.md) states that a unit-bounded-difference, $g$-certifiable nonnegative integer-valued function satisfies

$$
\log\mathbb E e^{-\lambda(Z-\mathbb EZ)}
\leq\frac{\lambda^2}{2}\mathbb E[g(Z)]
\qquad(\lambda\geq0).
$$

It follows by applying entropy tensorization to a minimal certificate: only its at most $g(Z)$ coordinates can contribute to the one-sided variance proxy, and changing any one contributes at most one.

The Chernoff bound therefore gives

$$
\mathbb P(Z-\mathbb EZ\leq-t)
\leq\inf_{\lambda>0}
\exp\!\left(-\lambda t+\frac{\lambda^2}{2}\mathbb E[g(Z)]\right).
$$

Choosing $\lambda=t/\mathbb E[g(Z)]$ proves

$$
\mathbb P(Z-\mathbb EZ\leq-t)
\leq\exp\!\left(-\frac{t^2}{2\mathbb E[g(Z)]}\right).
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
