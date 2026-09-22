<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [soluble group](../../../../../solvable-group.md), also called a [solvable group](../../../../../solvable-group.md), has a terminating [derived series](../../../../../derived-series.md):

$$
G^{(0)}=G,\qquad G^{(j+1)}=[G^{(j)},G^{(j)}],\qquad G^{(r)}=1\text{ for some }r\geq0.
$$

For a [subgroup](../../../../../subgroup.md) $S\leq G$, induction gives $S^{(j)}\leq G^{(j)}$, so subgroups of [soluble groups](../../../../../solvable-group.md) are soluble. For a surjective [group homomorphism](../../../../../group-homomorphism.md) $q:G\to Q$, $q(G^{(j)})=Q^{(j)}$, so quotients of [soluble groups](../../../../../solvable-group.md) are soluble. Finally, in a [group extension](../../../../../group-extension.md) $1\to K\to E\to Q\to1$, suppose $K^{(r)}=1$ and $Q^{(s)}=1$. Then $E^{(s)}\leq K$ and $E^{(s+r)}=1$. **[Soluble groups](../../../../../solvable-group.md) are closed under [subgroups](../../../../../subgroup.md), quotients and [group extensions](../../../../../group-extension.md).**

A [virtually soluble group](../../../../../virtually-solvable-group.md) contains a [soluble group](../../../../../solvable-group.md) as a [finite-index subgroup](../../../../../finite-index-subgroup.md). The finite-index facts proved in parts (i)–(iii) imply closure under [subgroups](../../../../../subgroup.md) and quotients: intersect a finite-index soluble subgroup with the chosen subgroup, or take its image under the quotient map.

For [group extensions](../../../../../group-extension.md), no finite-generation hypothesis may be inserted. We first establish the [finite-index characteristic soluble subgroup](../../../../../finite-index-characteristic-soluble-subgroup.md) lemma. If $K$ is a [virtually soluble group](../../../../../virtually-solvable-group.md), the kernel of its action on the cosets of a finite-index soluble subgroup is a soluble [normal subgroup](../../../../../normal-subgroup.md) $K_0$ of finite index. Among soluble [normal subgroups](../../../../../normal-subgroup.md) containing $K_0$, choose $R$ with maximal $|R/K_0|$, possible because $K/K_0$ is finite. If $S$ is any soluble [normal subgroup](../../../../../normal-subgroup.md) of $K$, then $RS$ is soluble: it is an extension of $R$ by $S/(R\cap S)$. Maximality forces $S\leq R$. Thus $R$ is the unique largest soluble [normal subgroup](../../../../../normal-subgroup.md) of $K$, making it a [characteristic subgroup](../../../../../characteristic-subgroup.md), and it has finite index.

Now suppose $1\to K\to G\overset{\pi}{\to}Q\to1$ has both $K$ and $Q$ virtually soluble. Replace $G$ by the preimage $G_0$ of a finite-index soluble subgroup of $Q$. The subgroup $R$ just constructed is characteristic in $K$ and therefore normal in $G_0$. In $E=G_0/R$, the subgroup $A=K/R$ is a finite [normal subgroup](../../../../../normal-subgroup.md), and $E/A$ is a [soluble group](../../../../../solvable-group.md). The [centralizer](../../../../../centralizer.md) $C_E(A)$ has finite index in $E$, since conjugation gives a map $E\to\operatorname{Aut}(A)$ with finite image. Its intersection with $A$ is the [center of a group](../../../../../center-of-a-group.md) $Z(A)$, an [abelian group](../../../../../abelian-group.md), while its quotient by $Z(A)$ embeds in the soluble group $E/A$. Thus $C_E(A)$ is a [soluble group](../../../../../solvable-group.md). Its preimage in $G_0$ is an extension by $R$, so it too is soluble and has finite index in $G$. **[Virtually soluble groups](../../../../../virtually-solvable-group.md) are closed under [group extensions](../../../../../group-extension.md).**

For the final example take the [restricted direct sum of groups](../../../../../restricted-direct-sum-of-groups.md)

$$
\boxed{D=\bigoplus_{j\geq1}A_5,}
$$

where $A_5$ is the nonabelian [simple group](../../../../../simple-group.md) of even permutations on five letters. Every finite collection of elements lies in a product of finitely many finite factors, so $D$ is a [locally finite group](../../../../../locally-finite-group.md) and hence a [torsion group](../../../../../torsion-group.md). It cannot contain a nonabelian [free group](../../../../../free-group.md), which is a [torsion-free group](../../../../../torsion-free-group.md).

To show that $D$ is not a [virtually soluble group](../../../../../virtually-solvable-group.md), let $H$ be any [finite-index subgroup](../../../../../finite-index-subgroup.md) and let $N\leq H$ be the kernel of the finite coset action. Each coordinate $A_5$ maps either injectively or trivially into the finite quotient $D/N$, by [Simplicity of the alternating group A5](../../../../../simplicity-of-the-alternating-group-a5.md). The nontrivial images of distinct factors commute, and each has trivial centre, so any $k$ of them generate a [direct product of groups](../../../../../direct-product-of-groups.md) of order $60^k$. Only finitely many such images can occur in a finite quotient. Therefore $N$, and hence $H$, contains a whole coordinate copy of $A_5$, which is not soluble: its nontrivial [commutator subgroup](../../../../../commutator-subgroup.md) is normal and therefore equals $A_5$. **No finite-index subgroup of $D$ is soluble.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
