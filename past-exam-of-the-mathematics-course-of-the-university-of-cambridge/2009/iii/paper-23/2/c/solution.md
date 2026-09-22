<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $!_A:A\to1$ be the unique arrow to the [terminal object](../../../../../../terminal-object.md) of $\mathcal C$. Define

$$
\widehat F(A)=(FA\xrightarrow{F!_A}F1),\qquad \widehat F(f)=Ff.
$$

This is a [functor](../../../../../../functor.md) into the [slice category](../../../../../../slice-category.md) $\mathcal D/F1$, because $!_Bf=!_A$, and $U_{F1}\widehat F=F$. The [terminal object](../../../../../../terminal-object.md) of this slice is $1_{F1}:F1\to F1$, exactly $\widehat F(1)$, so $\widehat F$ preserves the [terminal object](../../../../../../terminal-object.md).

The composite $U_{F1}\widehat F$ preserves [pullbacks](../../../../../../pullback-category-theory.md) by hypothesis, and $U_{F1}$ reflects [pullbacks](../../../../../../pullback-category-theory.md) by part (b). Part (a), restricted to the [pullback](../../../../../../pullback-category-theory.md) shape, therefore shows that $\widehat F$ preserves [pullbacks](../../../../../../pullback-category-theory.md). The allowed finite-limit criterion now gives that $\widehat F$ preserves all finite [categorical limits](../../../../../../categorical-limit.md), and hence [equalisers](../../../../../../equaliser.md). Since $U_{F1}$ preserves [equalisers](../../../../../../equaliser.md), their composite does too. Thus

$$
\boxed{F\text{ preserves equalisers.}}
$$

This is [equalizer preservation by pullback-preserving functors](../../../../../../equalizer-preservation-by-pullback-preserving-functors.md). The factorization supplies terminal-object preservation only in the slice; none is asserted for the original $F$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
