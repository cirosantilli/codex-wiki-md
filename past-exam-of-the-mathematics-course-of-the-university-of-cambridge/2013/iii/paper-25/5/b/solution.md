<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A=\langle X\rangle$ be the [quadratic variation](../../../../../../quadratic-variation.md). We use bilinear [quadratic covariation](../../../../../../quadratic-covariation.md) for the complex martingale: $\langle M,X\rangle=\langle\operatorname{Re}M,X\rangle+i\langle\operatorname{Im}M,X\rangle$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(e^{-2i\theta X_t})=-2i\theta e^{-2i\theta X_t}\,dX_t-2\theta^2e^{-2i\theta X_t}\,dA_t.
$$

By the [Itô product rule](../../../../../../ito-product-rule.md), the finite-variation part of $d(e^{-2i\theta X}M)$ is

$$
e^{-2i\theta X_t}\left(-2\theta^2 M_t\,dA_t-2i\theta\,d\langle M,X\rangle_t\right).
$$

Part (a) says the product is a martingale, so uniqueness of the continuous semimartingale decomposition makes this finite-variation part zero. For $\theta\ne0$, division gives

$$
\boxed{d\langle M,X\rangle_t=i\theta M_t\,d\langle X\rangle_t.}
$$

For $\theta=0$, $M\equiv1$ and both sides are zero, so the identity holds without exception.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
