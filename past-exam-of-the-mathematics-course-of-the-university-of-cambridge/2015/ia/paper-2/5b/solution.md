<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Introduce $\omega=\dot\theta$. The [pendulum with quadratic damping](../../../../../pendulum-with-quadratic-damping.md) is the [autonomous planar system](../../../../../autonomous-planar-system.md)

$$
\boxed{\dot\theta=\omega,\qquad\dot\omega=-\sin\theta-c\omega|\omega|.}
$$

Its [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are $(k\pi,0)$. Since the derivative of $\omega|\omega|$ is zero at zero, the [linearization of a dynamical system](../../../../../linearization-of-a-dynamical-system.md) at each [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is

$$
J_k=\begin{pmatrix}0&1\\-\cos(k\pi)&0\end{pmatrix}.
$$

At an odd multiple of $\pi$ its [eigenvalues](../../../../../eigenvalue.md) are $\pm1$, so it is a [saddle equilibrium](../../../../../saddle-equilibrium.md); the stable and unstable tangents are $\omega=-(\theta-k\pi)$ and $\omega=\theta-k\pi$. At an even multiple the [eigenvalues](../../../../../eigenvalue.md) are $\pm i$. This linearization is a centre and does not decide the nonlinear stability. In particular it would be incorrect to infer a linear damped focus from this Jacobian.

For the full system the mechanical energy is a [Lyapunov function](../../../../../lyapunov-function.md) near an even [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md):

$$
H(\theta,\omega)=\frac12\omega^2+1-\cos\theta,\qquad\boxed{\dot H=-c|\omega|^3\leq0.}
$$

A sufficiently small sublevel set is compact and contains only that [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md). The only invariant motion with $\dot H=0$ has $\omega=0$ and $\sin\theta=0$, hence is the [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) itself. The [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md) proves [asymptotic stability](../../../../../asymptotic-stability.md). Near it the trajectories turn clockwise and spiral inward, as the near-linear angular motion persists while energy decreases. Thus **even equilibria are nonhyperbolic asymptotically stable spiral points; odd equilibria remain saddles**.

<a id="5b/image-local-phase-trajectories-near-a-stable-pendulum-equilibrium-and-an-unstable-saddle-with-quadratic-damping"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2-quadratic-damping.png)

**[Figure 1](#5b/image-local-phase-trajectories-near-a-stable-pendulum-equilibrium-and-an-unstable-saddle-with-quadratic-damping). Local phase trajectories near a stable pendulum equilibrium and an unstable saddle with quadratic damping**.

For explicit trajectories put $W=\omega^2$ on a branch where $\omega\ne0$. The [chain rule](../../../../../chain-rule.md) gives $dW/d\theta=2\dot\omega$, so the two signs yield the [first-order linear differential equations](../../../../../first-order-linear-differential-equation.md) $W'+2cW=-2\sin\theta$ for $\omega>0$, and $W'-2cW=-2\sin\theta$ for $\omega<0$. Their [integrating factors](../../../../../integrating-factor.md) give

$$
\boxed{\begin{aligned}\omega^2&=K_+e^{-2c\theta}+\frac{2(\cos\theta-2c\sin\theta)}{1+4c^2},&&\omega>0,\\\omega^2&=K_-e^{2c\theta}+\frac{2(\cos\theta+2c\sin\theta)}{1+4c^2},&&\omega<0.\end{aligned}}
$$

Only portions with a nonnegative right-hand side are physical. At a turning point the constants of the two branches are matched using $\omega=0$; neither expression is one global trajectory through both signs. When $c=0$ they reduce to energy contours, with closed orbits around the even [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md). For every $c>0$, the [quadratic damping](../../../../../quadratic-damping.md) destroys those closed orbits and makes the centres attracting spirals. Its effect is higher order in amplitude, so decay is weaker near rest than with linear damping. The [saddle equilibria](../../../../../saddle-equilibrium.md) remain unstable, though their separatrices change shape.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
