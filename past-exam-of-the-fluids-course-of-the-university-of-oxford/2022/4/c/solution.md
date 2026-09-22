<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiating the axisymmetric [stream function](../../../../stream-function.md) gives

$$
v_r=\frac{2C}{r}\cos\theta,\qquad
v_\theta=-\frac C r\sin\theta.
$$

The normal [kinematic boundary condition](../../../../kinematic-boundary-condition.md) fixes $C=Ua/2$, so

$$
\boxed{\Psi=\frac{Ua}{2}r\sin^2\theta,\qquad
v_r=\frac{Ua}{r}\cos\theta,\qquad
v_\theta=-\frac{Ua}{2r}\sin\theta.}
$$

Both [velocity](../../../../velocity.md) components vanish at infinity, and the axisymmetric [stream function](../../../../stream-function.md) is regular at the polar axes. The tangential component of the [strain-rate tensor](../../../../strain-rate-tensor.md) vanishes everywhere:

$$
e_{r\theta}=\frac12\left(\frac{2C}{r^2}\sin\theta
-\frac{2C}{r^2}\sin\theta\right)=0.
$$

Thus the [stress-free boundary condition](../../../../stress-free-boundary-condition.md) is satisfied. The [vorticity](../../../../vorticity-split.md) is $\omega_\phi=2C\sin\theta/r^2=Ua\sin\theta/r^2$, and the supplied dipolar [pressure](../../../../pressure-split.md) is consistent with the [Stokes equation](../../../../stokes-equation.md).

Use the [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md) $\boldsymbol\sigma=-p\mathbf I+2\eta\mathbf e$. At the bubble surface,

$$
e_{rr}=-\frac{U}{a}\cos\theta,\qquad
\sigma_{rr}=-p_0-\frac{3\eta U}{a}\cos\theta,\qquad
\sigma_{r\theta}=0.
$$

The vertical force exerted by the liquid is the integral of the vertical [traction](../../../../traction.md):

$$
F_z=\int_{r=a}(\sigma_{rr}\cos\theta-\sigma_{r\theta}\sin\theta)\,dS
=-\frac{3\eta U}{a}\,2\pi a^2\int_0^\pi\cos^2\theta\sin\theta\,d\theta.
$$

Since the integral is $2/3$, the [drag](../../../../drag-physics.md) is downward and has magnitude

$$
\boxed{F=4\pi\eta aU.}
$$

The constant [pressure](../../../../pressure-split.md) integrates to zero force. The [pressure](../../../../pressure-split.md) perturbation contributes $4\pi\eta aU/3$ and the normal viscous [stress](../../../../stress.md) contributes $8\pi\eta aU/3$; there is no tangential [traction](../../../../traction.md) contribution.

For the free-interface qualification in part (b), the calculated normal [traction](../../../../traction.md) at $\theta=0$ and $\theta=\pi$ differs by $6\eta U/a$. It cannot equal a single uniform gas [pressure](../../../../pressure-split.md) if every restoring effect is discarded. Restoring the external-minus-internal variation of [hydrostatic pressure](../../../../hydrostatic-pressure.md) supplies a term $(\rho_w-\rho_a)ga\cos\theta$. It cancels the dynamic normal [traction](../../../../traction.md) at the [terminal velocity](../../../../terminal-velocity.md) $U=(\rho_w-\rho_a)ga^2/(3\eta)$, consistent with a [spherical clean bubble without surface tension](../../../../spherical-clean-bubble-without-surface-tension.md). This distinguishes the drag calculation from the extra conditions needed for a freely rising bubble.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
