<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B$ be Brownian motion and let $N(ds,dx)$ be an independent [Poisson random measure](../../../../../../poisson-random-measure.md) with intensity $ds\,K(dx)$. Writing $\widetilde N=N-ds\,K(dx)$ for its compensated version, the [Lévy–Itô decomposition](../../../../../../levy-ito-decomposition.md) constructs

$$
\boxed{
X_t=at+\sqrt b B_t
+\int_0^t\!\int_{|x|\leq1}x\,\widetilde N(ds,dx)
+\int_0^t\!\int_{|x|>1}x\,N(ds,dx).}
$$

The four terms are independent drift, Gaussian, compensated small-jump and compound-Poisson large-jump components.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
