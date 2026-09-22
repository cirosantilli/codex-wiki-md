<h1 id="h/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the position of a mass element relative to the [centre of mass](../../../../center-of-mass.md) as $r$. Expand its squared [velocity](../../../../velocity.md) and integrate:

$$
T=\frac12\int|v_G+\omega\times r|^2\,dm
=\frac12M|v_G|^2+\frac12\int|\omega\times r|^2\,dm.
$$

The mixed term vanishes because $\int r\,dm=0$. Also

$$
L_G=\int r\times(\omega\times r)\,dm,\qquad
\omega\cdot L_G=\int|\omega\times r|^2\,dm,
$$

using the scalar triple-product identity. Therefore

$$
\boxed{T=\tfrac12M|v_G|^2+\tfrac12\omega\cdot L_G.}
$$

In [principal axes](../../../../principal-axis.md) the [inertia tensor](../../../../inertia-tensor.md) is diagonal, so the second term is $\tfrac12(A\omega_1^2+B\omega_2^2+C\omega_3^2)$. Substituting the three Euler-angle components given in the source gives its displayed kinetic-energy expression directly.

For $A=B$, the first two component squares have opposite mixed terms and sum to $\dot\theta^2+\dot\phi^2\sin^2\theta$. Put $n=\dot\psi+\dot\phi\cos\theta$. Using the orientation-dependent potential printed in the source therefore gives the formal model

$$
L=\tfrac12 A\dot\theta^2+\tfrac12 A\dot\phi^2\sin^2\theta+\tfrac12 Cn^2
+\tfrac12M(\dot x^2+\dot y^2+\dot z^2)-Mgz\cos\theta.
$$

The [cyclic coordinates](../../../../cyclic-coordinate.md) $x,y,\psi$ have conserved momenta $M\dot x,M\dot y,Cn$. Consequently $\dot x,\dot y,n$ are constant. The coordinate $\phi$ is also cyclic, with

$$
p_\phi=A\dot\phi\sin^2\theta+Cn\cos\theta.
$$

For imposed fixed tilt $\theta=\alpha\in(0,\pi/2)$, conservation of $n$ and $p_\phi$ forces $\dot\phi=\Omega$ constant. Impose the fixed-height condition $z=h$ in this formal constrained model. Its $\theta$ equation is

$$
A\ddot\theta-A\dot\phi^2\sin\theta\cos\theta
+Cn\dot\phi\sin\theta-Mgz\sin\theta=0.
$$

[Set](../../../../set-split.md) the tilt constant and divide by its nonzero sine. This gives

$$
\boxed{A\Omega^2\cos\alpha-Cn\Omega+Mgh=0.}
$$

A real [polynomial root](../../../../root-of-a-polynomial.md) requires its [quadratic discriminant](../../../../quadratic-discriminant.md) to be nonnegative:

$$
\boxed{C^2n^2\ge4AMgh\cos\alpha.}
$$

When this condition holds the two algebraic rates are $(Cn\pm\sqrt{C^2n^2-4AMgh\cos\alpha})/(2A\cos\alpha)$.

There is a physical inconsistency in the printed data that must be kept distinct from this algebra. If $(x,y,z)$ are literally [Cartesian coordinates](../../../../cartesian-coordinate-system.md) of the [centre of mass](../../../../center-of-mass.md) in uniform [gravity](../../../../gravity.md), the [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md) is $Mgz$, not $Mgz\cos\theta$. The printed [Lagrangian](../../../../lagrangian.md) consequently does not follow from that Cartesian-height interpretation. Moreover its unconstrained $z$ equation is $\ddot z=-g\cos\theta$, so constant height at the indicated tilt requires a constraint reaction. The requested rate and [discriminant](../../../../discriminant.md) follow from the printed orientation-dependent potential with fixed height imposed; a standard heavy-top interpretation instead uses a height proportional to an axis distance times $\cos\theta$, with the reference point and corresponding inertia specified consistently. The kinetic-energy derivation is independent of this source inconsistency.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [H](../../h.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
