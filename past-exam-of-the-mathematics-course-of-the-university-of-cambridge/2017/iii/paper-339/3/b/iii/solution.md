<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Pair the off-circle [roots of a polynomial](../../../../../../../root-of-a-polynomial.md) using [reciprocal-conjugate root pairing](../../../../../../../reciprocal-conjugate-root-pairing.md), and split each unit-circle [root of a polynomial](../../../../../../../root-of-a-polynomial.md)'s even multiplicity equally between the two members of a pair. The [fundamental theorem of algebra](../../../../../../../fundamental-theorem-of-algebra.md) and the leading [coefficient](../../../../../../../coefficient.md) $p_d$ give $P(z)=p_d\prod_{i=1}^d(z-\zeta_i)(z-1/\overline{\zeta_i})$. None of the selected $\zeta_i$ is zero.

On the [unit circle](../../../../../../../complex-unit-circle.md), the identity

$$
z-\frac1{\overline{\zeta_i}}
=-\frac z{\overline{\zeta_i}}(\overline z-\overline{\zeta_i})
$$

turns $P(z)/z^d$ into

$$
p(z)=c\prod_{i=1}^d(z-\zeta_i)(\overline z-\overline{\zeta_i})
=c\prod_{i=1}^d|z-\zeta_i|^2,\qquad
c=\frac{(-1)^dp_d}{\prod_i\overline{\zeta_i}}.
$$

At a point of the [unit circle](../../../../../../../complex-unit-circle.md) outside the finite set of [roots of a polynomial](../../../../../../../root-of-a-polynomial.md), the product is positive and $p(z)$ is nonzero and nonnegative. Its ratio to the product is therefore real and strictly positive. This proves $c>0$, even though the algebraic expression initially permits a complex constant. Consequently

$$
\boxed{q(z)=\sqrt c\prod_{i=1}^d(z-\zeta_i),\qquad
p(z)=|q(z)|^2\quad(|z|=1)}.
$$

This proves the [Fejér–Riesz theorem](../../../../../../../fejer-riesz-theorem.md) for a nonzero [trigonometric polynomial](../../../../../../../trigonometric-polynomial.md) of actual order $d$. A positive constant has a constant square-root factor, and the identically zero [trigonometric polynomial](../../../../../../../trigonometric-polynomial.md) has $q=0$; if $p_d=0$ for a specified upper order $d$, reduce to the actual order first.

Although the PDF permits assuming even multiplicity, there is a short proof of [even multiplicity of unit-circle roots of a nonnegative trigonometric polynomial](../../../../../../../even-multiplicity-of-unit-circle-roots-of-a-nonnegative-trigonometric-polynomial.md). The [real analytic](../../../../../../../real-analytic-function.md) function $p(e^{i\theta})\geq0$ cannot have a zero of odd order. Near $\zeta=e^{i\theta_0}$, $e^{i\theta}-\zeta$ has a simple zero, and the nonzero factor $e^{-id\theta}$ leaves the zero order of $P(e^{i\theta})$ unchanged. Hence the [multiplicity of a root](../../../../../../../multiplicity-of-a-root.md) must be even.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
