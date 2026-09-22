# Hausdorff dimension

↑ **Parent:** [Hausdorff measure](hausdorff-measure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_dimension)

The Hausdorff dimension is the critical exponent at which [Hausdorff measure](hausdorff-measure.md) changes from infinite to zero:

$$
\dim_HE=\inf\{s\geq0:\mathcal H^s(E)=0\}
=\sup\{s\geq0:\mathcal H^s(E)=\infty\},
$$

with the standard endpoint convention for an empty supremum. This measures fine-scale geometric size rather than the number of coordinates used to describe the [set](set-split.md). A line segment has [Hausdorff dimension](hausdorff-dimension.md) one; a square has dimension two; the middle-third [Cantor set](cantor-set.md) has dimension $\log2/\log3\approx0.63093$.

Why can a dimension be fractional? At a scale reduced by a factor of three, the [Cantor set](cantor-set.md) needs twice as many construction intervals. The balance $2(1/3)^d=1$ gives $d=\log2/\log3$, between the growth rates of finitely many points and a whole interval. Making this argument rigorous requires a [cover](cover-topology.md) upper bound and the [mass distribution principle](mass-distribution-principle.md) lower bound, as in [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md).

At the critical exponent itself, [Hausdorff measure](hausdorff-measure.md) can be zero, finite and positive, or infinite; dimension does not specify that endpoint value. For example, [finite sets](finite-set.md) and [countably infinite sets](countably-infinite-set.md) both have dimension zero, although their [counting measures](counting-measure.md) differ. Dimension is also different from a finite-resolution estimate: [box-counting dimension](box-counting-dimension.md) is another asymptotic definition, and fitting a scaling slope over a handful of observed scales does not establish either dimension.

The metric matters. Multiplying every distance by a fixed positive constant multiplies $\mathcal H^s$ by that constant to the power $s$ and preserves [Hausdorff dimension](hausdorff-dimension.md). A [Lipschitz map](lipschitz-continuity.md) cannot increase it, because mapped [cover](cover-topology.md) [diameters](diameter.md) increase by at most a fixed factor. A [bi-Lipschitz map](bi-lipschitz-map.md) therefore preserves it by applying this fact in both directions. These properties make [Hausdorff dimension](hausdorff-dimension.md) useful for comparing geometric models while controlling how their measurements change.

**Table of contents**

- [Mass distribution principle](mass-distribution-principle.md)
- [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md)
- [Pressure upper bound for Hausdorff dimension](pressure-upper-bound-for-hausdorff-dimension.md)
- [Hausdorff dimension of a connected set](hausdorff-dimension-of-a-connected-set.md)

## ↑ Ancestors (8)

1. [Hausdorff measure](hausdorff-measure.md)
2. [Geometric measure theory](geometric-measure-theory.md)
3. [Measure theory](measure-theory-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (24)

- [Bi-Lipschitz map](bi-lipschitz-map.md)
- [Cantor set](cantor-set.md)
- [Cartesian powers of the Cantor set](cartesian-powers-of-the-cantor-set.md)
- [Euclidean similarity](euclidean-similarity.md)
- [Feigenbaum attractor](feigenbaum-attractor.md)
- [Finite similarity iterated function system](finite-similarity-iterated-function-system.md)
- [Fractal](fractal.md)
- [Geometric measure theory](geometric-measure-theory.md)
- [Hausdorff dimension](hausdorff-dimension.md)
- [Hausdorff dimension of a connected set](hausdorff-dimension-of-a-connected-set.md)
- [Hausdorff dimension of the Cantor set](hausdorff-dimension-of-the-cantor-set.md)
- [Hausdorff measure](hausdorff-measure.md)
- [Lebesgue null set](lebesgue-null-set.md)
- [Mass distribution principle](mass-distribution-principle.md)
- [Minkowski sausage](minkowski-sausage.md)
- [Open set condition](open-set-condition.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/3f/solution.md)
- [Tangent-disk Schottky group](tangent-disk-schottky-group.md)
