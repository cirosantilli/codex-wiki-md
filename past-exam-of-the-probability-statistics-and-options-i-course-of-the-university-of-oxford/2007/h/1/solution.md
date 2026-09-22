<h1 id="h/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Autonomy gives conservation of [energy](../../../../energy-split.md), while the [cyclic coordinate](../../../../cyclic-coordinate.md) give conserved [momenta](../../../../momentum-split.md):

$$
E=\frac A2(\dot\theta^2+\dot\phi^2\sin^2\theta)
+\frac C2(\dot\psi+\dot\phi\cos\theta)^2+mga\cos\theta,
$$



$$
p_\psi=C(\dot\psi+\dot\phi\cos\theta)=Cn,\qquad
p_\phi=A\dot\phi\sin^2\theta+Cn\cos\theta=h.
$$

Here $p_\psi$ is the [angular momentum](../../../../angular-momentum.md) along the body's symmetry axis, and $p_\phi$ is its component along the fixed vertical. The time symmetry corresponds to $E$, not to an additional angle [momentum](../../../../momentum-split.md).

With $u=\cos\theta$ and $-1<u<1$, solve

$$
\dot\phi=\frac{h-Cnu}{A(1-u^2)}.
$$

Insert this and the conserved spin rate $n$ into the [energy](../../../../energy-split.md) equation, multiply by $A$, and isolate $\dot\theta$:

$$
\boxed{A^2\dot\theta^2
=\frac{A(2E-Cn^2-2mgau)(1-u^2)-(h-Cnu)^2}{1-u^2}
=\frac{P(u)}{1-u^2}.}
$$

For a fixed nonvertical angle, let

$$
V_{\rm eff}(u)=\frac{(h-Cnu)^2}{2A(1-u^2)}
+\frac12Cn^2+mgau.
$$

The [energy](../../../../energy-split.md) is $A\dot\theta^2/2+V_{\rm eff}(\cos\theta)$. A constant angle in $(0,\pi)$ requires both $E=V_{\rm eff}(u_0)$ and $V_{\rm eff}'(u_0)=0$, by the reduced [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) and $\sin\theta_0\neq0$. Since

$$
P(u)=2A(1-u^2)(E-V_{\rm eff}(u)),
$$

both $P(u_0)=0$ and $P'(u_0)=0$, with $u_0\in(-1,1)$.

The source's unqualified final sentence omits the nonvertical restriction. A vertical axis has $u=\pm1$, where the displayed reduction divides by zero and the common root need not be interior. For example, the stationary upright top has $n=h=0$, $E=mga$, and

$$
P(u)=2Amga(1-u)^2(1+u).
$$

Its only repeated root is $u=1$, so it has no common root with its derivative in $(-1,1)$. Thus **the interior double-root conclusion holds for nonvertical steady precession**. The vertical configurations require separate endpoint treatment. This is [nonvertical qualification in the steady-top double-root condition](../../../../nonvertical-qualification-in-the-steady-top-double-root-condition.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [H](../../h.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
