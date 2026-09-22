<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the coordinatewise lattice operations $\omega\vee\eta$ and $\omega\wedge\eta$, [Holley's condition](../../../../../../holley-condition.md) is

$$
\boxed{\mu_1(\omega\vee\eta)\mu_2(\omega\wedge\eta)
\ge\mu_1(\omega)\mu_2(\eta)\quad\text{for all }\omega,\eta.}
$$

This sufficient condition implies $\mu_1\ge\mu_2$ by the [Holley inequality](../../../../../../holley-inequality.md). It is often stated first for strictly positive [probability](../../../../../../probability.md) weights, as will hold for the random-cluster application, but the displayed condition is also sufficient for nonnegative weights.

For clarity about the zero-weight case, apply the [four functions theorem](../../../../../../ahlswede-daykin-inequality.md) to an [increasing event](../../../../../../increasing-event.md) $A$, with the first two functions $\mu_1\mathbf1_{A^c}$ and $\mu_2\mathbf1_A$, and the last two $\mu_1\mathbf1_A$ and $\mu_2\mathbf1_{A^c}$. If $\omega\notin A$ and $\eta\in A$, then $\omega\vee\eta\in A$ and $\omega\wedge\eta\notin A$. The pointwise hypothesis is exactly the displayed cross-lattice inequality. Its summed conclusion gives

$$
\mu_1(A^c)\mu_2(A)\le\mu_1(A)\mu_2(A^c),
$$

which rearranges to $\mu_1(A)\ge\mu_2(A)$. This establishes the same statement without a positivity-of-support assumption.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
