<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\omega_h=\dot\alpha$, positive on opening. The [no-slip boundary condition](../../../../no-slip-boundary-condition.md) equates the fluid [velocity](../../../../velocity.md) with each plate's [velocity](../../../../velocity.md):

$$
\begin{aligned}
v_r(r,0)&=v_\theta(r,0)=0,\\
v_r(r,\alpha)&=0,\qquad v_\theta(r,\alpha)=r\omega_h.
\end{aligned}
$$

The upper condition is a moving-wall [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md), not zero normal [velocity](../../../../velocity.md) in the laboratory frame. At the hinge the [velocity](../../../../velocity.md) tends to zero. With the arbitrary constant of the [streamfunction](../../../../stream-function.md) chosen so that $\psi(r,0)=0$, these conditions become

$$
\psi_\theta(r,0)=\psi_\theta(r,\alpha)=0,\qquad
\psi(r,\alpha)=-\frac12\omega_h r^2.
$$

A changing angle cannot give a literally [steady flow](../../../../steady-flow.md) in fixed coordinates. We interpret the stated steadiness as the [quasi-steady Stokes approximation](../../../../quasi-steady-stokes-approximation.md) at each instantaneous $\alpha$.

**The printed expression is not biharmonic.** To test it without reproducing the source formula, write its bracket as $G_p(\theta)$ and its [streamfunction](../../../../stream-function.md) as $\psi_p=-\Omega r^2G_p/2$. For any angular function $G$, the [Laplacian](../../../../laplacian.md) gives

$$
\nabla^4(r^2G)=\frac{G^{(4)}+4G''}{r^2}.
$$

At the concrete angle $\alpha=\pi/4$, differentiation of the printed bracket gives

$$
G_p^{(4)}+4G_p''
=\frac{-16\pi\cos2\theta+32\sin2\theta}{\pi^2/4-1}.
$$

For example, at the interior point $\theta=\pi/8$,

$$
\boxed{\nabla^4\psi_p
=\frac{4\sqrt2(\pi-2)\Omega}{(\pi^2/4-1)r^2}\ne0\quad(\Omega\ne0).}
$$

The printed bracket does satisfy $G_p(0)=G_p'(0)=G_p'(\alpha)=0$ and $G_p(\alpha)=1$, so its boundary [velocities](../../../../velocity.md) would require $\Omega=\omega_h$. Satisfying these [boundary conditions](../../../../boundary-condition.md) does not cure its nonzero [biharmonic operator](../../../../biharmonic-operator.md). The stated series is likewise not a general biharmonic basis: its $r^2\theta\sin2\theta$ term already fails the displayed test. The [separated polar solutions of the biharmonic equation](../../../../separated-polar-solutions-of-the-biharmonic-equation.md) contain additional radial powers; for the required $r^2$ dependence, the angular basis is $1,\theta,\sin2\theta,\cos2\theta$.

The corrected [slowly opening Stokes wedge](../../../../slowly-opening-stokes-wedge.md) [similarity solution](../../../../similarity-solution.md) follows by setting $\psi=-\omega_h r^2G(\theta)/2$. The [biharmonic equation](../../../../biharmonic-equation.md) gives $G^{(4)}+4G''=0$. The two lower-wall conditions reduce its general solution to

$$
G=A(\cos2\theta-1)+B(\sin2\theta-2\theta).
$$

The upper-wall condition $G'(\alpha)=0$ fixes the ratio of $A$ and $B$, and $G(\alpha)=1$ fixes their scale. An expression that also remains finite at $\alpha=\pi/2$ is

$$
\boxed{G(\theta)=
\frac{\sin\alpha(1-\cos2\theta)+\cos\alpha(\sin2\theta-2\theta)}
{2(\sin\alpha-\alpha\cos\alpha)},\qquad
\psi=-\frac12\dot\alpha r^2G(\theta).}
$$

For $0<\alpha<\pi$, its denominator is positive: the [derivative](../../../../derivative.md) of $\sin\alpha-\alpha\cos\alpha$ is $\alpha\sin\alpha>0$. Direct differentiation verifies all four [boundary conditions](../../../../boundary-condition.md) and the [biharmonic equation](../../../../biharmonic-equation.md). The resulting [velocity](../../../../velocity.md) components are $v_r=-\dot\alpha rG'/2$ and $v_\theta=\dot\alpha rG$.

For a fixed angle of order one, $U(r)\sim|\dot\alpha|r$, so the local [Reynolds number](../../../../reynolds-number.md) is $\mathrm{Re}_r\sim|\dot\alpha|r^2/\nu$. One breakdown [length](../../../../length.md) is therefore

$$
\boxed{l_1\sim\sqrt{\frac{\nu}{|\dot\alpha|}}.}
$$

A second is the geometric [length](../../../../length.md) $l_2\sim\min(L,W)$, where $L$ is the distance to the radial ends and $W$ the spanwise width. At $r\sim l_2$, matching to the surrounding bath or three-dimensional end flow matters. Thus $r\ll\min(l_1,l_2)$ is required for this local two-dimensional [Stokes flow](../../../../stokes-flow-split.md), with angle-dependent factors in the inertial estimate. Ideal infinite plates remove the geometric cutoff but not the inertial one.

There is also a temporal restriction: the relevant [viscous diffusion time](../../../../viscous-diffusion-time.md) must be short compared with the time $T_s$ over which the shape and its [velocity field](../../../../velocity-field.md) change appreciably. Using $r$ as a conservative diffusion [length](../../../../length.md) gives $r\ll\sqrt{\nu T_s}$. For order-one angles and constant $\dot\alpha$, $T_s\sim|\dot\alpha|^{-1}$ gives the same scale as $l_1$; narrow angles require using their actual gap and angular factors rather than extrapolating this order-one-angle estimate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
