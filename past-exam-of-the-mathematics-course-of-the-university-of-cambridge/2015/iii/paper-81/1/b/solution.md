<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Make a [bipartite spin rotation](../../../../../../bipartite-spin-rotation.md): rotate every odd site's [spin](../../../../../../spin.md) through $\pi$ about the $x$ axis, using $U=\prod_{n\ \mathrm{odd}}e^{-i\pi S_n^x}$. This [unitary conjugation](../../../../../../unitary-conjugation.md) preserves the [spin commutation relations](../../../../../../spin-commutation-relations.md). At an odd site it sends $(S^x,S^y,S^z)$ to $(S^x,-S^y,-S^z)$ and exchanges the [spin raising operator](../../../../../../spin-raising-operator.md) and [spin lowering operator](../../../../../../spin-lowering-operator.md).

Each bond joins one rotated and one unrotated site. In the transformed operators,

$$
\mathbf S_n\cdot\mathbf S_{n+1}\longmapsto S_n^xS_{n+1}^x-S_n^yS_{n+1}^y-S_n^zS_{n+1}^z=-S_n^zS_{n+1}^z+\frac12(S_n^+S_{n+1}^++S_n^-S_{n+1}^-).
$$

Thus

$$
\boxed{H=-J\sum_n\left[S_n^zS_{n+1}^z-\frac12(S_n^+S_{n+1}^++S_n^-S_{n+1}^-)\right]}.
$$

The selected [Néel state](../../../../../../neel-state.md) becomes an all-up reference state, so a single [Holstein–Primakoff transformation](../../../../../../holstein-primakoff-transformation.md) convention works on both sublattices.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
