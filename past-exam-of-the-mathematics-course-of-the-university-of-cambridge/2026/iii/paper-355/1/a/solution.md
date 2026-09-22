<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On the upper half-filament, write $\mathbf r(s)=(h(s),s)$ with $0\leq s\leq L$. To first order in slope, [resistive-force theory](../../../../../../resistive-force-theory.md) supplies the uniform transverse load $f_x=\zeta_\perp U$, and Euler--Bernoulli balance gives

$$
A h''''=\zeta_\perp U.
$$

Midpoint symmetry and clamping impose $h(0)=h'(0)=0$; the free-end force and moment conditions are $h'''(L)=h''(L)=0$. With $H=h/L$ and $\xi=s/L$,

$$
H''''(\xi)=\operatorname{Sp},
\qquad
\operatorname{Sp}=\frac{\zeta_\perp L^3U}{A}.
$$

Four integrations give

$$
\boxed{H(\xi)=\frac{\operatorname{Sp}}{24}
(\xi^4-4\xi^3+6\xi^2)}.
$$

In particular, $H(1)=\operatorname{Sp}/8$ and $H'(1)=\operatorname{Sp}/6$. The small-slope approximation first fails when the end slope is order one, giving the estimate $\operatorname{Sp}\sim6$; parametrically, breakdown occurs at [Sperm number](../../../../../../sperm-number.md) of order one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
