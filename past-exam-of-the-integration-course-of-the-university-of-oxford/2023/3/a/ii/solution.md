<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [Lebesgue measure](../../../../../lebesgue-measure.md) restricted to the [Lebesgue measurable set](../../../../../lebesgue-measurable-set.md) $E$. For $1\leq p<\infty$, start with the measurable real-valued [functions](../../../../../function-split.md) $f$ on $E$ satisfying $\int_E|f|^p\,dm<\infty$. Define an [equivalence relation](../../../../../equivalence-relation.md) by $f\sim g$ when $f=g$ [almost everywhere](../../../../../almost-everywhere.md), and let $L^p(E)$ consist of their [equivalence classes](../../../../../equivalence-class.md). Addition and scalar multiplication are defined using representatives. The [Lp norm](../../../../../lp-norm.md) is

$$
\boxed{\|[f]\|_p=\left(\int_E|f|^p\,dm\right)^{1/p},\qquad1\leq p<\infty.}
$$

For $p=\infty$, use measurable [functions](../../../../../function-split.md) bounded [almost everywhere](../../../../../almost-everywhere.md), apply the same identification, and define the [L-infinity norm](../../../../../l-infinity-norm.md) by

$$
\boxed{\|[f]\|_\infty=\operatorname*{ess\,sup}_{x\in E}|f(x)|
=\inf\{C\geq0:m(\{x\in E:|f(x)|>C\})=0\}.}
$$

These expressions are independent of the representative. For finite $p$, zero [norm](../../../../../norm.md) is equivalent to $f=0$ [almost everywhere](../../../../../almost-everywhere.md): each set $\{|f|>1/n\}$ must have measure zero, and their union is $\{f\ne0\}$. The same implication follows from the [essential supremum](../../../../../essential-supremum.md) for $p=\infty$. Absolute homogeneity is immediate; [Minkowski inequality](../../../../../minkowski-inequality.md) proves the [triangle inequality](../../../../../triangle-inequality.md) and closure under addition. Thus these are [normed vector spaces](../../../../../normed-vector-space-split.md). Using complex-valued representatives gives their complex versions by the same construction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
