<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the usual no-linkage reference model with unrelated, noninbred parents, define $J$ as the number of homologous [allele](../../../../../../allele.md) copies shared [identical by descent](../../../../../../identity-by-descent.md) by two [full siblings](../../../../../../full-sibling.md) at the marker. The two siblings receive the same paternal copy with [probability](../../../../../../probability.md) $1/2$, and independently receive the same maternal copy with [probability](../../../../../../probability.md) $1/2$. Therefore [Mendelian IBD sharing of full siblings](../../../../../../mendelian-ibd-sharing-of-full-siblings.md) gives

$$
P(J=0)=\frac14,\quad P(J=1)=\frac12,\quad P(J=2)=\frac14,\qquad J\sim\operatorname{Bin}(2,1/2).
$$

Hence

$$
\boxed{E[J]=1,\qquad \operatorname{Var}(J)=\frac12.}
$$

For affected siblings, absence of [genetic linkage](../../../../../../genetic-linkage.md) makes the marker transmissions independent of selection by disease, so these are the relevant null moments. This is a fresh outbred reference calculation, not an application of these sharing probabilities to the inbred siblings $E,F$ in part (b). Without the outbred-parent assumption the three ordinary sharing probabilities require modification.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
