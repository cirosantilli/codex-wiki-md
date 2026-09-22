<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Exactly one lowest-numbered ball is selected in each occupied bin, so

$$
\sum_{j=1}^m\alpha_j(x)
=n-f(x)\leq n,
\qquad
\sum_{j=1}^m\alpha_j(x)^2\leq n.
$$

Part c supplies the corresponding one-sided coordinate certificate. The product-space [entropy method for certifiable functions](../../../../../../entropy-method-for-certifiable-functions.md) states that a function with such a certificate of squared size at most $v$ has both centered tails bounded by $e^{-t^2/(2v)}$. Taking $v=n$ gives

$$
\boxed{\mathbb P(Z-\mathbb EZ\geq t)
\leq e^{-t^2/(2n)},
\qquad
\mathbb P(Z-\mathbb EZ\leq-t)
\leq e^{-t^2/(2n)}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
