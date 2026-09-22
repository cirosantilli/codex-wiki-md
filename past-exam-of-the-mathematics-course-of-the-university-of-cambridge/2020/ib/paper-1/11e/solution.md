<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The curve is symmetric in both coordinate axes and under interchange of $x$ and $z$. Its shape, including its eight [inflection points](../../../../../inflection-point.md), is:

<a id="11e/image-a-plane-curve-and-its-inflection-points"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1-curve-and-inflections.png)

**[Figure 1](#11e/image-a-plane-curve-and-its-inflection-points). A plane curve and its inflection points**.

Writing $r^2=x^2+y^2$, the [surface of revolution](../../../../../surface-of-revolution.md) has equation

$$
\boxed{(x^2+y^2-1)^2+(z^2-1)^2=5}.
$$

Let

$$
F(x,y,z)=(x^2+y^2-1)^2+(z^2-1)^2-5.
$$

Its [gradient](../../../../../gradient.md) is

$$
\nabla F=4\bigl(x(r^2-1),y(r^2-1),z(z^2-1)\bigr).
$$

If this vanished, then $r^2\in\{0,1\}$ and $z^2\in\{0,1\}$, but at such a point $(r^2-1)^2+(z^2-1)^2\le2$, not five. Hence zero is a [regular value](../../../../../regular-value.md), and the [regular level set theorem](../../../../../regular-level-set-theorem.md) shows that $S=F^{-1}(0)$ is a smooth [embedded surface](../../../../../embedded-submanifold.md).

For a surface of revolution, the two [principal curvatures](../../../../../principal-curvature.md) are the curvature of the meridian and the normal curvature of a parallel. Along $r=1$,

$$
F_r=4r(r^2-1)=0,
$$

so the normal is vertical in the meridian plane and the parallel principal curvature vanishes. Therefore the [Gaussian curvature](../../../../../gaussian-curvature.md), the product of the principal curvatures, is zero there.

These are not the only zero-curvature points. The meridian itself has inflection points, at which its principal curvature vanishes. Setting $u=r^2$ and $v=z^2$, their positive squared coordinates satisfy

$$
(u-1)^2+(v-1)^2=5,
$$



$$
(3u-1)v(v-1)^2+(3v-1)u(u-1)^2=0.
$$

Besides interchanging $u$ and $v$, the solution is approximately

$$
(u,v)=(0.304199,3.125056).
$$

Each corresponding meridian inflection point sweeps out another circle on $S$, so $r=1$ does not exhaust the zero set of the Gaussian curvature.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
