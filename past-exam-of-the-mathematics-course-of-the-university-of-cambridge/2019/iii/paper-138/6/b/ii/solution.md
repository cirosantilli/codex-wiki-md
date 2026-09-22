<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $N=N_G(D)$. For an algebra on which a group acts by conjugation, write

$$
A_D^H=\operatorname{Tr}_D^H(A^D),
\qquad
\operatorname{Tr}_D^H(a)=\sum_{h\in H/D}hah^{-1},
$$

for its [transfer ideal of conjugation-fixed elements](../../../../../../../transfer-ideal-of-conjugation-fixed-elements.md). In the diagram, $\tau=\operatorname{Tr}_D^G$, $\tau'=\operatorname{Tr}_D^N$, the upper map is $\beta=\operatorname{Br}_D$, and $\beta'$ is the restriction of $\operatorname{Br}_D$ from $(kG)^G$ to $(kG)_D^G$. Since $N$ normalizes both $D$ and $C_G(D)$, the lower map lands in $(kC_G(D))_D^N$.

For $a\in(kG)^D$, let $D$ act on the left cosets $G/D$. A coset $gD$ is fixed precisely when $g^{-1}Dg\leq D$, hence, because the two groups have the same order, precisely when $g\in N$. Every nonfixed orbit has size divisible by $p$. Moreover, after applying $\operatorname{Br}_D$, all summands indexed by one $D$-orbit are equal: conjugation by an element of $D$ acts trivially on $kC_G(D)$. Those orbits therefore contribute zero in characteristic $p$, while the fixed cosets contribute the trace over $N/D$. Consequently

$$
\beta'\tau(a)
=\operatorname{Br}_D\!\left(\operatorname{Tr}_D^G(a)\right)
=\operatorname{Tr}_D^N\!\left(\operatorname{Br}_D(a)\right)
=\tau'\beta(a).
$$

This is the [Brauer morphism and relative trace](../../../../../../../brauer-morphism-and-relative-trace.md) identity, so **the diagram commutes**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 138](../../../../paper-138-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
