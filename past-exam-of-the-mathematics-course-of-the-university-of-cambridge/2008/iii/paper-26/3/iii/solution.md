<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Every covariant [representable functor](../../../../../../representable-functor.md) preserves [categorical limits](../../../../../../categorical-limit.md): arrows from its representing object into a limiting object are exactly compatible cones of arrows into the diagram. Apply the density formula proved in the root solution. For any finite diagram $D:J\to\mathcal C$,

$$
F(\lim_JD)\cong\operatorname*{colim}_{e\in E^{\mathrm{op}}}\lim_{j\in J}H_e(D_j)
\cong\lim_{j\in J}\operatorname*{colim}_{e\in E^{\mathrm{op}}}H_e(D_j)
\cong\lim_J FD.
$$

The middle [isomorphism](../../../../../../isomorphism.md) uses exactly the permitted theorem that [filtered colimits](../../../../../../filtered-colimit-of-modules.md) commute with [finite limits](../../../../../../finite-limit.md) in sets; it applies because $E^{\mathrm{op}}$ is filtered. All maps are the natural comparison maps, so $F$ preserves [finite limits](../../../../../../finite-limit.md), including the [terminal object](../../../../../../terminal-object.md). This proves $\boxed{\text{(iii)}\Rightarrow\text{(i)}}$ and completes the equivalence.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
