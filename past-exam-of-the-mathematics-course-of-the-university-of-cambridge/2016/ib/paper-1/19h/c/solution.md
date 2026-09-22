<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $L=\min_iX_i$, $R=\max_iX_i$ and $M=\max_i|X_i|=\max\{-L,R\}$. The joint [probability density](../../../../../../probability-density.md) factors as

$$
f_\theta(x)=(2\theta)^{-n}\mathbf1_{\{\theta\geq\max_i|x_i|\}}=(2\theta)^{-n}\mathbf1_{\{\theta\geq\max(-L,R)\}}.
$$

By the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md), **$T=(L,R)$ is a [sufficient statistic](../../../../../../sufficient-statistic.md)**. The same factorization shows that the smaller [statistic](../../../../../../statistic.md) $M$ is also a [sufficient statistic](../../../../../../sufficient-statistic.md). This gives the [sufficient statistic for a symmetric uniform sample](../../../../../../sufficient-statistic-for-a-symmetric-uniform-sample.md).

In fact, the [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) identifies $M$ as a [minimal sufficient statistic](../../../../../../minimal-sufficient-statistic.md): two sample points with the same $M$ have identical likelihoods for all $\theta$; with different $M$, their likelihoods have different parameter supports, and so are not proportional as functions of $\theta$. Equivalently, the condition that $f_\theta(x)=c f_\theta(y)$ for every $\theta$ and some positive constant $c$ holds exactly when their absolute maxima agree.

To see rigorously that $T$ cannot be recovered from $M$ almost surely, fix any $\theta>0$. The sample has a [distribution](../../../../../../distribution-mathematical-analysis.md) invariant under simultaneous sign reversal. If $T=h(M)$ almost surely, the same identity would hold for the sign-reversed sample on another probability-one set. Since $M$ is unchanged by sign reversal, it would follow that

$$
(L,R)=(-R,-L)\quad\text{almost surely},
$$

and hence $L=-R$ almost surely. But this event has probability zero for a finite sample from a continuous [uniform distribution](../../../../../../continuous-uniform-distribution.md): it entails $X_i=-X_j$ for some pair of indices, including the possible case $X_i=0$. Therefore $T$ is not a function of the sufficient statistic $M$. **The pair of extrema is not minimally sufficient**, for every $n\geq1$, even though it is sufficient.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
