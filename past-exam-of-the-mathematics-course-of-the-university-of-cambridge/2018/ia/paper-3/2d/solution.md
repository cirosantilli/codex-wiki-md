<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Every $Q\in O(3)$ with $\det Q=1$ is a [rotation in three dimensions](../../../../../rotation-in-three-dimensions.md), hence is the product of two reflections in planes through its axis whose angle is half the rotation angle.

If $\det Q=-1$, its real eigenvalue is $-1$: the other two eigenvalues are either a complex-conjugate pair or two real signs, and their product is positive. Let $v$ be a corresponding unit eigenvector and let $H$ be reflection in $v^\perp$. Then $HQ$ fixes $v$ and has determinant $1$, so it is a rotation and hence a product of two reflections. Since $Q=H(HQ)$, **every member of $O(3)$ is a product of at most three reflections**.

Two reflections have determinant $1$, whereas one reflection has eigenvalues $(-1,1,1)$. The map $-I\in O(3)$ has determinant $-1$ but is not a reflection, so it cannot be a product of at most two reflections. Thus **three are sometimes necessary**.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
