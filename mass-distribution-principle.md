# Mass distribution principle

↑ **Parent:** [Hausdorff dimension](hausdorff-dimension.md)

The mass distribution principle converts a diffuse [measure](measure-split.md) into a lower bound on [Hausdorff dimension](hausdorff-dimension.md). Let $s>0$ and let a [Borel probability measure](borel-probability-measure.md) $\mu$ give a [Borel set](borel-set.md) $E$ full mass. If, for some $C,r_0>0$, every [ball](ball-mathematics.md) centered in $E$ satisfies

$$
\mu(B(x,r))\leq Cr^s\qquad(0<r<r_0),
$$

then $\mathcal H^s(E)\geq1/C>0$ in the diameter-cost convention, and consequently $\dim_HE\geq s$.

The idea is to keep unit mass from being crowded into cheap covering pieces. For a piece $U$ of positive [diameter](diameter.md) $r$ meeting $E$, choose $x\in U\cap E$. A ball of radius $r+\varepsilon$ contains $U$; letting $\varepsilon\downarrow0$ gives $\mu^*(U)\leq Cr^s$, where $\mu^*$ is the associated [outer measure](outer-measure.md). Zero-diameter pieces have zero mass by the same estimate. For any sufficiently small [cover](cover-topology.md),

$$
1=\mu(E)\leq\sum_j\mu^*(U_j)\leq C\sum_j(\operatorname{diam}U_j)^s.
$$

Thus every cover costs at least $1/C$. This is the lower-bound counterpart to the explicit covers in [scale-restricted Hausdorff content](scale-restricted-hausdorff-content.md). The [Cantor distribution](cantor-distribution.md) supplies the needed mass in [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md). [Bishop and Peres, §1.2: the mass distribution principle](https://www.math.stonybrook.edu/~bishop/fractalbook.pdf).

## ↑ Ancestors (9)

1. [Hausdorff dimension](hausdorff-dimension.md)
2. [Hausdorff measure](hausdorff-measure.md)
3. [Geometric measure theory](geometric-measure-theory.md)
4. [Measure theory](measure-theory-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Hausdorff dimension](hausdorff-dimension.md)
- [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md)
- [Scale-restricted Hausdorff content](scale-restricted-hausdorff-content.md)
