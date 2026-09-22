<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) of a [product measure](../../../../../../product-measure.md) is the sum of the individual divergences, by expanding the logarithm of the [likelihood ratio](../../../../../../likelihood-ratio.md) and taking its [expected value](../../../../../../expected-value.md). Put $q=1/2-t/\sqrt n$ and define $W(S)$ to be the unordered pairs lying within one group, while $C(S)$ is the set of unordered pairs crossing between groups. Then

$$
D_{\mathrm{KL}}(P_S\Vert P_{S'})=\sum_{e\in W(S)\setminus W(S')}D_{\mathrm{KL}}(\operatorname{Ber}(1/2)\Vert\operatorname{Ber}(q))+\sum_{e\in W(S')\setminus W(S)}D_{\mathrm{KL}}(\operatorname{Ber}(q)\Vert\operatorname{Ber}(1/2)).
$$

Thus choosing the printed $\partial S$ to mean $W(S)$ gives its order of the summands. If $\partial S$ denotes the usual [graph cut](../../../../../../graph-cut.md) $C(S)$, their two orders must be interchanged. Each unordered [edge](../../../../../../edge-of-a-graph.md) is counted once.

The inequality $\log x\leq x-1$ gives

$$
\boxed{D_{\mathrm{KL}}(\operatorname{Ber}(p)\Vert\operatorname{Ber}(q))\leq p\left(\frac pq-1\right)+(1-p)\left(\frac{1-p}{1-q}-1\right)=\frac{(p-q)^2}{q(1-q)}.}
$$

Since $1/3<q<1/2$, each changed-edge divergence is at most $9t^2/(2n)$. Summing over at most $n(n-1)/2$ pairs gives $D_{\mathrm{KL}}(P_S\Vert P_{S'})\leq9nt^2/4$. This is the information scale needed for [Fano's inequality](../../../../../../fano-s-inequality.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
