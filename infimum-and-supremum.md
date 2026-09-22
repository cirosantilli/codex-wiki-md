# Infimum and supremum

↑ **Parent:** [Real analysis](real-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infimum_and_supremum)

For a [subset](subset.md) $A$ of a [partially ordered set](partially-ordered-set.md), its [infimum](infimum.md) is its [greatest lower bound](greatest-lower-bound-in-a-partially-ordered-set.md) and its [supremum](supremum.md) is its [least upper bound](least-upper-bound-in-a-partially-ordered-set.md). An [upper bound](upper-bound-in-a-partially-ordered-set.md) only has to lie above every member; the [supremum](supremum.md) is the smallest such bound. A [lower bound](lower-bound-in-a-partially-ordered-set.md) lies below every member; the [infimum](infimum.md) is the largest such bound. These definitions identify the exact edges of a [set](set-split.md) even when neither edge belongs to it.

For example, $(0,1)$ and $[0,1]$ both have [infimum](infimum.md) zero and [supremum](supremum.md) one. Only $[0,1]$ has a [minimum](minimum-of-a-subset-of-a-total-order.md) and a [maximum](maximum-of-a-subset-of-a-total-order.md): those must be actual members of the [set](set-split.md). The [set](set-split.md) $C=\{1/n:n\in\mathbb N_{>0}\}$ has [infimum](infimum.md) zero without a [minimum](minimum-of-a-subset-of-a-total-order.md), but its [supremum](supremum.md) one is also its [maximum](maximum-of-a-subset-of-a-total-order.md). Such examples distinguish a bound from an attained extremal value. [Basic Analysis: Introduction to Real Analysis, Volume I by Jiří Lebl; Lebl, Basic Analysis I, §1.2: supremum, infimum and attainment](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/1-2-the-set-of-real-numbers.md).

<a id="image-infimum-and-supremum-need-not-be-attained-as-a-minimum-or-maximum"></a>
![](infimum-supremum-attainment.png)

**[Figure 3](#image-infimum-and-supremum-need-not-be-attained-as-a-minimum-or-maximum). Infimum and supremum need not be attained as a minimum or maximum**. Filled endpoint markers belong to the displayed [set](set-split.md); hollow markers do not. The reciprocal row shows selected values $1/n$, with further values accumulating toward the excluded lower edge zero. The finite row attains both bounds.

For a nonempty [subset](subset.md) of the [real numbers](real-number.md), [completeness of the real numbers](completeness-of-the-real-numbers.md) guarantees a real [supremum](supremum.md) when it is bounded above, and a real [infimum](infimum.md) when it is bounded below. The bound and the ambient [partially ordered set](partially-ordered-set.md) both matter: $\{q\in\mathbb Q:q\geq0,\ q^2<2\}$ has [supremum](supremum.md) $\sqrt2$ in the [real numbers](real-number.md), but no [supremum](supremum.md) in the [rational numbers](rational-number.md). The detailed explanation belongs to [completeness of the real numbers](completeness-of-the-real-numbers.md).

Why are unattained bounds useful? They specify a precise limiting target. In [mathematical optimization](mathematical-optimization-split.md), $f(x)=x$ on $(0,1)$ has [infimum](infimum.md) zero but no [global minimizer](global-minimizer.md). The inputs $x_n=1/n$ for $n\geq2$ give a [minimizing sequence](minimizing-sequence.md): their objective values approach zero without ever reaching it. Bounds therefore describe what approximation can achieve even when no feasible input is best. The [approximation property of an infimum](approximation-property-of-an-infimum.md) and [approximation property of a supremum](approximation-property-of-a-supremum.md) express this idea quantitatively.

**Table of contents**

- [Essential infimum and essential supremum](essential-infimum-and-essential-supremum.md)
  - [Essential infimum](essential-infimum.md)
- [Supremum](supremum.md)
  - [Supremum of a sum](supremum-of-a-sum.md)
  - [Stability of a supremum under uniform perturbations](stability-of-a-supremum-under-uniform-perturbations.md)
  - [Approximation property of a supremum](approximation-property-of-a-supremum.md)
  - [Accumulation below an unattained supremum](accumulation-below-an-unattained-supremum.md)
- [Infimum](infimum.md)
  - [Approximation property of an infimum](approximation-property-of-an-infimum.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Upper and lower bounds](upper-and-lower-bounds.md)
