<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Let the independent unit-step vectors be $V_j=(\cos\Theta_j,\sin\Theta_j)$. The [uniform distribution](../../../../../continuous-uniform-distribution.md) of each angle gives $\mathbb E[V_j]=0$, while $|V_j|^2=1$. With $S_n=\sum_{j=1}^nV_j$, expand the [squared Euclidean norm](../../../../../squared-euclidean-norm.md):

$$
\mathbb E|S_n|^2=\sum_{j=1}^n\mathbb E|V_j|^2+2\sum_{i<j}\mathbb E[V_i\cdot V_j].
$$

By [independence](../../../../../independent-random-variables.md), each cross term equals $\mathbb E[V_i]\cdot\mathbb E[V_j]=0$. Hence

$$
\boxed{\mathbb E|S_n|^2=n.}
$$

This [mean-square displacement of an isotropic planar random walk](../../../../../mean-square-displacement-of-an-isotropic-planar-random-walk.md) grows linearly even though the [expected value](../../../../../expected-value.md) of the displacement vector remains zero.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
