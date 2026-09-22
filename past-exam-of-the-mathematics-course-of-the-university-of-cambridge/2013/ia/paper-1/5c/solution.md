<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Two nonzero vectors are [linearly independent](../../../../../linear-independence.md) when $s\mathbf x+t\mathbf y=0$ forces $s=t=0$. Their [linear span](../../../../../linear-span.md) then has dimension two. If they are [linearly dependent](../../../../../linear-dependence.md), one is a nonzero scalar multiple of the other, and their span has dimension one. Thus the two requested dimensions are $\boxed{2\text{ and }1}$.

The Euclidean [scalar product](../../../../../dot-product.md) and its [norm](../../../../../norm.md) are $\mathbf x\cdot\mathbf y=\sum_{j=1}^n x_jy_j$ and $\|\mathbf x\|=\sqrt{\mathbf x\cdot\mathbf x}$. To prove the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), first handle $\mathbf y=0$ trivially. Otherwise the squared [norm](../../../../../norm.md)

$$
0\leq\left\|\mathbf x-\frac{\mathbf x\cdot\mathbf y}{\|\mathbf y\|^2}\mathbf y\right\|^2
=\|\mathbf x\|^2-\frac{(\mathbf x\cdot\mathbf y)^2}{\|\mathbf y\|^2}
$$

gives

$$
\boxed{|\mathbf x\cdot\mathbf y|\leq\|\mathbf x\|\|\mathbf y\|.}
$$

Equality holds exactly when the residual vector is zero, meaning the vectors are [linearly dependent](../../../../../linear-dependence.md); this includes the zero-vector cases. Expanding $\|\mathbf x+\mathbf y\|^2$ and applying [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) then gives

$$
\|\mathbf x+\mathbf y\|^2\leq\|\mathbf x\|^2+2\|\mathbf x\|\|\mathbf y\|+\|\mathbf y\|^2,
\qquad\boxed{\|\mathbf x+\mathbf y\|\leq\|\mathbf x\|+\|\mathbf y\|}.
$$

Taking nonnegative square roots proves the [triangle inequality](../../../../../triangle-inequality.md).

For the unit-vector optimization, let $\mathbf w=\mathbf x+\mathbf y$. Independence ensures $\mathbf w\ne0$. The variable part of $S$ is $\mathbf z\cdot\mathbf w$, which [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) bounds below by $-\|\mathbf w\|$. Equality occurs only for the antiparallel unit vector. Thus

$$
\boxed{\mathbf z_*=-\frac{\mathbf x+\mathbf y}{\|\mathbf x+\mathbf y\|},\qquad
\lambda=-\frac1{\|\mathbf x+\mathbf y\|},\qquad
S_{\min}=\mathbf x\cdot\mathbf y-\sqrt{2+2\mathbf x\cdot\mathbf y}.}
$$

This is [minimizing a linear functional on a sphere](../../../../../minimizing-a-linear-functional-on-a-sphere.md). The two consequences follow below.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
