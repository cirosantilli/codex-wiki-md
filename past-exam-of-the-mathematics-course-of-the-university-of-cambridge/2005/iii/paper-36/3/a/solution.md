<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\kappa=2(1-H)>0$. For the [Gaussian process](../../../../../../gaussian-process.md) $Z$, [self-similarity of a stochastic process](../../../../../../self-similarity-of-a-stochastic-process.md) gives the identity in distribution

$$
\frac{Z(N\,\cdot)}{N}\ \overset d=\ N^{H-1}Z
=\frac{Z}{\sqrt{N^\kappa}}.
$$

Apply the given small-noise [large deviation principle](../../../../../../large-deviation-principle.md) with $L=N^\kappa$. The answer is

$$
\boxed{\text{speed }N^{2(1-H)},\qquad\text{good rate function }I.}
$$

No [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) needs to be recomputed: the scaled paths have exactly the small-noise law at this scale.

If the stated small-noise [large deviation principle](../../../../../../large-deviation-principle.md) is indexed only by integer $L$, use $L_N=\lfloor N^\kappa\rfloor$. This gives speed $N^\kappa$ as well, since $L_N/N^\kappa\to1$. The multiplying factor $\sqrt{L_N/N^\kappa}\to1$ does not change the [large deviation principle](../../../../../../large-deviation-principle.md). To justify this last step, the error in the path norm is $o(1)\|Z/\sqrt{L_N}\|$. For each fixed $M$, [good rate functions](../../../../../../good-rate-function.md) have bounded sublevel sets, so $\inf_{\|f\|\geq M}I(f)\to\infty$ as $M\to\infty$. The closed-set upper bound then makes the [probability](../../../../../../probability.md) of an error greater than any fixed $\eta>0$ superexponentially small. Thus [exponential equivalence](../../../../../../exponential-equivalence.md) applies. This also justifies positive real, rather than only integer, rescalings used in part (c).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
