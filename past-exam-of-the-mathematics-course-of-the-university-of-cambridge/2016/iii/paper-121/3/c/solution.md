<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [club filter completeness](../../../../../../club-filter-completeness.md) argument works for every regular uncountable $\kappa$. Let $\mu<\kappa$ and let $C_i$ be a [club set](../../../../../../club-set.md) for each $i<\mu$. Their intersection is closed. To prove it unbounded, start above any prescribed $\beta<\kappa$ and choose an increasing sequence $(\delta_n)_{n<\omega}$ so that $\delta_{n+1}$ lies above a chosen point of every $C_i$ greater than $\delta_n$. $\kappa$ is a [regular cardinal](../../../../../../regular-cardinal.md), so the supremum of these $\mu$ choices remains below $\kappa$. The resulting countable supremum $\delta=\sup_n\delta_n$ likewise remains below $\kappa$. For each $i$, the chosen $C_i$ points are cofinal in $\delta$, so closure gives $\delta\in C_i$. Thus the intersection is a [club set](../../../../../../club-set.md). Intersecting fewer than $\kappa$ members of the [club filter](../../../../../../club-filter.md) still contains such an intersection of clubs. In particular, $\boxed{\mathcal D_{\omega_2}\text{ is }\aleph_2\text{-complete}}$.

It is not an [ultrafilter](../../../../../../ultrafilter.md). For a regular infinite $\theta<\kappa$, the set

$$
S_\theta^\kappa=\{\delta<\kappa:\operatorname{cf}(\delta)=\theta\}
$$

is stationary. Given a [club set](../../../../../../club-set.md) $C$, build in $C$ a strictly increasing continuous sequence of length $\theta$ and take its supremum $\delta<\kappa$. Closure gives $\delta\in C$, and the [cofinality of an increasing ordinal supremum](../../../../../../cofinality-of-an-increasing-ordinal-supremum.md) gives $\operatorname{cf}(\delta)=\theta$. This proves the [stationarity of ordinals of prescribed cofinality](../../../../../../stationarity-of-ordinals-of-prescribed-cofinality.md).

At $\kappa=\omega_2$, the disjoint sets $S_\omega^{\omega_2}$ and $S_{\omega_1}^{\omega_2}$ are both stationary. A club contained in either $S_\omega^{\omega_2}$ or its complement would miss one of these stationary sets. Thus neither $S_\omega^{\omega_2}$ nor its complement belongs to $\mathcal D_{\omega_2}$, and

$$
\boxed{\mathcal D_{\omega_2}\text{ is not an ultrafilter}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
