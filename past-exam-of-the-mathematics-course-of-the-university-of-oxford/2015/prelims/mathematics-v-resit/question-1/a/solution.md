<h1 id="question-1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here $\phi$ is a [scalar field](../../../../../../scalar-field.md): the source's description as a [vector field](../../../../../../vector-field.md) is a typographical slip, since the displayed formula is for its [gradient](../../../../../../gradient.md). For [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md), write $x=r\cos\theta$, $y=r\sin\theta$. Away from $r=0$, a local choice of $\theta$ gives the [partial derivatives](../../../../../../partial-derivative.md)

$$
r_x=\cos\theta,\quad r_y=\sin\theta,\quad
\theta_x=-\frac{\sin\theta}{r},\quad
\theta_y=\frac{\cos\theta}{r}.
$$

The [chain rule](../../../../../../chain-rule.md) therefore gives

$$
\phi_x=\Phi_r\cos\theta-\frac{\Phi_\theta}{r}\sin\theta,
\qquad
\phi_y=\Phi_r\sin\theta+\frac{\Phi_\theta}{r}\cos\theta,
\qquad \phi_z=\Phi_z.
$$

Use the [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md) definition $\nabla\phi=\phi_x\mathbf e_x+\phi_y\mathbf e_y+\phi_z\mathbf e_z$ and the [unit vectors](../../../../../../unit-vector.md)

$$
\mathbf e_r=\cos\theta\,\mathbf e_x+\sin\theta\,\mathbf e_y,
\qquad
\mathbf e_\theta=-\sin\theta\,\mathbf e_x+\cos\theta\,\mathbf e_y.
$$

Collecting their coefficients proves

$$
\boxed{\nabla\phi=\Phi_r\mathbf e_r+\frac1r\Phi_\theta\mathbf e_\theta+\Phi_z\mathbf e_z,\qquad r>0.}
$$

This is the [gradient in cylindrical coordinates](../../../../../../gradient-in-cylindrical-coordinates.md). The factor $1/r$ converts a change in angle into a change per unit [arc length](../../../../../../arc-length.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Question 1](../../question-1.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
