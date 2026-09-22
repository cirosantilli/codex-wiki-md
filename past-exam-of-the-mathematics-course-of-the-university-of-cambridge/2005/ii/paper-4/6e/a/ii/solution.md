<h1 id="6e/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the modified [Hebbian learning](../../../../../../../hebbian-learning.md) rule,

$$
\tau\dot s=2y^2(1-\alpha s^2).
$$

It increases below $s_*=\alpha^{-1/2}$ and decreases above $s_*$, without crossing that equilibrium. More precisely, for a nonzero initial [norm](../../../../../../../norm.md),

$$
\frac{s(t)-s_*}{s(t)+s_*}
=\frac{s(0)-s_*}{s(0)+s_*}
\exp\!\left[-\frac{4\sqrt\alpha}{\tau}\int_0^t y(u)^2\,du\right].
$$

Under persistent excitation, meaning the integral tends to infinity, this gives

$$
\boxed{|w|\longrightarrow\alpha^{-1/4}}.
$$

Without persistent excitation the limiting [norm](../../../../../../../norm.md) need not reach this value; zero weights remain zero. The [quartic norm stabilization of Hebbian learning](../../../../../../../quartic-norm-stabilization-of-hebbian-learning.md) bounds the [norm](../../../../../../../norm.md) and supplies negative feedback at large amplitudes.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6E](../../../6e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
