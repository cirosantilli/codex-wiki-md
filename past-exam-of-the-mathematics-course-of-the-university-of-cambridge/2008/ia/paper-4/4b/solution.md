<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

Introduce $v=\dot x$. The [phase plane](../../../../../phase-plane.md) system for the [damped pendulum](../../../../../damped-pendulum.md) is

$$
\dot x=v,\qquad \dot v=-2kv-\omega^2\sin x.
$$

At an [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), $v=0$ and $\sin x=0$, so all [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are $\boxed{(x,v)=(n\pi,0),\ n\in\mathbb Z}$. Angles identified modulo $2\pi$ give one downward and one upward [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md).

The [linearization of a dynamical system](../../../../../linearization-of-a-dynamical-system.md) at $(n\pi,0)$ has [Jacobian matrix](../../../../../jacobian-matrix.md) and [eigenvalues](../../../../../eigenvalue.md)

$$
J_n=\begin{pmatrix}0&1\\-\omega^2(-1)^n&-2k\end{pmatrix},\qquad \lambda_\pm=-k\pm\sqrt{k^2-\omega^2(-1)^n}.
$$

When $n$ is even and $k>\omega$, both [eigenvalues](../../../../../eigenvalue.md) are real and strictly negative, since $0<\sqrt{k^2-\omega^2}<k$. These downward [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are **[stable nodes](../../../../../stable-node.md)**. When $n$ is even and $k<\omega$, the [eigenvalues](../../../../../eigenvalue.md) are $-k\pm i\sqrt{\omega^2-k^2}$, so the downward [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are **[stable foci](../../../../../stable-spiral.md)**, approached with decaying oscillations.

When $n$ is odd, $\sqrt{k^2+\omega^2}>k$, so one [eigenvalue](../../../../../eigenvalue.md) is positive and one is negative in either parameter range. Every upward [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is consequently an **unstable [saddle equilibrium](../../../../../saddle-equilibrium.md)**. All these [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are [hyperbolic equilibria](../../../../../hyperbolic-equilibrium-point.md) in the two requested cases, so their [linearization of a dynamical system](../../../../../linearization-of-a-dynamical-system.md) gives their local nonlinear classification.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
