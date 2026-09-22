<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppose $F\cong\operatorname*{colim}_{j\in J}R_j$, where $J$ is a [filtered category](../../../../../../filtered-category.md) and every $R_j$ is a [representable functor](../../../../../../representable-functor.md). Every covariant [representable functor](../../../../../../representable-functor.md) $\mathcal C(A,-)$ preserves all existing [categorical limits](../../../../../../categorical-limit.md): maps from $A$ into a limiting object are exactly compatible families of maps into its diagram.

For a finite [diagram in a category](../../../../../../diagram-category-theory.md) $K:I\to\mathcal C$, use pointwise [colimits](../../../../../../colimit.md) in the [functor category](../../../../../../functor-category.md), preservation by each $R_j$, and the permitted result that [filtered colimits commute with finite limits in sets](../../../../../../filtered-colimits-commute-with-finite-limits-in-sets.md) to obtain

$$
\begin{aligned}
F(\lim_iK_i)
&\cong\operatorname*{colim}_jR_j(\lim_iK_i)\\
&\cong\operatorname*{colim}_j\lim_iR_j(K_i)\\
&\cong\lim_i\operatorname*{colim}_jR_j(K_i)
\cong\lim_i F(K_i).
\end{aligned}
$$

The isomorphism is the canonical comparison, since every step respects the limiting projections. This also covers the empty finite diagram and hence the [terminal object](../../../../../../terminal-object.md). Thus **$(iv)\Rightarrow(i)$**, completing the cycle:

$$
\boxed{(i)\Longleftrightarrow(ii)\Longleftrightarrow(iii)\Longleftrightarrow(iv).}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
