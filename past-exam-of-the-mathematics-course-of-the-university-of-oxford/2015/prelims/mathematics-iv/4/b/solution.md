<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $c=\mathbf k\cdot\mathbf e$. Since $\mathbf s=\ell(\mathbf k-\mathbf e)$, the total [torque](../../../../../../torque.md) simplifies to

$$
\boldsymbol\tau=(\kappa\ell^2-mgh)\mathbf e\wedge\mathbf k.
$$

Taking the [dot product](../../../../../../dot-product.md) of the equation of motion with $\mathbf e$ gives $C\dot n=0$: both [torque](../../../../../../torque.md) terms are perpendicular to $\mathbf e$, as are the other terms on the left. Hence

$$
\boxed{n=\text{constant}.}
$$

Taking the [dot product](../../../../../../dot-product.md) of $\dot{\mathbf L}_Q=\boldsymbol\tau$ with the fixed [vector](../../../../../../vector.md) $\mathbf k$ gives

$$
\dot p=\mathbf k\cdot\dot{\mathbf L}_Q=0,\qquad
\boxed{p=\mathbf k\cdot\mathbf L_Q=\text{constant}.}
$$

These are conservation of the axial spin and of the vertical component of [angular momentum](../../../../../../angular-momentum.md).

For [energy](../../../../../../energy-split.md), the [kinetic energy](../../../../../../kinetic-energy.md) and [potential energy](../../../../../../potential-energy.md) are

$$
T=\frac12\boldsymbol\omega\cdot\mathbf L_Q
=\frac A2|\dot{\mathbf e}|^2+\frac C2n^2,
\qquad
V=mghc+\frac\kappa2|\mathbf s|^2
=mghc+\kappa\ell^2(1-c).
$$

Dot the equation of motion, with $\dot n=0$, with $\mathbf e\wedge\dot{\mathbf e}$. The [cross product](../../../../../../cross-product.md) identity $(\mathbf e\wedge\mathbf u)\cdot(\mathbf e\wedge\mathbf v)=\mathbf u\cdot\mathbf v-(\mathbf e\cdot\mathbf u)(\mathbf e\cdot\mathbf v)$ gives

$$
A\ddot{\mathbf e}\cdot\dot{\mathbf e}
=(\kappa\ell^2-mgh)\mathbf k\cdot\dot{\mathbf e}.
$$

It follows that

$$
\dot T=(\kappa\ell^2-mgh)\dot c,\qquad
\dot V=(mgh-\kappa\ell^2)\dot c,
$$

so

$$
\boxed{E=T+V=\frac12\boldsymbol\omega\cdot\mathbf L_Q+mgh\mathbf k\cdot\mathbf e+\frac\kappa2|\mathbf s|^2=\text{constant}.}
$$

The applied [force](../../../../../../force-split.md) is conservative even if $\kappa$ is negative: its [potential energy](../../../../../../potential-energy.md) is $\kappa|\mathbf s|^2/2$. This is a [symmetric top with a quadratic alignment potential](../../../../../../symmetric-top-with-a-quadratic-alignment-potential.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
