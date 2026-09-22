<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce the [Euler differential operator](../../../../euler-differential-operator.md) $D=x\partial_x$. The fourth-order spatial expression is $D^4u$. The moving boundary has similarity coordinate $\xi=1$, so its two conditions give

$$
v(1)=0,\qquad t^\alpha v'(1)=1\quad(t>0).
$$

Hence $\alpha=0$ and $v'(1)=1$. With $D_\xi=\xi\partial_\xi$, substitution in the equation yields

$$
(D_\xi^4-\beta D_\xi)v=0,\qquad v(\xi)\to0\quad(\xi\to\infty).
$$

This is a [Cauchy-Euler equation](../../../../cauchy-euler-equation.md); putting $r=\log\xi$ turns it into the constant-coefficient equation $V^{(4)}-\beta V'=0$. Its [characteristic polynomial](../../../../characteristic-polynomial.md) is $n(n^3-\beta)$.

If $\beta>0$, write $a=\beta^{1/3}$. The roots are $0,a,-a/2\pm i\sqrt3a/2$. Decay excludes the constant and growing modes, leaving

$$
v(\xi)=\xi^{-a/2}\left[A\cos\left(\frac{\sqrt3a}2\log\xi\right)+B\sin\left(\frac{\sqrt3a}2\log\xi\right)\right].
$$

The boundary conditions force $A=0$ and $B=2/(\sqrt3a)$. If $\beta<0$, writing $\beta=-a^3$ leaves only one decaying mode, $C\xi^{-a}$; $v(1)=0$ then forces the zero function, which fails the derivative condition. If $\beta=0$, the solutions are polynomials of degree at most three in $\log\xi$, and none can both decay and satisfy $v'(1)=1$.

Consequently all real self-similar solutions are the one-parameter family

$$
\boxed{\alpha=0,\quad\beta>0,\quad s(t)=t^\beta,\quad u(x,t)=\frac{2}{\sqrt3\,\beta^{1/3}}\left(\frac{x}{t^\beta}\right)^{-\beta^{1/3}/2}\sin\left[\frac{\sqrt3\,\beta^{1/3}}2\log\left(\frac{x}{t^\beta}\right)\right]}.
$$

The [decaying profile for a fourth-order dilation equation](../../../../decaying-profile-for-a-fourth-order-dilation-equation.md) oscillates in logarithmic distance. No positivity condition on $u$ was imposed, so these sign changes are permitted.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the applied partial differential equations course of the University of Oxford](../../../split.md)
5. [Applied partial differential equations course of the University of Oxford](../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
