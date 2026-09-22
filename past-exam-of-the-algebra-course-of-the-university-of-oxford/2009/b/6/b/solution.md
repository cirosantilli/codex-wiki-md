<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [Abelian group](../../../../../abelian-group.md) has the central series $1<G$, since $Z(G)=G$. In any central series, each factor is a subgroup of a center and hence [Abelian](../../../../../abelian-group.md). A finite normal series with [Abelian](../../../../../abelian-group.md) factors makes the group [soluble](../../../../../solvable-group.md): inductively, if $N$ is soluble and $G/N$ is [Abelian](../../../../../abelian-group.md), then $G'\subseteq N$, and successive derived groups eventually vanish. Hence **every nilpotent group is soluble**.

The group $S_3$ has the normal series $1<A_3<S_3$ with cyclic factors of orders three and two, so it is soluble. Its center is trivial, since a permutation commuting with both $(12)$ and $(23)$ must fix all three letters. Every nontrivial nilpotent group has nontrivial center: its first nonidentity central-series term is contained in $Z(G)$. Consequently **$S_3$ is soluble but not nilpotent**.

For a finite [p-group](../../../../../p-group.md), use induction on its order. The identity group is the base case. A nontrivial $G$ has nontrivial $Z=Z(G)$, so $G/Z$ has smaller order, still a power of $p$. By induction it has a central series. Lift that series to subgroups of $G$ and prepend $1<Z$. The first factor is central by definition of $Z$, and centrality of every lifted factor is exactly centrality of the corresponding quotient factor. This gives a central series for $G$. This proves [finite p-groups are nilpotent](../../../../../finite-p-groups-are-nilpotent.md):

$$
\boxed{\text{Every finite p-group is nilpotent}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
