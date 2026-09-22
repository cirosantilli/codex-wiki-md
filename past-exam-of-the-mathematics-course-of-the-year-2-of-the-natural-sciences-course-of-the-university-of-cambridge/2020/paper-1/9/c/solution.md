<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial [displacement](../../../../../displacement.md) lies in an [invariant subspace](../../../../../invariant-subspace.md) of axial motions. Let the three opposite vertex pairs have positions

$$
\pm(1+q_x)\mathbf e_x,\qquad \pm(1+q_y)\mathbf e_y,\qquad \pm(1+q_z)\mathbf e_z.
$$

For a vertex on the positive $x$ axis, the two [springs](../../../../../spring.md) towards the $y$ vertices contribute $-k(q_x+q_y)$ in the $x$ direction; the two towards the $z$ vertices contribute $-k(q_x+q_z)$. Transverse components cancel in pairs. Cyclically,

$$
m\frac{d^2}{dt^2}\begin{pmatrix}q_x\\q_y\\q_z\end{pmatrix}
=-k\begin{pmatrix}2&1&1\\1&2&1\\1&1&2\end{pmatrix}
\begin{pmatrix}q_x\\q_y\\q_z\end{pmatrix}.
$$

The [matrix](../../../../../matrix.md) is $I+\mathbf1\mathbf1^{\mathsf T}$. It has [eigenvalue](../../../../../eigenvalue.md) $4$ on the breathing [vector](../../../../../vector.md) $(1,1,1)$, and [eigenvalue](../../../../../eigenvalue.md) $1$ on the orthogonal plane $q_x+q_y+q_z=0$. This identifies the [axial normal modes of an octahedral spring framework](../../../../../axial-normal-modes-of-an-octahedral-spring-framework.md) without a large characteristic [determinant](../../../../../determinant.md).

Put $\omega_0=\sqrt{k/m}$ and decompose the initial [vector](../../../../../vector.md) as

$$
(\epsilon_1,\epsilon_2,\epsilon_2)
=A(1,1,1)+D(2,-1,-1),\qquad
A=\frac{\epsilon_1+2\epsilon_2}{3},\quad D=\frac{\epsilon_1-\epsilon_2}{3}.
$$

Since all initial [velocities](../../../../../velocity.md) are zero, only [cosine](../../../../../cosine.md) time factors occur. The complete motion to first order in the [displacements](../../../../../displacement.md) is

$$
\boxed{q_x(t)=A\cos(2\omega_0t)+2D\cos(\omega_0t),\qquad
q_y(t)=q_z(t)=A\cos(2\omega_0t)-D\cos(\omega_0t),}
$$

with the vertex positions given by the first displayed formula. No [translation](../../../../../translation-geometry.md) or [rotation](../../../../../rotation-mathematics.md) is excited: the initial [displacements](../../../../../displacement.md) are orthogonal to those [zero modes](../../../../../zero-mode.md) and their initial [velocities](../../../../../velocity.md) vanish. The two checks $\epsilon_1=\epsilon_2$ and $\epsilon_1+2\epsilon_2=0$ respectively isolate pure breathing and pure traceless axial [oscillation](../../../../../oscillation.md). Nonlinear corrections beyond the small-displacement approximation have been omitted.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
