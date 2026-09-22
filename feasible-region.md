# Feasible region

↑ **Parent:** [Feasible point](feasible-point.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feasible_region)

The [set](set-split.md) of all [feasible points](feasible-point.md) of an [optimization](mathematical-optimization-split.md) problem. It depends on the [optimization constraints](optimization-constraint.md) and the decision domain; the [objective function](objective-function.md) ranks its members.

Think of three successive questions. Which decisions can be represented in the model? Which satisfy every [optimization constraint](optimization-constraint.md)? Which of those receive the best [objective function](objective-function.md) value? For decisions $z$ in a domain $D$, [inequalities](inequality-mathematics.md) $g_i(z)\leq0$ and [equations](equation.md) $h_j(z)=0$ define the [feasible region](feasible-region.md)

$$
F=\{z\in D:g_i(z)\leq0\text{ for every }i,\ h_j(z)=0\text{ for every }j\}.
$$

The domain must be contained in the [domain of a function](domain-of-a-function.md) for every [function](function-split.md) being evaluated; choosing [integers](integer-split.md) rather than [real numbers](real-number.md) as decisions can also change the [feasible set](feasible-region.md). Constraint satisfaction determines membership of $F$. Minimizing an [objective function](objective-function.md) $f$ then compares its members by $f(z)$, with optimal value $\inf_{z\in F}f(z)$. Changing the scores while keeping $D$ and the [optimization constraints](optimization-constraint.md) fixed leaves $F$ unchanged, provided the new [objective function](objective-function.md) is defined throughout $D$. These distinctions separate an allowed decision from a best decision.[§4.1.1, printed pp. 127–128: problem domain, feasible set, optimal value and attainment](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

**Table of contents**

- [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
- [Equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md)
- [Empty and open feasible regions](empty-and-open-feasible-regions.md)

## ↑ Ancestors (5)

1. [Feasible point](feasible-point.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Bolzano-Weierstrass theorem](bolzano-weierstrass-theorem.md)
- [Convex feasible region for a resource budget](convex-feasible-region-for-a-resource-budget.md)
- [Convex hull](convex-hull.md)
- [Convex set](convex-set-split.md)
- [Empty and open feasible regions](empty-and-open-feasible-regions.md)
- [Equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md)
- [Feasible region](feasible-region.md)
- [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
- [Integer restrictions on a convex feasible region](integer-restrictions-on-a-convex-feasible-region.md)
- [Solution set](solution-set.md)
