<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose positive $x$ downhill and positive $\theta$ in the corresponding rolling direction, with $x=\theta=0$ initially. For [rolling without slipping](../../../../../../rolling-without-slipping.md), the contact point has zero [velocity](../../../../../../velocity.md), so $\dot x-b\dot\theta=0$. Integrating the [rolling constraint](../../../../../../rolling-constraint.md) gives

$$
\boxed{x=b\theta,\qquad \ddot x=b\ddot\theta.}
$$

Let $F$ be the uphill [static friction](../../../../../../static-friction.md). Along the inclined [plane](../../../../../../plane.md), [Newton's second law](../../../../../../newton-s-second-law.md) for the [centre of mass](../../../../../../center-of-mass.md) gives

$$
M\ddot x=Mg\sin\varphi-F.
$$

The weight passes through the [centre of mass](../../../../../../center-of-mass.md), and the [normal reaction](../../../../../../normal-force.md) has its line of action through it. Thus only [static friction](../../../../../../static-friction.md) supplies [torque](../../../../../../torque.md) about $G$. The [angular velocity](../../../../../../angular-velocity.md) is along the cylinder's symmetry axis, so the [inertia tensor](../../../../../../inertia-tensor.md) gives [angular momentum](../../../../../../angular-momentum.md) $C\dot\theta$ in that direction. The [torque](../../../../../../torque.md) equation is therefore

$$
C\ddot\theta=bF,\qquad F=\frac{C}{b^2}\ddot x.
$$

Eliminating [static friction](../../../../../../static-friction.md) and inserting $C$ gives

$$
\left(M+\frac{C}{b^2}\right)\ddot x=Mg\sin\varphi,
\qquad
\boxed{\left(1+\frac{a^2+b^2}{2b^2}\right)\ddot x=g\sin\varphi.}
$$

The extra term represents the rotational [inertia](../../../../../../inertia.md) that must be accelerated along with the translational [mass](../../../../../../mass.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
