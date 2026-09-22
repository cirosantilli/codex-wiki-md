<h1 id="19g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is a missing hypothesis in the printed equivalence. A group acting trivially on a two-point set has a one-dimensional zero-sum subspace $S$, hence an irreducible trivial [representation](../../../../../../group-representation.md), but its action is not doubly transitive. Thus **the assertion as written is false**. The intended result holds for a transitive action; more generally the trivial two-point action is the only exceptional case under $|X|>1$.

For the intended proof, decompose $\mathbb C[X]=\mathbf1\oplus S$ by separating constant functions from functions with zero sum. If the action is transitive, $\langle\mathbf1,\chi_X\rangle=1$. Hence

$$
\|\chi_S\|^2=\|\chi_X-\mathbf1\|^2=\|\chi_X\|^2-1.
$$

Over the complex numbers, complete reducibility and [character orthogonality](../../../../../../character-orthogonality.md) identify this norm as the sum of squared irreducible multiplicities; it is one precisely when $S$ is irreducible. By part (i), $\|\chi_X\|^2$ counts orbits on $X\times X$. Transitivity gives one diagonal orbit, and the norm equals two exactly when all off-diagonal ordered pairs form one orbit, which is double transitivity. This proves both implications with the missing transitivity condition restored.

To check the exact exception, if the action has $r>1$ orbits, then $S$ contains an invariant subspace of [dimension](../../../../../../dimension-vector-space.md) $r-1$, from orbitwise constant functions with total sum zero. If $S$ is irreducible this makes $S$ the one-dimensional trivial [representation](../../../../../../group-representation.md), so $|X|-1=1$ and $|X|=2$. Nontransitivity on two points means both are fixed. Therefore **irreducibility is equivalent to double transitivity, except for the trivial two-point action**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19G](../../19g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
