<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
S=(1-\alpha)F_r,
\qquad
F_*=\epsilon\sigma T_m^4-S.
$$

The quasi-steady model is the coupled pair

$$
\epsilon\sigma T_s^4
=S+\frac ah\log\frac{T_m}{T_s},
\qquad
\rho L\dot h=\frac ah\log\frac{T_m}{T_s}-F_w.
$$

For a thin shell, $T_s$ is close to $T_m$. A first-order [asymptotic expansion](../../../../../../asymptotic-expansion.md) gives

$$
\log\frac{T_m}{T_s}\sim\frac{T_m-T_s}{T_m},
$$

and therefore

$$
\boxed{T_s\sim T_m-\frac{hT_m}{a}F_*},
\qquad h\ll \frac a{F_w}.
$$

To leading order $F_c\sim F_*$, so an initially freezing shell grows linearly:

$$
\boxed{h(t)\sim h(0)+\frac{F_*-F_w}{\rho L}t}.
$$

For a thick shell the conductive correction in the surface balance is small. The [radiative equilibrium](../../../../../../radiative-equilibrium.md) temperature and its first correction are

$$
T_e=\left(\frac{S}{\epsilon\sigma}\right)^{1/4},
\qquad
\boxed{T_s\sim T_e+
\frac{a\log(T_m/T_e)}
{4\epsilon\sigma T_e^3h}}.
$$

Thus, with $A=a\log(T_m/T_e)$,

$$
\boxed{\rho L\dot h\sim\frac Ah-F_w},
\qquad
h_\infty\sim\frac A{F_w}.
$$

When $F_w$ is negligible over an intermediate range, this [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives the square-root growth law

$$
h^2-h_0^2\sim\frac{2A}{\rho L}(t-t_0).
$$

Retaining $F_w$, its implicit solution is

$$
t-t_0=\frac{\rho L}{F_w}
\left[
h_0-h+h_\infty
\log\frac{h_\infty-h_0}{h_\infty-h}
\right].
$$

Consequently a sketch of $h(t)$ starts approximately linearly, crosses to square-root growth, and approaches $h_\infty$ with [exponential decay](../../../../../../exponential-decay.md) of $h_\infty-h$. A shell placed above $h_\infty$ instead thins because the basal oceanic heat flux exceeds the conductive loss.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
