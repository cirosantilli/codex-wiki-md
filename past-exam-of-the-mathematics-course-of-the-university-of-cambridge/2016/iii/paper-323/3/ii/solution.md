<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Gamma=T_B$ denote the [partial transpose](../../../../../../partial-transpose.md). The [partial transpose of a maximally entangled projector](../../../../../../partial-transpose-of-a-maximally-entangled-projector.md) is

$$
(\phi^+)^\Gamma=\frac1d\sum_{i,j}|i\rangle\langle j|\otimes|j\rangle\langle i|=\frac Sd,
$$

where $S$ is the [swap operator](../../../../../../swap-operator.md), satisfying $S^\dagger S=I$ and $\|S\|_{\rm op}=1$. If $\sigma$ has [positive partial transpose](../../../../../../positive-partial-transpose.md), then $\sigma^\Gamma$ is a [positive operator](../../../../../../positive-operator.md) of [trace](../../../../../../matrix-trace.md) one, hence $\|\sigma^\Gamma\|_1=1$.

For a [pure state](../../../../../../pure-state.md) $\phi^+=|\Phi\rangle\langle\Phi|$, the unsquared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) obeys $F(\phi^+,\sigma)^2=\langle\Phi|\sigma|\Phi\rangle$. Using the [trace-adjoint identity for partial transpose](../../../../../../trace-adjoint-identity-for-partial-transpose.md) and part (i),

$$
F(\phi^+,\sigma)^2
=\operatorname{Tr}(\phi^+\sigma)
=\frac1d\operatorname{Tr}(S\sigma^\Gamma)
\leq\frac1d\|\sigma^\Gamma\|_1=\frac1d.
$$

The overlap is nonnegative, so taking its square root proves **the [PPT maximally entangled overlap bound](../../../../../../ppt-maximally-entangled-overlap-bound.md)**:

$$
\boxed{F(\phi^+,\sigma)\leq\frac1{\sqrt d}.}
$$

The [product state](../../../../../../product-state.md) $|00\rangle\langle00|$ attains the bound, so it is sharp.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
