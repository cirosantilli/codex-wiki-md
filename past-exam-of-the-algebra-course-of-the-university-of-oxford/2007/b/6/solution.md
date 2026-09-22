<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [composition series](../../../../composition-series.md) is a chain $1=G_0\triangleleft G_1\triangleleft\cdots\triangleleft G_r=G$ with simple nontrivial factors. Every [finite group](../../../../finite-group.md) has one, by recursively choosing a maximal proper [normal subgroup](../../../../normal-subgroup.md). The [Jordan–Hölder theorem](../../../../jordan-holder-theorem.md) states that any two such series have the same length and the same multiset of simple factors up to isomorphism.

For a proof induct on $|G|$. Let $M,N$ be the penultimate terms in two series. If $M=N$, apply induction there. Otherwise their maximal normality gives $MN=G$. Set $D=M\cap N$. The second isomorphism theorem gives

$$
M/D\cong G/N,\qquad N/D\cong G/M,
$$

so these quotients are simple. Choose a [composition series](../../../../composition-series.md) of $D$ and extend it once to $M$ and once to $N$. Induction in the smaller [groups](../../../../group-split.md) $M,N$ compares these with the respective original prefixes. Appending $G/M$ or $G/N$ gives in both cases the factors of $D$ together with $G/M,G/N$. This completes the proof, including the case $D=1$.

**Exactly one:** take $S_5$. Its only nontrivial proper [normal subgroup](../../../../normal-subgroup.md) is $A_5$. Indeed a normal $N$ has $N\cap A_5$ either $1$ or $A_5$ by the supplied simplicity. In the first case $N$ injects into $S_5/A_5\cong C_2$, so a nontrivial $N$ would be a [normal subgroup](../../../../normal-subgroup.md) of order two and hence central. But $S_5$ has trivial center: conjugating every transposition trivially forces preservation of each unordered pair, and therefore of every point. Thus the unique series is $1\triangleleft A_5\triangleleft S_5$.

**Exactly two:** take $A_5\times C_2$. A [normal subgroup](../../../../normal-subgroup.md) containing $A_5\times1$ is that subgroup or the whole product. For a [normal subgroup](../../../../normal-subgroup.md) $N$ meeting $A_5\times1$ trivially, commutators of its elements with $A_5\times1$ vanish; its first coordinates therefore lie in $Z(A_5)=1$. Hence $N\subseteq1\times C_2$. The two nontrivial proper [normal subgroups](../../../../normal-subgroup.md) are exactly the two factors, each simple, so the two series pass respectively through $A_5\times1$ and $1\times C_2$.

**More than two:** take $C_{120}$. A [cyclic group](../../../../cyclic-group.md) has exactly one subgroup of each divisor order, and composition steps have prime indices. The orders of those indices are the distinct permutations of $2,2,2,3,5$, giving

$$
\boxed{5!/3!=20\text{ composition series}.}
$$

All three example [groups](../../../../group-split.md) have order $120$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
