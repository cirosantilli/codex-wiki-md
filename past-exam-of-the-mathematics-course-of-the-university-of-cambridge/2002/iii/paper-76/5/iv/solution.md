<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

There is an argument-order defect in the printed flip context: the discriminator constructed above takes its numeral first. Fix $U\in\mathcal U,V\in\mathcal V$ and use

$$
F=\lambda x.D(Gx)UV.
$$

Equivalently, define $E=\lambda u v n.Dnuv$ and write the context as $\lambda x.EUV(Gx)$. This is an explicit permutation of the discriminator arguments, not an assumption that $DUV(Gx)$ has the required behavior.

Let $Q\equiv_\beta Fd(Q)$ be the [self-quoting fixed point](../../../../../../self-quoting-fixed-point.md). There are exactly two cases. If $Gd(Q)\equiv_\beta c_0$, then $Q\equiv_\beta U$, so closure under [beta equivalence](../../../../../../beta-equivalence.md) puts $Q$ in $\mathcal U$ and forces $Gd(Q)\equiv_\beta c_1$. If $Gd(Q)\equiv_\beta c_1$, then $Q\equiv_\beta V\in\mathcal V$, forcing $Gd(Q)\equiv_\beta c_0$. Both contradict the distinct beta-normal [Church numerals](../../../../../../church-numeral.md) $c_0,c_1$. Hence **no such total binary lambda classifier exists**.

If [beta equivalence](../../../../../../beta-equivalence.md) were decidable, its decision algorithm would give a total computable function that outputs one exactly on codes of terms beta-equivalent to $I$, and zero on all other codes. Its numeral representation would be such a $G$, taking $\mathcal U$ to be the class of $I$ and $\mathcal V$ its complement. Both are nonempty: $K$ has a different [beta-normal form](../../../../../../beta-normal-form.md) from $I$. The contradiction proves **beta equality is undecidable**. It is nevertheless [semidecidable](../../../../../../recursively-enumerable-set.md), since finite conversion proofs can be effectively enumerated.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
