<h1 id="10/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Model the cart as a [particle on a fixed plane curve](../../../../../particle-on-a-fixed-plane-curve.md), remaining constrained to the track. Its vertical [velocity](../../../../../velocity.md) is $\dot y=y'(x)\dot x$, so its [kinetic energy](../../../../../kinetic-energy.md), [gravitational potential energy](../../../../../gravitational-energy.md) and [Lagrangian](../../../../../lagrangian.md) are

$$
T=\frac m2[1+y'(x)^2]\dot x^2,\qquad
V=mgy(x),\qquad
L=\frac m2[1+y'^2]\dot x^2-mgy.
$$

Consequently the [canonical momentum](../../../../../canonical-momentum.md) conjugate to the horizontal coordinate is

$$
\boxed{p_x=m[1+y'^2]\dot x.}
$$

It is not simply the horizontal component $m\dot x$ of the mechanical [momentum](../../../../../momentum-split.md), because a change in $x$ also moves the cart vertically. Differentiate carefully in the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md):

$$
\frac{d p_x}{dt}=m(1+y'^2)\ddot x+2my'y''\dot x^2,
\qquad
\frac{\partial L}{\partial x}=my'y''\dot x^2-mgy'.
$$

Subtracting yields

$$
\boxed{(1+y'^2)\ddot x=-gy'-y'y''\dot x^2.}
$$

The term involving $y''$ accounts for the changing track geometry. An independent check is [conservation of energy](../../../../../conservation-of-energy.md):

$$
H=\frac m2(1+y'^2)\dot x^2+mgy,
\qquad
\frac{dH}{dt}=m\dot x\big[(1+y'^2)\ddot x+y'y''\dot x^2+gy'\big]=0.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [10](../../../10.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the physics 1 paper of the University of Oxford](../../../../split.md)
6. [Physics 1 paper of the University of Oxford](../../../../../physics-1-paper-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
