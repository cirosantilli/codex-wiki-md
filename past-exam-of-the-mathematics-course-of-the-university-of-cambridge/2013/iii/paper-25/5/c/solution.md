<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $F_t=\exp(-i\theta X_t-\frac12\theta^2A_t)$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
dF_t=-i\theta F_t\,dX_t-\theta^2F_t\,dA_t.
$$

The explicit decreasing exponential contributes half the finite-variation term; the other half is the quadratic correction from $e^{-i\theta X_t}$. Now the [Itô product rule](../../../../../../ito-product-rule.md) and part (b) yield

$$
d(F_tM_t)=F_t\,dM_t-i\theta F_tM_t\,dX_t-\theta^2F_tM_t\,dA_t-i\theta F_t\,d\langle M,X\rangle_t=F_t\,dM_t-i\theta F_tM_t\,dX_t.
$$

The finite-variation terms cancel because $-i\theta(i\theta)=\theta^2$. This proves the product is a [local martingale](../../../../../../local-martingale.md). Moreover $|F_t|=e^{-\theta^2A_t/2}\le1$ and $|M_t|\le1$. The [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) therefore proves **the product is a true martingale**.

## ↑ Ancestors (11)

1. [C](../c.md)
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
