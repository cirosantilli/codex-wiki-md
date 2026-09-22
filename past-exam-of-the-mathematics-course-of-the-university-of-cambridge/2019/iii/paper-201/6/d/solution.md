<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The joint process is a two-dimensional [Compound Poisson process](../../../../../../compound-poisson-process.md) whose [Lévy measure](../../../../../../levy-measure.md) is

$$
\nu(B)=\lambda\,\operatorname{Leb}
\{y\in[0,1]:(g_1(y),g_2(y))\in B\}.
$$

Two coordinates of a Lévy process are independent exactly when its Lévy measure charges only the coordinate axes and its Gaussian covariance has no cross term. Here there is no Gaussian part, so independence is equivalent to

$$
g_1(y)g_2(y)=0
\quad\text{for almost every }y.
$$

Since $g_1g_2$ is continuous, this is equivalent to pointwise vanishing. Conversely, when the product vanishes, the mark sets where $g_1$ and $g_2$ are nonzero are disjoint; independent thinning of the [Poisson random measure](../../../../../../poisson-random-measure.md) gives independent coordinate processes. Hence

$$
\boxed{(X_t^{g_1})_{t\geq0}\text{ and }(X_t^{g_2})_{t\geq0}
\text{ are independent}
\iff g_1(y)g_2(y)=0\ \text{for every }y\in[0,1].}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
