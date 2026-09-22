<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Both positive-density components have nonnegative [pressure](../../../../pressure-split.md), so the [Friedmann acceleration equation](../../../../friedmann-acceleration-equation.md) gives $\ddot a<0$ whenever $a>0$. Suppose $a(t_1)=a_1>0$ and $\dot a(t_1)=v_1>0$. Going backward while the solution is regular, $\dot a(t)\ge v_1$. Integrating,

$$
a_1-a(t)=\int_t^{t_1}\dot a(s)\,ds\ge v_1(t_1-t),
$$

and therefore

$$
a(t)\le a_1-v_1(t_1-t).
$$

A positive [scale factor](../../../../scale-factor-cosmology.md) cannot persist indefinitely into the past: the right side vanishes at the finite time $t_1-a_1/v_1$.

For completeness, in this model the past endpoint must actually have $a\to0$, rather than another singularity at positive $a$. From part (d) write $\rho_m=C_m/a^3$ and $\rho_r=C_r/a^4$ with $C_m,C_r>0$. Then

$$
\dot a^2=\frac{K_m}{a}+\frac{K_r}{a^2}-c^2k,
\qquad
K_i=\frac{8\pi G}{3}C_i>0.
$$

The right side strictly decreases with $a$ and is positive at $a_1$, so it remains positive throughout $0<a<a_1$. There is no earlier bounce. It is smooth at every positive $a$, permitting continuation there. The lookback integral is

$$
t_1-t_0
=\int_0^{a_1}
\frac{da}{\sqrt{K_m/a+K_r/a^2-c^2k}}<\infty.
$$

Near $a=0$ its integrand is $a/\sqrt{K_r}$, which is integrable. Thus

$$
\boxed{
\lim_{t\downarrow t_0}a(t)=0,\qquad
0<t_1-t_0\le\frac{a_1}{v_1}=H(t_1)^{-1}.
}
$$

The early asymptotic behavior is $a\simeq[2\sqrt{K_r}(t-t_0)]^{1/2}$. Both densities diverge at this [Big Bang](../../../../big-bang.md) boundary. Writing $a(t_0)=0$ denotes the limiting singular endpoint of the classical solution, not an ordinary regular spacetime slice.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
