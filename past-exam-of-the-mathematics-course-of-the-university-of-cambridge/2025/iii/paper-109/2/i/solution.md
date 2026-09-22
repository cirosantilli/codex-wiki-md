<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) says that if $n\geq2r$ and $\mathcal A\subseteq[n]^{(r)}$ is an [intersecting family](../../../../../../intersecting-family.md), then

$$
|\mathcal A|\leq\binom{n-1}{r-1}.
$$

The star of all $r$-sets containing one fixed point attains equality.

For the shadow proof, let $\nabla_{n-r}\mathcal A$ be the iterated upper shadow at level $n-r$, and let

$$
\mathcal A^c=\{[n]\setminus A:A\in\mathcal A\}.
$$

These two families are disjoint: if $A\subseteq[n]\setminus B$, then $A$ and $B$ are disjoint. The upper-shadow form of the [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md) says that if

$$
|\mathcal A|>\binom{n-1}{r-1},
$$

then

$$
|\nabla_{n-r}\mathcal A|>\binom{n-1}{r}.
$$

But $|\mathcal A^c|=|\mathcal A|$, so disjointness and [Pascal's identity](../../../../../../pascal-s-rule.md) would give more than

$$
\binom{n-1}{r}+\binom{n-1}{r-1}=\binom nr
$$

members at level $n-r$, a contradiction.

For the [Katona circle method](../../../../../../katona-circle-method.md), place $[n]$ in a cyclic order. At most $r$ of its cyclic intervals of length $r$ can belong to an intersecting family. Indeed, after fixing one selected interval, every selected interval starts at one of the $2r-1$ positions at cyclic distance below $r$ from its start; apart from the fixed interval, these positions form $r-1$ pairs whose corresponding intervals are disjoint. Double-count pairs consisting of $A\in\mathcal A$ and a cyclic order in which $A$ is consecutive. There are $(n-1)!$ cyclic orders, at most $r$ selected intervals in each, and each $A$ is consecutive in $r!(n-r)!$ cyclic orders. Therefore

$$
|\mathcal A|r!(n-r)!\leq r(n-1)!,
$$

which rearranges to the required bound.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
