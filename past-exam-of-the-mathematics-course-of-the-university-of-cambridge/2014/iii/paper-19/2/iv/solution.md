<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $E=\{\alpha<\kappa:\operatorname{cf}(\alpha)=\omega\}$. This [set](../../../../../../set-split.md) is stationary: in any [club set](../../../../../../club-set.md), choose a strictly increasing countable sequence and take its supremum, which lies in the [club set](../../../../../../club-set.md) and has [cofinality](../../../../../../cofinality.md) $\omega$. For each $\alpha\in E$ choose an increasing cofinal sequence $c_\alpha:\omega\to\alpha$.

Fix $\beta<\kappa$. For every $\alpha\in E$ above $\beta$, some $c_\alpha(n)$ exceeds $\beta$. Partition this stationary tail by the least such $n$. A countable union of nonstationary [sets](../../../../../../set-split.md) is nonstationary, because fewer than $\kappa$ [club sets](../../../../../../club-set.md) have [club filter completeness](../../../../../../club-filter-completeness.md), so some cell is stationary. On it the [regressive function](../../../../../../regressive-function.md) $\alpha\mapsto c_\alpha(n)$ has, by [Fodor lemma](../../../../../../fodor-lemma.md), a stationary fiber at a value $\gamma>\beta$.

Let $I_n=\{\gamma<\kappa:\{\alpha\in E:c_\alpha(n)=\gamma\}\text{ is stationary}\}$. The preceding argument says $\bigcup_n I_n$ is unbounded in $\kappa$. Since $\operatorname{cf}(\kappa)>\omega$, at least one $I_n$ is unbounded and therefore has size $\kappa$. Its fibers are pairwise disjoint [stationary sets](../../../../../../stationary-set.md). Enumerate $\kappa$ of them as $T_\xi$, $\xi<\kappa$, and define $S_\xi=T_\xi$ for $\xi>0$, while

$$
S_0=T_0\cup\left(\kappa\setminus\bigcup_{\xi<\kappa}T_\xi\right).
$$

Adding a remainder preserves stationarity and introduces no overlap. Consequently

$$
\boxed{\kappa=\bigsqcup_{\xi<\kappa}S_\xi,\qquad S_\xi\text{ stationary for every }\xi.}
$$

This proves the [stationary partition by cofinal-sequence fibers](../../../../../../stationary-partition-by-cofinal-sequence-fibers.md) directly for every regular uncountable $\kappa$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
