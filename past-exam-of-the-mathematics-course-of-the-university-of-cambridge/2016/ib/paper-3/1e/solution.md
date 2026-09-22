<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

A [permutation representation](../../../../../permutation-representation.md) is a [group homomorphism](../../../../../group-homomorphism.md) $\rho:G\to\operatorname{Sym}(\Omega)$, equivalently a [group action](../../../../../group-action.md) on a set $\Omega$. The [left regular action](../../../../../left-regular-action.md) takes $\Omega=G$ and $\rho(g)(h)=gh$. Each such map is a [bijection](../../../../../bijection.md), and $\rho(g_1g_2)=\rho(g_1)\rho(g_2)$. If $\rho(g)$ is the identity, evaluating at the identity element gives $g=1$. Thus the representation is faithful. Numbering the elements of $G$ identifies $\operatorname{Sym}(G)$ with the [symmetric group](../../../../../symmetric-group.md) $S_n$, proving [Cayley theorem](../../../../../cayley-s-theorem.md):

$$
\boxed{G\cong\rho(G)\leq S_n.}
$$

For a nonabelian [simple group](../../../../../simple-group.md), compose this faithful representation with the [sign of a permutation](../../../../../sign-of-a-permutation.md) homomorphism $S_n\to\{1,-1\}$. Its [kernel](../../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../../normal-subgroup.md) of $G$, hence either trivial or all of $G$. A trivial kernel would embed $G$ in a group of order two, contradicting noncommutativity. Therefore every represented element is even, and **the same representation embeds $G$ in the [alternating group](../../../../../alternating-group.md) $A_n$**.

Finally let $S_3$ act on the two [cosets](../../../../../coset.md) of its [normal subgroup](../../../../../normal-subgroup.md) $A_3$. An even permutation fixes both cosets, whereas an odd permutation exchanges them. This gives $S_3\to S_2$ with **kernel $A_3$**; explicitly, send even permutations to the identity and odd permutations to $(12)$.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
