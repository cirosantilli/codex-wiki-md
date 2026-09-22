# Hausdorff measure

↑ **Parent:** [Geometric measure theory](geometric-measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_measure)

Hausdorff measure measures the geometric size of a [set](set-split.md) using [covers](cover-topology.md) by increasingly small pieces. The exponent $s$ chooses the measuring scale: $s=1$ is length-like, $s=2$ is area-like, and noninteger exponents can measure [fractals](fractal.md). Unlike a count of occupied grid cells, the construction allows pieces of different sizes and considers every admissible [cover](cover-topology.md).

For $s>0$ and a [subset](subset.md) $E$ of a [metric space](metric-space.md), use the diameter-cost convention

$$
\mathcal H_\delta^s(E)=\inf\left\{
\sum_{j=1}^\infty(\operatorname{diam}U_j)^s:
E\subseteq\bigcup_jU_j,\quad\operatorname{diam}U_j\leq\delta
\right\},\qquad
\mathcal H^s(E)=\lim_{\delta\downarrow0}\mathcal H_\delta^s(E).
$$

The first quantity is [scale-restricted Hausdorff content](scale-restricted-hausdorff-content.md). Shrinking $\delta$ removes options from the [infimum](infimum.md), so these contents increase to a [limit](limit-of-a-function.md), possibly infinite. The resulting [outer measure](outer-measure.md) restricts to a [measure](measure.md) on the [Borel sets](borel-set.md). For $s=0$, counting each nonempty covering piece with cost one gives [counting measure](counting-measure.md).

A different common convention multiplies these quantities by $c_s=\pi^{s/2}/(2^s\Gamma(1+s/2))$, using the [Gamma function](gamma-function.md). At integer $s$, that normalization agrees with ordinary Euclidean $s$-dimensional volume. Here $c_1=1$, so both conventions make $\mathcal H^1$ agree with [arc length](arc-length.md) on [smooth curves](smooth-curve.md) in [Euclidean space](euclidean-norm.md). Positive normalization constants never change [Hausdorff dimension](hausdorff-dimension.md). A definition must specify this constant when numerical values of [Hausdorff measure](hausdorff-measure.md) matter.

For a line segment of [length](length.md) $L$, splitting it into $n$ equal pieces gives the [cover](cover-topology.md) cost

$$
n(L/n)^s=L^s n^{1-s}.
$$

It tends to zero for $s>1$, stays at $L$ for $s=1$, and grows for $s<1$. The matching lower bound comes from the fact that any interval [cover](cover-topology.md) must have total [length](length.md) at least $L$. The exponent one is therefore the transition between a measuring rule too coarse to see the segment and one that assigns it infinite size. For a [Cantor set](cantor-set.md), the transition is instead at $\log2/\log3$, as shown in [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md).

This makes [Hausdorff measure](hausdorff-measure.md) useful when ordinary [Lebesgue measure](lebesgue-measure.md) sees too little: a [curve](curve.md) in the plane has zero planar area but can have positive [arc length](arc-length.md), and the [Cantor set](cantor-set.md) has zero line [length](length.md) but positive geometric size at its own dimension. It also separates local covering estimates from global cardinality: a [countable](countable-set.md) dense [set](set-split.md) has zero [Hausdorff dimension](hausdorff-dimension.md), despite meeting every open region of its closure.

An original source for the construction is Felix Hausdorff's [Dimension und äußeres Maß, Mathematische Annalen 79, pp. 157–179](https://link.springer.com/article/10.1007/BF01457179). The modern covering and [Hausdorff dimension](hausdorff-dimension.md) framework is developed in [Bishop and Peres, Fractals in Probability and Analysis, §1.2](https://www.math.stonybrook.edu/~bishop/fractalbook.pdf).

**Table of contents**

- [Scale-restricted Hausdorff content](scale-restricted-hausdorff-content.md)
- [Hausdorff dimension](hausdorff-dimension.md)
  - [Mass distribution principle](mass-distribution-principle.md)
  - [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md)
  - [Pressure upper bound for Hausdorff dimension](pressure-upper-bound-for-hausdorff-dimension.md)
  - [Hausdorff dimension of a connected set](hausdorff-dimension-of-a-connected-set.md)

## ↑ Ancestors (7)

1. [Geometric measure theory](geometric-measure-theory.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Approximate discontinuity set](approximate-discontinuity-set.md)
- [BV trace on a hypersurface](bv-trace-on-a-hypersurface.md)
- [Cover (topology)](cover-topology.md)
- [Geometric measure theory](geometric-measure-theory.md)
- [Hausdorff dimension](hausdorff-dimension.md)
- [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md)
- [Hausdorff measure](hausdorff-measure.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/4/b/solution.md)
- [Perimeter](perimeter.md)
- [Perimeter quasiminimizer](perimeter-quasiminimizer.md)
- [Pressure upper bound for Hausdorff dimension](pressure-upper-bound-for-hausdorff-dimension.md)
- [Scale-restricted Hausdorff content](scale-restricted-hausdorff-content.md)
