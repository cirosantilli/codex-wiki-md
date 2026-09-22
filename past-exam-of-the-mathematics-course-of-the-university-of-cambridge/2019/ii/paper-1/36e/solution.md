<h1 id="36e/solution">Solution</h1>

↑ **Parent:** [36E](../36e.md)

For a constant [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md), the [relativistic Lorentz force](../../../../../relativistic-lorentz-force.md) is a linear system with constant coefficients, so

$$
\boxed{u^\mu(\tau)=
\left[\exp\!\left(\frac qmF\tau\right)\right]^\mu{}_{\nu}u^\nu(0).}
$$

Put

$$
a=\frac{qE}{mc},
\qquad
b=\frac{qB}{m},
\qquad
\gamma_0=\frac1{\sqrt{1-v_0^2/c^2}}.
$$

The initial [four-velocity](../../../../../four-velocity.md) is $(u^0,u^1,u^2,u^3)=\gamma_0(c,0,v_0,0)$. For parallel fields along $x$, the field tensor has one hyperbolic block in the $(0,1)$ plane and one rotation block in the $(2,3)$ plane. With the orientation convention in the question,

$$
u^0=\gamma_0c\cosh(a\tau),
\qquad
u^1=\gamma_0c\sinh(a\tau),
$$



$$
u^2=\gamma_0v_0\cos(b\tau),
\qquad
u^3=-\gamma_0v_0\sin(b\tau).
$$

Taking the initial spacetime point to be the origin and integrating $u^\mu=dx^\mu/d\tau$ gives the [relativistic motion in parallel electric and magnetic fields](../../../../../relativistic-motion-in-parallel-electric-and-magnetic-fields.md)

$$
\boxed{
\begin{aligned}
t(\tau)&=\frac{\gamma_0}{a}\sinh(a\tau),\\
x(\tau)&=\frac{\gamma_0c}{a}\bigl(\cosh(a\tau)-1\bigr),\\
y(\tau)&=\frac{\gamma_0v_0}{b}\sin(b\tau),\\
z(\tau)&=\frac{\gamma_0v_0}{b}\bigl(\cos(b\tau)-1\bigr).
\end{aligned}}
$$

The expressions have their continuous $a\to0$ or $b\to0$ limits when one field vanishes; reversing the sign of $q$ reverses the electric acceleration and magnetic rotation.

Eliminating [proper time](../../../../../proper-time.md) between the first two equations yields

$$
\boxed{x(t)=\frac{\gamma_0c}{a}
\left[\sqrt{1+\left(\frac{at}{\gamma_0}\right)^2}-1\right].}
$$

At early coordinate time,

$$
x(t)=\frac{qE}{2m\gamma_0}t^2+O(t^4),
$$

which is uniformly accelerated motion with the transverse relativistic inertia factor $\gamma_0$. At late positive time,

$$
x(t)=\operatorname{sgn}(qE)ct-\frac{\gamma_0mc^2}{qE}+O(t^{-1}),
$$

so the longitudinal speed approaches the [speed of light](../../../../../speed-of-light.md).

The $y$-$z$ projection satisfies

$$
y^2+\left(z+\frac{\gamma_0v_0}{b}\right)^2
=\left(\frac{\gamma_0v_0}{b}\right)^2.
$$

It is therefore a circle of radius and proper-time period

$$
\boxed{R=\frac{\gamma_0m|v_0|}{|q|B},
\qquad
\Delta\tau=\frac{2\pi m}{|q|B}.}
$$

For the pitch magnitude assume $v_0>0$ and put $\alpha=|q|E/(mc)$, $\Omega=|q|B/m$, and

$$
r=\alpha\Delta\tau=\frac{2\pi E}{cB}.
$$

Number the $n$th proper-time period as $[(n-1)\Delta\tau,n\Delta\tau]$. Its longitudinal displacement is

$$
\Delta x_n=\frac{\gamma_0c}{\alpha}
\bigl[\cosh(nr)-\cosh((n-1)r)\bigr].
$$

Consequently, as $n\to\infty$,

$$
P_n=\frac{\Delta x_n}{R}
\sim\frac{c\Omega}{2\alpha v_0}(1-e^{-r})e^{nr}
=A\exp\!\left(\frac{2\pi En}{cB}\right),
$$

where

$$
\boxed{A=\frac{c^2B}{2Ev_0}
\left(1-e^{-2\pi E/(cB)}\right).}
$$

## ↑ Ancestors (10)

1. [36E](../36e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
