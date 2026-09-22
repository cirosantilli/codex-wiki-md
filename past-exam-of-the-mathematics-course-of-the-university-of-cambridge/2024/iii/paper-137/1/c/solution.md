<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $t>0$, the product from part (b) has $q=e^{-2\pi t}\in(0,1)$, so

$$
\Delta(it)>0.
$$

The weight-twelve transformation law gives

$$
\Delta(i/t)=t^{12}\Delta(it).
$$

Together with exponential decay as $t\to\infty$, this implies rapid decay at both endpoints for the [Mellin transform](../../../../../../mellin-transform.md)

$$
I(s)=\int_0^\infty\Delta(it)t^{s-1}\,dt.
$$

The integral therefore converges for every real $s$, and its integrand is strictly positive.

In the half-plane where the Dirichlet series may be integrated term by term,

$$
I(s)=(2\pi)^{-s}\Gamma(s)L(\Delta,s).
$$

Analytic continuation preserves this identity. For real $s>0$, both $(2\pi)^s$ and the [Gamma function](../../../../../../gamma-function.md) $\Gamma(s)$ are positive, so

$$
L(\Delta,s)=\frac{(2\pi)^s}{\Gamma(s)}I(s)>0.
$$

This is the positivity statement in the [Mellin transform of the modular discriminant](../../../../../../mellin-transform-of-the-modular-discriminant.md), and in particular $L(\Delta,s)\ne0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
