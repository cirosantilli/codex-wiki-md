<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [system of linear equations](../../../../../../../system-of-linear-equations.md) $T_\alpha x=b$ is solvable exactly when $b\in\operatorname{im}T_\alpha$. If $x_0$ is one solution, then

$$
T_\alpha x=b\iff T_\alpha(x-x_0)=0,
$$

so its solution set is $x_0+\ker T_\alpha$, a translate of the [kernel of a linear map](../../../../../../../kernel-of-a-linear-map-split.md).

For $\alpha\ne2$, the [matrix](../../../../../../../matrix.md) is an [invertible matrix](../../../../../../../invertible-matrix.md), and

$$
\boxed{\operatorname{im}T_\alpha=\mathbb R^3,\qquad\ker T_\alpha=\{0\}.}
$$

Every $b$ is in the [image of a linear map](../../../../../../../image-of-a-linear-map.md) and has exactly one preimage. For $\alpha=2$, its first two columns [span](../../../../../../../linear-span.md) the [image of a linear map](../../../../../../../image-of-a-linear-map.md), while the corresponding [homogeneous linear system](../../../../../../../homogeneous-linear-system.md) gives the [kernel of a linear map](../../../../../../../kernel-of-a-linear-map-split.md):

$$
\boxed{\operatorname{im}T_2=\{(u,v,w):u-v+w=0\},\qquad\ker T_2=\operatorname{span}\{(1,1,1)\}.}
$$

The prescribed $b=(-1,\beta,1)^T$ satisfies the displayed condition precisely when $\beta=0$. If $\beta\ne0$, it lies outside the [image of a linear map](../../../../../../../image-of-a-linear-map.md) and there is no solution. If $\beta=0$, it lies in the [image of a linear map](../../../../../../../image-of-a-linear-map.md), and the nonzero [kernel of a linear map](../../../../../../../kernel-of-a-linear-map-split.md) supplies infinitely many solutions.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
