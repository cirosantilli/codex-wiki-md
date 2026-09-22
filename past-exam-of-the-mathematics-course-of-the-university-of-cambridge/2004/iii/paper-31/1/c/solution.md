<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [continuity](../../../../../../continuous-function.md) of f makes its prescribed interval preimage B open, and $\hat x\in B$. On B we have $f(x)>f(\hat x)-\varepsilon$, so

$$
\mathbb E e^{nf(X_n)}\geq e^{n(f(\hat x)-\varepsilon)}\mathbb P(X_n\in B).
$$

The open-set lower bound of the [large deviation principle](../../../../../../large-deviation-principle.md) therefore yields

$$
\liminf_n n^{-1}\log\mathbb E e^{nf(X_n)}\geq f(\hat x)-\varepsilon-\inf_BI\geq f(\hat x)-I(\hat x)-\varepsilon.
$$

Thus the claimed **lower bound holds at every chosen point**. When $I(\hat x)=\infty$ its right side is minus infinity and the assertion is immediate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
