<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [conservative vector field](../../../conservative-vector-field.md) can be written as $F=\nabla\Phi$ for a single-valued [scalar potential](../../../scalar-potential.md) $\Phi$. Its [line integral](../../../line-integral.md) between two points depends only on the endpoints, and its integral around every closed curve is zero. A necessary local test for a smooth planar field $F=(P,Q)$ is $P_y=Q_x$. On a [simply connected](../../../simply-connected-space.md) domain such as the whole plane, this is also sufficient.

Here

$$
P_y=(3x^2+x^3y)e^{xy}=Q_x.
$$

An explicit [scalar potential](../../../scalar-potential.md) is even more decisive:

$$
\boxed{\Phi(x,y)=x^2e^{xy}+y^2,\qquad F=\nabla\Phi.}
$$

Indeed $\Phi_x=2xe^{xy}+x^2ye^{xy}$ and $\Phi_y=x^3e^{xy}+2y$. Thus the field is conservative on $\mathbb R^2$.

An [exact differential](../../../exact-differential.md) is a [differential one-form](../../../one-form.md) equal to $d\Phi$ on its domain; an [inexact differential](../../../inexact-differential.md) is not the differential of a single-valued potential there. For example, $d(xy)=y\,dx+x\,dy$ is exact. For the supplied form $\eta=42y\,dx+x\,dy$, the cross derivatives are

$$
\frac{\partial(42y)}{\partial y}=42,\qquad
\frac{\partial x}{\partial x}=1.
$$

They disagree, so $\eta$ is not even closed and hence cannot be exact. Equivalently, its counterclockwise [line integral](../../../line-integral.md) around the unit square is $1-42=-41\ne0$. Therefore

$$
\boxed{42y\,dx+x\,dy\text{ is inexact}.}
$$

The connection is $F\cdot d r=d\Phi$: a [vector field](../../../vector-field.md) is conservative precisely when its work [differential one-form](../../../one-form.md) is exact. Locally vanishing [curl](../../../curl.md) alone need not guarantee global exactness on a domain with holes.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
