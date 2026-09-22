<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose zero [electrostatic potential](../../../electric-potential.md) at infinity. By [Coulomb's law](../../../coulomb-s-law.md) and the [superposition principle](../../../superposition-principle.md), the two [point charges](../../../point-charge.md) give

$$
\boxed{\Phi(r,\theta)=\frac1{4\pi\epsilon_0}\left[\frac{q_1}{\sqrt{r^2+r_1^2-2rr_1\cos\theta}}+\frac{q_2}{\sqrt{r^2+r_2^2-2rr_2\cos\theta}}\right].}
$$

Here $\epsilon_0$ is the [vacuum permittivity](../../../vacuum-permittivity.md). For a nondegenerate zero-[equipotential curve](../../../equipotential-curve.md), the [electric charges](../../../electric-charge-split.md) must have opposite signs. Let $d_1,d_2$ be the two distances. The equation $\Phi=0$ becomes $q_1d_2=-q_2d_1$, and hence

$$
q_1^2(r^2+r_2^2-2rr_2\cos\theta)=q_2^2(r^2+r_1^2-2rr_1\cos\theta).
$$

For a circle $r=\rho>0$ centred at the origin, its $\cos\theta$ coefficient must vanish: $q_1^2r_2=q_2^2r_1$. If $r_1,r_2>0$ and $r_1\ne r_2$, this gives

$$
\boxed{q_2=-q_1\sqrt{r_2/r_1}.}
$$

Substitute $q_2^2/q_1^2=r_2/r_1$ in the constant term:

$$
r_1\rho^2+r_1r_2^2=r_2\rho^2+r_2r_1^2,
\qquad (r_1-r_2)(\rho^2-r_1r_2)=0.
$$

Therefore

$$
\boxed{\rho=\sqrt{r_1r_2}.}
$$

This is an [Apollonius circle](../../../circles-of-apollonius.md): the distance ratio $d_2/d_1$ is constant. The distinct-position assumption matters. For example, $r_1=r_2=1$, $q_2=-q_1$ gives zero [electrostatic potential](../../../electric-potential.md) everywhere away from the coincident [point charges](../../../point-charge.md), so there is no distinguished zero circle. If only one position is at the origin and the other is not, no nontrivial positive-radius circle centred at the origin is possible.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2022](../../2022-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
