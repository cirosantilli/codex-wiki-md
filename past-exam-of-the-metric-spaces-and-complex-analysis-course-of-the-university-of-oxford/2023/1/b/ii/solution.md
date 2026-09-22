<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

The [intersection](../../../../../set-intersection.md) $G$ is a [closed set](../../../../../closed-set.md) because arbitrary [intersections](../../../../../set-intersection.md) of [closed sets](../../../../../closed-set.md) are closed. Its nonemptiness needs a construction: bounded closed sets need not be [compact sets](../../../../../compact-space.md) in this setting.

Fix $n$, $x_n\in F_n$, and $\eta>0$. Recursively choose $x_{k+1}\in F_{k+1}$, for $k\geq n$, using the [approximation property of an infimum](../../../../../approximation-property-of-an-infimum.md) so that

$$
d(x_k,x_{k+1})<2^{-k}+\eta\,2^{n-k-1}.
$$

This is possible because $x_k\in F_k$ and $\operatorname{dist}(x_k,F_{k+1})\leq\rho(F_k,F_{k+1})\leq2^{-k}$. The two bounds form convergent [geometric series](../../../../../geometric-series.md), so the [triangle inequality](../../../../../triangle-inequality.md) shows $(x_k)_{k\geq n}$ is a [Cauchy sequence](../../../../../cauchy-sequence.md). By [completeness](../../../../../completeness.md) it converges to some $x\in X$.

For each fixed $j$, all sufficiently late $x_k$ lie in $F_j$, by nesting. Closedness of $F_j$ gives $x\in F_j$, and hence $x\in G$. In particular, starting with any $x_1\in F_1$ proves $G\ne\varnothing$. Moreover,

$$
d(x_n,x)\leq\sum_{k=n}^{\infty}\bigl(2^{-k}+\eta\,2^{n-k-1}\bigr)=2^{1-n}+\eta.
$$

For each starting point $x_n$, let $\eta\downarrow0$ in this bound on its [distance to a set](../../../../../distance-to-a-set.md) $G$. This does not assert that a nearest point exists. It proves $\operatorname{dist}(x_n,G)\leq2^{1-n}$. Since $G\subseteq F_n$, the other directed [Hausdorff distance](../../../../../hausdorff-distance.md) is zero, and

$$
\boxed{G\in\mathcal F(X),\qquad\rho(F_n,G)\leq2^{1-n}\longrightarrow0}.
$$

This is the [Summably nested Hausdorff intersection theorem](../../../../../summably-nested-hausdorff-intersection-theorem.md); the summable movement replaces any need for [compactness](../../../../../compact-space.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
