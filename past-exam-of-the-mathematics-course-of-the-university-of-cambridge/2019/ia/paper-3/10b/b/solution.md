<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unit sphere and the kernel $e^{-c|y-x|^2}$ are invariant under every [rotation in three dimensions](../../../../../../rotation-in-three-dimensions.md) fixing $y$. Therefore $T(y)$ has the same [axisymmetry](../../../../../../axisymmetric-vector-field.md), so part (a) gives

$$
T_{ij}=\alpha\delta_{ij}+\beta y_iy_j.
$$

Choose [spherical polar coordinates](../../../../../../spherical-coordinate-system.md) with polar axis $y$ and put $u=\cos\theta=x\mathbin\cdot y$. Since $|x|=|y|=1$,

$$
|y-x|^2=2(1-u),
\qquad dA=2\pi\,du.
$$

The [tensor contraction](../../../../../../tensor-contraction.md) giving the trace is

$$
T_{kk}=\int_S|x|^2e^{-c|y-x|^2}\,dA
=2\pi\int_{-1}^1e^{-2c(1-u)}du
=\boxed{\frac{\pi}{c}(1-e^{-4c})}.
$$

Similarly,

$$
T_{ij}y_iy_j
=2\pi\int_{-1}^1u^2e^{-2c(1-u)}du
=\boxed{\frac{\pi e^{-2c}}{c^3}
\left[(2c^2+1)\sinh(2c)-2c\cosh(2c)\right]}.
$$

At $c=0$ these expressions have the continuous limiting values $4\pi$ and $4\pi/3$. Writing them as $A=T_{kk}=3\alpha+\beta$ and $B=T_{ij}y_iy_j=\alpha+\beta$ gives

$$
\boxed{\alpha=\frac{A-B}{2},\qquad \beta=\frac{3B-A}{2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
