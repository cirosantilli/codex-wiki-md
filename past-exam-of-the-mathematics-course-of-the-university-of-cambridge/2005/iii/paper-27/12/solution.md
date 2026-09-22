<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

The [Fodor lemma](../../../../../fodor-lemma.md), also called [Fodor's theorem](../../../../../fodor-lemma.md), states: if $\kappa$ is a regular uncountable [cardinal](../../../../../cardinal-number.md), $S\subseteq\kappa$ is stationary and $f:S\to\kappa$ is regressive, meaning $f(\alpha)<\alpha$ for every nonzero $\alpha\in S$, then some fibre $f^{-1}(\{\xi\})$ is stationary.

Delete zero from $S$, which preserves stationarity. Suppose no fibre is stationary. For each $\xi<\kappa$, choose a [club set](../../../../../club-set.md) $C_\xi$ avoiding that fibre. The [diagonal intersection](../../../../../diagonal-intersection.md)

$$
C=\{\alpha<\kappa:(\forall\xi<\alpha)\ \alpha\in C_\xi\}
$$

is a club. To prove unboundedness, start above an arbitrary bound and choose a strictly increasing sequence $\alpha_n$ with $\alpha_{n+1}$ in every $C_\xi$ for $\xi\le\alpha_n$. The intersection of these fewer-than-$\kappa$ clubs is club by [club filter completeness](../../../../../club-filter-completeness.md). Put $\alpha=\sup_n\alpha_n<\kappa$. For any $\xi<\alpha$, every sufficiently late $\alpha_n$ lies in $C_\xi$, so its closure gives $\alpha\in C_\xi$. Thus $\alpha\in C$. For closure of $C$, let $\alpha<\kappa$ be a limit point of $C$; for each $\xi<\alpha$, the members of $C$ above $\xi$ witnessing that limit lie in $C_\xi$, and closure gives $\alpha\in C_\xi$.

Stationarity supplies $\alpha\in S\cap C$. Since $f(\alpha)<\alpha$, we have $\alpha\in C_{f(\alpha)}$, but that club was chosen to avoid the fibre containing $\alpha$. This contradiction proves the theorem. For completeness, [club filter completeness](../../../../../club-filter-completeness.md) follows by a similar diagonal sequence: cycle through fewer than $\kappa$ clubs over $\omega$ rounds, each time choosing a larger member of the next club. Regularity keeps the supremum below $\kappa$, and every club is visited cofinally often in the construction, so its closure contains the supremum. Their intersection is also closed.

## ↑ Ancestors (10)

1. [12](../12.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
