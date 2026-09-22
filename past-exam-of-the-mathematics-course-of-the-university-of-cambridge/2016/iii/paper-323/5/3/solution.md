<h1 id="5/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the distribution and [POVM](../../../../../../positive-operator-valued-measure.md) from part 2, apply the [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) to the [measurement channel](../../../../../../measurement-channel.md). The [quantum mutual information](../../../../../../quantum-mutual-information.md) is the [quantum relative entropy](../../../../../../quantum-relative-entropy.md) from the joint [density operator](../../../../../../density-matrix.md) to the product of its marginals, so for $k\geq2$,

$$
\begin{aligned}
I(\widetilde X:Q)_\rho
&=D(\rho_{\widetilde XQ}\|\rho_{\widetilde X}\otimes\bar\rho_Q)\\
&\geq D(\omega[\epsilon]\|\omega[1-1/k])\\
&=(1-\epsilon)\log_2 k-h_2(\epsilon)-\epsilon\log_2(1-1/k)\\
&\geq(1-\epsilon)\log_2 k-1.
\end{aligned}
$$

The last step uses $h_2(\epsilon)\leq1$ for the [binary entropy](../../../../../../binary-entropy.md) and $\log_2(1-1/k)\leq0$. If $0\leq\epsilon<1$, rearrangement and then the supremum over $P_X$ give **the [one-shot classical-quantum coding converse](../../../../../../one-shot-classical-quantum-coding-converse.md)**:

$$
\boxed{\log_2 k\leq\frac{I(\widetilde X:Q)_\rho+1}{1-\epsilon}
\leq\frac{\sup_{P_X}I(\widetilde X:Q)_{\rho_{\widetilde XQ}}+1}{1-\epsilon}.}
$$

For $k=1$, the sole [POVM](../../../../../../positive-operator-valued-measure.md) effect is $I_Q$, forcing $\epsilon=0$, and the bound is trivial. For $\epsilon=1$, division by $1-\epsilon$ is undefined: the undivided inequality remains valid and gives no size restriction. The displayed coding bound is therefore understood for $\epsilon<1$, or with a vacuous $+\infty$ right-hand side at $\epsilon=1$.

An alternative uses the original decoder directly. Let $M$ be the uniform message and $\widehat M$ its measured estimate. For $k\geq2$, [Fano's inequality](../../../../../../fano-s-inequality.md) bounds the [conditional entropy](../../../../../../conditional-entropy.md) by $H(M|\widehat M)\leq h_2(\epsilon)+\epsilon\log_2(k-1)$. The [Holevo bound](../../../../../../holevo-s-theorem.md) gives

$$
I(\widetilde X:Q)_\rho\geq I(M:\widehat M)
=\log_2 k-H(M|\widehat M)
\geq\log_2 k-h_2(\epsilon)-\epsilon\log_2(k-1)
\geq(1-\epsilon)\log_2 k-1.
$$

Thus the same coding bound follows by bounding the classical [mutual information](../../../../../../mutual-information.md) obtainable from the [POVM](../../../../../../positive-operator-valued-measure.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
