<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $(u_1,\theta_1)$ and $(u_2,\theta_2)$ be two weak solutions with the same initial data, and set $U=u_1-u_2$ and $\Theta=\theta_1-\theta_2$. The diagnostic Stokes equation gives

$$
|AU|\leq\frac{\alpha}{\nu}\|\Theta\|_2,
\qquad
\|U\|_\infty\leq C\|\Theta\|_2.
$$

Subtracting the temperature equations yields

$$
\partial_t\Theta-\kappa\Delta\Theta
+(u_1\mathbin\cdot\nabla)\Theta
+(U\mathbin\cdot\nabla)\theta_2
=\beta U\mathbin\cdot e_3.
$$

Pair this equation with $\Theta$. The term transported by $u_1$ vanishes by the [skew-symmetry of incompressible transport](../../../../../../skew-symmetry-of-incompressible-transport.md), while the other nonlinear term satisfies

$$
\left|\int_\Omega(U\mathbin\cdot\nabla\theta_2)\Theta\,dx\right|
\leq C\|\nabla\theta_2\|_2\|\Theta\|_2^2.
$$

The forcing difference is at most $C\|\Theta\|_2^2$. Consequently

$$
\frac d{dt}\|\Theta\|_2^2
\leq C\bigl(1+\|\nabla\theta_2\|_2\bigr)\|\Theta\|_2^2.
$$

The coefficient is integrable on $[0,T]$ because $\theta_2\in L^2(0,T;H^1)$. Since $\Theta(0)=0$, the [Gronwall inequality](../../../../../../gronwall-inequality.md) gives $\Theta=0$, and the Stokes equation then gives $U=0$. The weak solution is unique.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 359](../../../paper-359-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
