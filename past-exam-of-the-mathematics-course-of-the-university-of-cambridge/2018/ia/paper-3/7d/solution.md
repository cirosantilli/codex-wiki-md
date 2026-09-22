<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

For a [normal subgroup](../../../../../normal-subgroup.md) $H\trianglelefteq G$, the [quotient group](../../../../../quotient-group.md) $G/H$ is the set of cosets $gH$ with multiplication $(gH)(kH)=gkH$. If $gH=g'H$ and $kH=k'H$, normality moves the intervening elements of $H$ past $k$, proving that the product is independent of representatives.

If $g$ has finite order $m$, then $(gH)^m=H$, so $\operatorname{ord}(gH)$ divides $m$. For finite $G$, the greatest element order in $G/H$ is therefore no greater than that in $G$.

Every kernel is normal because $\varphi(ghg^{-1})=\varphi(g)\varphi(h)\varphi(g)^{-1}=1$ whenever $h\in\ker\varphi$. Conversely, if $H$ is normal, the quotient map $G\to G/H$ has kernel $H$. Thus **$H\trianglelefteq G$ exactly when it is the kernel of a group homomorphism**.

A group is [metacyclic](../../../../../metacyclic-group.md) when it has a cyclic normal subgroup with cyclic quotient. A [dihedral group](../../../../../dihedral-group.md) has its cyclic rotation subgroup normal and quotient $C_2$, so every dihedral group is metacyclic.

Up to isomorphism the groups of order eight are

$$
C_8,\quad C_4\times C_2,\quad C_2^3,\quad D_8,\quad Q_8.
$$

All except $C_2^3$ are metacyclic: use a cyclic subgroup of order four in the three noncyclic examples that have one. In $C_2^3$, every cyclic subgroup has order at most two and its quotient is not cyclic. The normal subgroups of $A_4$ are $1,V_4,A_4$; none gives the required cyclic subgroup and quotient, so $A_4$ is not metacyclic. Finally, $S_1,S_2,S_3$ are metacyclic, while $S_4$ and $S_5$ are not, by their normal-subgroup structures. Hence

$$
\boxed{S_n\text{ is metacyclic for }n\leq5\text{ exactly when }n=1,2,3.}
$$

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
