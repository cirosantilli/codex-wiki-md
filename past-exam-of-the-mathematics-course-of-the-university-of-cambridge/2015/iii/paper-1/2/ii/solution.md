<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the convention that a [multiplicative subset](../../../../../../multiplicatively-closed-set.md) contains $1$ and is closed under multiplication. Usually $0$ is excluded; allowing it gives the harmless zero-ring localization. A [prime ideal](../../../../../../prime-ideal.md) disjoint from $S$ is mapped to

$$
S^{-1}P=\{a/s:a\in P,\ s\in S\}
$$

in the [localization of a ring](../../../../../../localization-of-a-ring.md). This [ideal](../../../../../../ideal.md) is proper, and

$$
(S^{-1}R)/(S^{-1}P)\cong S^{-1}(R/P)
$$

is an [integral domain](../../../../../../integral-domain.md), since the denominators are nonzero in the [integral domain](../../../../../../integral-domain.md) $R/P$. Thus $S^{-1}P$ is a [prime ideal](../../../../../../prime-ideal.md).

Conversely, for a [prime ideal](../../../../../../prime-ideal.md) $Q$ in $S^{-1}R$, its contraction

$$
P=\{a\in R:a/1\in Q\}
$$

is a [prime ideal](../../../../../../prime-ideal.md) disjoint from $S$: each $s/1$ is a unit and cannot belong to a proper [ideal](../../../../../../ideal.md). Membership in $Q$ is equivalent to numerator membership in $P$, since $a/s=(a/1)(s/1)^{-1}$. Hence $Q=S^{-1}P$.

To check the other composite, $a/1\in S^{-1}P$ implies $sa\in P$ for some $s\in S$, by the equality criterion for fractions in a [localization of a ring](../../../../../../localization-of-a-ring.md). Since $s\notin P$, primality gives $a\in P$. Therefore **extension and contraction are mutually inverse:**

$$
\boxed{\{P\in\operatorname{Spec}R:P\cap S=\varnothing\}
\ \longleftrightarrow\ \operatorname{Spec}(S^{-1}R),\qquad P\mapsto S^{-1}P.}
$$

If $0\in S$, both sets are empty. This is the [prime ideal correspondence for localization](../../../../../../prime-ideal-correspondence-for-localization.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
