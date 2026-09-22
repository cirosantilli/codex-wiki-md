<h1 id="34a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $H_0|r\rangle=E_r|r\rangle$. In the [interaction picture](../../../../../../interaction-picture.md),

$$
\delta H_I(t)
=e^{iH_0t/\hbar}\delta H(t)e^{-iH_0t/\hbar},
$$

and the state obeys

$$
i\hbar\frac d{dt}|\psi_I(t)\rangle
=\delta H_I(t)|\psi_I(t)\rangle.
$$

The first term of the [Dyson series](../../../../../../dyson-series.md), or equivalently first-order [time-dependent perturbation theory](../../../../../../time-dependent-perturbation-theory.md), gives

$$
|\psi_I(t)\rangle
=\left[
1-\frac i\hbar\int_0^t\delta H_I(t')\,dt'
\right]|\psi(0)\rangle
+O(\delta H^2).
$$

Thus, if $|\psi(0)\rangle=\sum_ra_r|r\rangle$,

$$
\boxed{
|\psi_I(t)\rangle
=\sum_s\left[
a_s-\frac i\hbar\sum_ra_r
\int_0^t
e^{i(E_s-E_r)t'/\hbar}
\langle s|\delta H(t')|r\rangle\,dt'
\right]|s\rangle
+O(\delta H^2)
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34A](../../34a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
