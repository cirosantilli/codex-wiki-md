<h1 id="b/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The stabilizer of an ordered pair is the subgroup $\Sigma_{n-2}$ fixing both entries, so the [permutation module](../../../../../permutation-module.md) is $\operatorname{Ind}_{\Sigma_{n-2}}^{\Sigma_n}\mathbf1$. Induce in two stages through $\Sigma_{n-1}$. The first stage is $S^{(n-1)}\oplus S^{(n-2,1)}$. The characteristic-zero [induction branching rule for a symmetric group](../../../../../induction-branching-rule-for-a-symmetric-group.md) adds one box in every possible [partition](../../../../../integer-partition.md) position, with multiplicity one. Thus the two second-stage decompositions are

$$
\operatorname{Ind}S^{(n-1)}=S^{(n)}\oplus S^{(n-1,1)},\qquad\operatorname{Ind}S^{(n-2,1)}=S^{(n-1,1)}\oplus S^{(n-2,2)}\oplus S^{(n-2,1,1)}.
$$

By transitivity of induction this yields

$$
\boxed{M^{(n-2,1,1)}\cong S^{(n)}\oplus2S^{(n-1,1)}\oplus S^{(n-2,2)}\oplus S^{(n-2,1,1)}.}
$$

The dimensions are $1$, $2(n-1)$, $n(n-3)/2$ and $(n-1)(n-2)/2$, whose sum is $n(n-1)$, checking the decomposition also at $n=4$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
