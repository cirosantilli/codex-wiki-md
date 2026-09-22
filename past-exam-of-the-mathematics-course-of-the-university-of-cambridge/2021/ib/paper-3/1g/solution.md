<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Let $G$ act by left multiplication on the set $G/H$ of $n$ left [cosets](../../../../../coset.md). This gives a [group action](../../../../../group-action.md) homomorphism

$$
\varphi:G\longrightarrow S_n.
$$

Its kernel

$$
K=\bigcap_{g\in G}gHg^{-1}
$$

is a [normal subgroup](../../../../../normal-subgroup.md) of $G$, and the [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) gives $G/K\cong\operatorname{im}\varphi$. By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), $|G/K|$ divides $n!$. The image acts transitively on the $n$ cosets, so the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) shows that $n$ divides $|G/K|$; in particular,

$$
|G/K|\geq n.
$$

Now suppose $G$ is nonabelian and [simple](../../../../../simple-group.md). Since $H$ is proper, the coset action is nontrivial, so $K\ne G$. Simplicity gives $K=\{e\}$, and $\varphi$ embeds $G$ into $S_n$. Composing with the [sign homomorphism](../../../../../sign-homomorphism.md) gives

$$
G\longrightarrow S_n\longrightarrow\{\pm1\}.
$$

Its kernel is normal. A nontrivial map would embed the simple group $G$ into the abelian group of order two, which is impossible because $G$ is nonabelian. The sign is therefore always $+1$, so

$$
\boxed{G\cong\varphi(G)\leq A_n}.
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
