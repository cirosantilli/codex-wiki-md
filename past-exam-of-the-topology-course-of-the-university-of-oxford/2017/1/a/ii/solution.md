<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $K$ is [compact](../../../../../compact-space.md), and let the [closed subsets](../../../../../closed-set.md) $F_i$ of $K$ have the [finite intersection property](../../../../../finite-intersection-property.md). If their total [intersection](../../../../../set-intersection.md) were empty, their [complements](../../../../../complement-of-a-set.md) $K\setminus F_i$ would form an [open cover](../../../../../open-cover.md) of $K$. A [finite subcover](../../../../../finite-subcover.md) would give

$$
K=\bigcup_{j=1}^m(K\setminus F_{i_j})
\quad\Longrightarrow\quad
\bigcap_{j=1}^mF_{i_j}=\varnothing,
$$

contradicting the [finite intersection property](../../../../../finite-intersection-property.md). Therefore the total [intersection](../../../../../set-intersection.md) is nonempty.

Conversely, assume the stated nonempty-[intersection](../../../../../set-intersection.md) property for every family of [closed subsets](../../../../../closed-set.md) of $K$. Given an [open cover](../../../../../open-cover.md) $\{V_i:i\in I\}$ of $K$ in its [subspace topology](../../../../../subspace-topology.md), set $F_i=K\setminus V_i$. Their total [intersection](../../../../../set-intersection.md) is empty. By the contrapositive of the assumed property, this family fails the [finite intersection property](../../../../../finite-intersection-property.md); hence some finite $J\subseteq I$ satisfies

$$
\bigcap_{j\in J}F_j=\varnothing
\quad\Longrightarrow\quad
K=\bigcup_{j\in J}V_j.
$$

This is a [finite subcover](../../../../../finite-subcover.md), proving [compactness](../../../../../compact-space.md). Both directions are instances of [De Morgan's laws](../../../../../de-morgan-s-laws.md). Thus **[compactness](../../../../../compact-space.md) is equivalent to the [finite intersection characterization of compactness](../../../../../finite-intersection-characterization-of-compactness.md)**.

For completeness, the [intersection](../../../../../set-intersection.md) of the empty family of [subsets](../../../../../subset.md) of $K$ is $K$. If $K$ is empty, no family has the [finite intersection property](../../../../../finite-intersection-property.md) when the empty finite subfamily is included, so the implication remains valid.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
