<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

When sliding dominates and the whole cap is below the [snowline](../../../../../../snowline.md), its thickness obeys

$$
h_t=\beta(hh_x)_x-\alpha.
$$

With $\alpha=0$, this is a one-dimensional [porous medium equation](../../../../../../porous-medium-equation.md). Its mass-preserving [Barenblatt solution](../../../../../../barenblatt-solution.md) is

$$
\boxed{
h_{ss}(x,t)=
\left[A t^{-1/3}-\frac{x^2}{6\beta t}\right]_+}.
$$

Within its support,

$$
(h_{ss})_{xx}=-\frac1{3\beta t}.
$$

Now set $h=h_{ss}+ct$. Since $h_{ss}$ solves the unforced equation,

$$
h_t-\beta(hh_x)_x
=c-\beta ct(h_{ss})_{xx}
=\frac43c.
$$

Matching the uniform ablation term $-\alpha$ gives

$$
\boxed{c=-\frac{3\alpha}{4}},
\qquad
\boxed{
h(x,t)=
\left[A t^{-1/3}-\frac{x^2}{6\beta t}
-\frac{3\alpha t}{4}\right]_+}.
$$

The similarity solution has a virtual origin. Writing $s=t+t_0$ gives the exact decaying family

$$
h(x,t)=
\left[
C s^{-1/3}-\frac{x^2}{6\beta s}
-\frac{3\alpha s}{4}
\right]_+.
$$

If its initial centre thickness is $h^*$, then $C=(h^*+3\alpha t_0/4)t_0^{1/3}$ and the exact extinction time is

$$
t_{\rm melt}
=t_0\left[
\left(1+\frac{4h^*}{3\alpha t_0}\right)^{3/4}-1
\right].
$$

Its value depends on the initial cap width through the virtual age $t_0$, but its dimensional scale is unambiguously

$$
\boxed{t_{\rm melt}=O\left(\frac{h^*}{\alpha}\right)}.
$$

The additive melting correction alone has the corresponding time $4h^*/(3\alpha)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
