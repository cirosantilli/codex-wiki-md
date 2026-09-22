<h1 id="19g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induct on the order of the [p-group](../../../../../../p-group.md). Every complex [irreducible representation](../../../../../../irreducible-representation.md) of an abelian group is one-dimensional: commuting group operators preserve a common eigenspace, and irreducibility makes that eigenspace the whole space. This handles the abelian cases.

If $V$ is not faithful, it is an irreducible representation of a smaller quotient $G/K$, where $K$ is its kernel. Induction expresses it as induced from a one-dimensional representation of a subgroup of $G/K$. Pulling back the subgroup and inflating the character gives the same induction statement for $G$, because the coset spaces of the quotient subgroup and its inverse image agree.

Now suppose $V$ is faithful and $G$ is nonabelian. Use the allowed abelian normal subgroup $A$ not contained in the centre. If restriction to $A$ were isotypic, its irreducible type would be one-dimensional, so every $a\in A$ would act as a scalar. It would therefore commute with every representing matrix of $G$. Faithfulness would imply $ga=ag$ in $G$ for every $g$, contradicting the choice of $A$. By part (a), $V=\operatorname{Ind}_H^GW$ for an irreducible representation of a proper subgroup $H$. Induction on $H$ gives $W=\operatorname{Ind}_K^H\chi$ with $\chi$ one-dimensional. Transitivity of induction yields

$$
\boxed{V=\operatorname{Ind}_K^G\chi.}
$$

This proves the [monomiality of irreducible representations of finite p-groups](../../../../../../monomiality-of-irreducible-representations-of-finite-p-groups.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19G](../../19g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
