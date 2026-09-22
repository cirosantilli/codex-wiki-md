<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Define $G^{(0)}=G$ and $G^{(i+1)}=[G^{(i)},G^{(i)}]$. A group is a [soluble group](../../../../solvable-group.md) if this [derived series](../../../../derived-series.md) reaches the identity after finitely many steps. Its [derived length](../../../../derived-length.md) is the least $d$ with $G^{(d)}=1$.

Let $V=\{1,(12)(34),(13)(24),(14)(23)\}\leq A_4$. This [Klein four-group](../../../../klein-four-group.md) is a [normal subgroup](../../../../normal-subgroup.md) and Abelian; $A_4/V$ has order three, so $A_4'\subseteq V$. The group $A_4$ is nonabelian, so its derived [subgroup](../../../../subgroup.md) is nontrivial. Conjugation by a three-cycle permutes the three nonidentity elements of $V$ transitively. Since the derived [subgroup](../../../../subgroup.md) is a [normal subgroup](../../../../normal-subgroup.md), containing any one forces it to contain all three. Thus $A_4'=V$, and $V'=1$. Therefore **$A_4$ has [derived length](../../../../derived-length.md) two**.

If $H\leq G$, every [commutator](../../../../commutator.md) in $H$ is one in $G$, and induction gives $H^{(i)}\subseteq G^{(i)}$ for all $i$. Thus a [subgroup](../../../../subgroup.md) of a [solvable group](../../../../solvable-group.md) is solvable, with no larger [derived length](../../../../derived-length.md).

The sign map gives $S_4'\subseteq A_4$. The [commutator](../../../../commutator.md) $[(12),(23)]$ is a three-cycle. Normality of $S_4'$ supplies every conjugate three-cycle, and three-cycles generate $A_4$. Hence $S_4'=A_4$, so the complete [derived series](../../../../derived-series.md) is

$$
\boxed{S_4\supset A_4\supset V\supset1.}
$$

Every inclusion is strict, proving solvability and [derived length](../../../../derived-length.md) three.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
