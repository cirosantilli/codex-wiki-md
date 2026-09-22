<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The family $(Y_x)$ is a [Gaussian random field](../../../../../../gaussian-random-field.md). For distinct $x,x'$ its [covariance](../../../../../../covariance.md) is

$$
\operatorname{Cov}(Y_x,Y_{x'})
=\frac1{4d^2}\bigl|\{y:y\sim x\text{ and }y\sim x'\}\bigr|.
$$

Two distinct vertices of $\mathbb Z^d$ have a common neighbour exactly when their [graph distance](../../../../../../distance-graph-theory.md), equivalently their $\ell^1$ distance, is two. Since jointly [Gaussian variables](../../../../../../multivariate-normal-distribution.md) are independent exactly when they are uncorrelated,

$$
Y_x\text{ and }Y_{x'}\text{ are independent}
\quad\Longleftrightarrow\quad
x\ne x'\text{ and }\lVert x-x'\rVert_1\ne2.
$$

**Thus the field has finite-range dependence, even though nearest-neighbour values are independent.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
