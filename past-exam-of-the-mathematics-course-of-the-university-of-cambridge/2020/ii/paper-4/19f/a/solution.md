<h1 id="19f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Burnside lemma](../../../../../../burnside-s-lemma.md) says that the number of orbits of a finite group $G$ on a finite set $X$ is

$$
|X/G|=\frac1{|G|}\sum_{g\in G}|X^g|.
$$

Indeed, double-count the set $\{(g,x):gx=x\}$. Counting first by $g$ gives the numerator. Counting first by $x$ gives $\sum_x|G_x|$; each orbit $O$ contributes $|O||G_x|=|G|$ by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md), proving the formula.

Let $\pi(g)=|X^g|$ be the character of the [permutation representation](../../../../../../permutation-representation.md). Then

$$
\langle\pi,\pi\rangle
=\frac1{|G|}\sum_g|X^g|^2
$$

is, by Burnside's lemma, the number of orbits on $X\times X$. A [two-transitive group action](../../../../../../two-transitive-group-action.md) has exactly two such orbits: the diagonal and the ordered pairs of distinct points. Hence $\langle\pi,\pi\rangle=2$. Transitivity also gives $\langle\pi,1_G\rangle=1$. If $\pi=1_G+\sum m_i\chi_i$ is its [irreducible character decomposition](../../../../../../irreducible-character.md), then $2=1+\sum m_i^2$, so exactly one nontrivial irreducible character occurs, with multiplicity one. Thus the permutation character has precisely two distinct irreducible summands.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19F](../../19f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
