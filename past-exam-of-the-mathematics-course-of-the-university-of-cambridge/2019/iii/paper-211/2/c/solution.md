<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the bound in part (a), [Fubini's theorem](../../../../../../fubini-s-theorem.md) applies. Conditional on $S$,

$$
\begin{aligned}
&\sqrt K\,\mathbb E_Y\left[
S^{(1+iY)/2}e^{-iY\log K/2}
\right]\\
&\qquad=\sqrt{KS}\,
\mathbb E_Y\exp\left(\frac{iY}{2}\log\frac SK\right)\\
&\qquad=\sqrt{KS}\,
\exp\left(-\frac12\left|\log\frac SK\right|\right)
=\min(S,K),
\end{aligned}
$$

where the [Characteristic function of the Cauchy distribution](../../../../../../characteristic-function-of-the-cauchy-distribution.md) was used. Since $\mathbb ES=1$,

$$
\mathbb E[(S-K)^+]
=\mathbb E[S-\min(S,K)]
=\boxed{1-\sqrt K\,
\mathbb E\left[M\left(\frac{1+iY}{2}\right)
e^{-iY\log K/2}\right].}
$$

The formula expresses a [European call option](../../../../../../european-call-option.md) value through complex moments of $S$. In an affine stochastic-volatility model such as the [Heston model](../../../../../../heston-model.md), those moments are available from an explicit transform, so call prices reduce to a one-dimensional Fourier expectation or integral.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
