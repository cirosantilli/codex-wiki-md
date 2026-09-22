<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $t>0$, differentiate

$$
u(t)=\mathbb E[f(\sqrt tZ)].
$$

The growth assumptions justify differentiation under the expectation, and [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md) gives

$$
\begin{aligned}
u'(t)
&=\frac1{2\sqrt t}\mathbb E[Zf'(\sqrt tZ)]\\
&=\frac1{2\sqrt t}\mathbb E\left[
\frac d{dZ}f'(\sqrt tZ)\right]\\
&=\frac12\mathbb E[f''(\sqrt tZ)].
\end{aligned}
$$

Since $u(0)=f(0)$, integration from $0$ to $t$ yields the [Brownian transition semigroup](../../../../../../brownian-transition-semigroup.md) identity

$$
\boxed{
\frac12\int_0^t\mathbb E[f''(\sqrt sZ)]\,ds
=\mathbb E[f(\sqrt tZ)]-f(0)}.
$$

Continuity at zero covers $t=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
