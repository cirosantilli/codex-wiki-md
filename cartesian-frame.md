# Cartesian frame

↑ **Parent:** [Cartesian basis](cartesian-basis.md)

A [Cartesian frame](cartesian-frame.md) combines a chosen origin [point](point-geometry.md) $O$ with a [Cartesian basis](cartesian-basis.md) $\mathcal E$, including its ordering as an [ordered basis](ordered-basis.md). A [point](point-geometry.md) $P$ has [coordinate vector](coordinate-vector.md) $c$ when $\overrightarrow{OP}=\sum_i c_i e_i$. The [basis](basis.md) supplies measuring directions and unit lengths; the [coordinate vector](coordinate-vector.md) is the resulting [tuple](finite-tuple.md) of numbers; the [Cartesian frame](cartesian-frame.md) additionally fixes where measurement starts. A [vector](vector.md) already belongs to a [vector space](vector-space-split.md) with a [zero vector](zero-vector.md), so expressing it in a [basis](basis.md) requires no additional choice of spatial origin.

For example, keeping the [standard basis](standard-basis.md) but moving the origin from $O=(0,0)$ to $O'=(1,0)$ changes the [coordinates](coordinate-linear-algebra.md) of the physical [point](point-geometry.md) $P=(2,1)$ from $(2,1)^T$ to $(1,1)^T$. This happens because $\overrightarrow{O'P}=\overrightarrow{OP}-\overrightarrow{OO'}$ is a different displacement [vector](vector.md). By contrast, the two diagrams above keep $O$ fixed and change only the [basis](basis.md). In a fixed reference [Cartesian frame](cartesian-frame.md), a new frame with origin column $o$ and basis-column [matrix](matrix.md) $Q$ describes [points](point-geometry.md) by $p=o+Qc$; the new [coordinates](coordinate-linear-algebra.md) are $c=Q^T(p-o)$ when $Q$ is an [orthogonal matrix](orthogonal-matrix.md).

## ↑ Ancestors (6)

1. [Cartesian basis](cartesian-basis.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cartesian frame](cartesian-frame.md)
