<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put

$$
a(x,y)=\frac{x^Ty}{\lVert x\rVert^2+\lVert y\rVert^2}.
$$

The numerator is the [linear kernel](../../../../../../linear-kernel.md), while the reciprocal of the denominator is the kernel from part c applied to $\lVert x\rVert^2$ and $\lVert y\rVert^2$. The [product of positive-semidefinite kernels](../../../../../../product-of-positive-semidefinite-kernels.md) therefore shows that $a$ is a positive-semidefinite kernel. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) give $|a(x,y)|\leq1/2$, so

$$
k_2(x,y)=\frac{a(x,y)}{1-a(x,y)}=\sum_{m=1}^\infty a(x,y)^m.
$$

Each power is positive semidefinite by the [Schur product theorem](../../../../../../schur-product-theorem.md), and the convergent sum is positive semidefinite.

Moreover $k_2(x,x)=1$. If $\Phi$ is its canonical [feature map](../../../../../../feature-map.md), then

$$
d(x,y)^2=2-2k_2(x,y)=\lVert\Phi(x)-\Phi(y)\rVert^2.
$$

The feature-space norm gives symmetry and the [triangle inequality](../../../../../../triangle-inequality.md). Finally, $d(x,y)=0$ implies $k_2(x,y)=1$, hence $a(x,y)=1/2$ and

$$
2x^Ty=\lVert x\rVert^2+\lVert y\rVert^2,
$$

which is equivalent to $\lVert x-y\rVert^2=0$. Thus $d$ is a [metric](../../../../../../metric.md) rather than merely a [pseudometric](../../../../../../pseudometric.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
