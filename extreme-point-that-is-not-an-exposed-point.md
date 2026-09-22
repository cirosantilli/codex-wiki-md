# Extreme point that is not an exposed point

↑ **Parent:** [Extreme point](extreme-point.md)

The distinction appears at a smooth join between a straight segment and a curved boundary. Consider the [convex hull](convex-hull.md)

$$
C=\operatorname{conv}(D\cup\{P\}),\qquad D=\{z:\|z\|_2\leq1\},\qquad P=(2,0).
$$

The upper tangent from $P$ meets the [unit circle](complex-unit-circle.md) at $T=(1/2,\sqrt3/2)$. The [supporting line](supporting-line.md) is

$$
T\cdot z=1,\qquad T\cdot P=T\cdot T=1.
$$

Every [point](point-geometry.md) of the [unit disk](unit-disk.md) has $T\cdot z\leq1$, with equality only at $T$. Hence the [convex face](face-of-a-convex-set.md) of $C$ where equality holds is exactly the [line segment](line-segment.md) $TP$.

<a id="image-an-extreme-point-can-fail-to-be-an-exposed-point"></a>
![](extreme-point-not-exposed-rounded-hull.png)

**[Figure 4](#image-an-extreme-point-can-fail-to-be-an-exposed-point). An extreme point can fail to be an exposed point**. Original analytic [convex hull](convex-hull.md) of the [unit disk](unit-disk.md) and $P=(2,0)$. The tangent contact $T=(1/2,\sqrt3/2)$ is extreme, but its only [supporting line](supporting-line.md) contains the entire [line segment](line-segment.md) $TP$. A different marked [point](point-geometry.md) on the curved arc is exposed by its own tangent [line](straight-line.md).

The [point](point-geometry.md) $T$ is extreme. If a nontrivial [convex combination](convex-combination.md) of two [points](point-geometry.md) of $C$ equals $T$, both must belong to the [convex face](face-of-a-convex-set.md) $TP$. Since $T$ is an endpoint of that [line segment](line-segment.md), both must equal $T$.

Yet $T$ is not exposed. A nonzero [linear functional](linear-functional.md) maximizing at $T$ on $C$ must also maximize there on the included [unit disk](unit-disk.md). Its [vector](vector.md) must be a positive multiple of $T$, by the equality condition in the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). It then gives $P$ the same value as $T$. No [linear functional](linear-functional.md) can select $T$ alone. Being an [extreme point](extreme-point.md) is a property of possible mixtures; being an [exposed point](exposed-point.md) adds the ability to distinguish it by one linear objective.

## ↑ Ancestors (6)

1. [Extreme point](extreme-point.md)
2. [Convex set](convex-set-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
