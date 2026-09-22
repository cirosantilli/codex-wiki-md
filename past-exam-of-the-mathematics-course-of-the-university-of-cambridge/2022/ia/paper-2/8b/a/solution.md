<h1 id="8b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the vector field as

$$
\dot x=2x(4-x-y^2),\qquad \dot y=y(x-1).
$$

The [equilibrium points of a dynamical system](../../../../../../equilibrium-point-of-a-dynamical-system.md) in the closed first quadrant are

$$
\boxed{(0,0),\quad(4,0),\quad(1,\sqrt3)}.
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J(x,y)=
\begin{pmatrix}
8-4x-2y^2&-4xy\\
y&x-1
\end{pmatrix}.
$$

At $(0,0)$ its eigenvalues are $8,-1$, so this is a [saddle equilibrium](../../../../../../saddle-equilibrium.md). Its unstable direction is the positive $x$-axis and its stable direction is the positive $y$-axis; to first order, nearby trajectories satisfy $\dot x=8x$, $\dot y=-y$.

At $(4,0)$ the eigenvalues are $-8,3$, so it is also a saddle. The $x$-axis is the stable direction, while trajectories entering the quadrant in the $y$ direction move away.

At $(1,\sqrt3)$,

$$
J=\begin{pmatrix}-2&-4\sqrt3\\ \sqrt3&0\end{pmatrix},
$$

whose eigenvalues are

$$
-1\mathbin{\pm}i\sqrt{11}.
$$

It is therefore a [stable spiral](../../../../../../stable-spiral.md). A point immediately to its right moves upward, so nearby trajectories spiral counterclockwise into the equilibrium. These eigendirections and the inward spiral give the requested local phase-portrait sketches.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
