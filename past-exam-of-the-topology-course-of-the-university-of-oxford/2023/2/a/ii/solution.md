<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [equivalence relation induced by a function](../../../../../equivalence-relation-induced-by-a-function.md):

$$
x\sim x'\quad\Longleftrightarrow\quad f(x)=f(x').
$$

Equality in $Y$ supplies reflexivity, symmetry, and transitivity, so this is an [equivalence relation](../../../../../equivalence-relation.md). Define $\bar f:X/{\sim}\to Y$ by $\bar f([x])=f(x)$. It is well-defined; it is [injective](../../../../../injective-function.md) by the definition of $\sim$ and [surjective](../../../../../surjective-function.md) because $f$ is [surjective](../../../../../surjective-function.md).

For an [open set](../../../../../open-set.md) $W\subseteq Y$,

$$
p^{-1}\bigl(\bar f^{-1}(W)\bigr)=f^{-1}(W)
$$

is [open](../../../../../open-set.md) by [continuity](../../../../../continuous-function.md) of $f$. The [quotient topology](../../../../../quotient-topology.md) therefore makes $\bar f^{-1}(W)$ [open](../../../../../open-set.md), proving that $\bar f$ is [continuous](../../../../../continuous-function.md).

The [continuous image of a compact space](../../../../../continuous-image-of-a-compact-space.md) theorem applied to $p$ makes $X/{\sim}$ [compact](../../../../../compact-space.md). If $C$ is [closed](../../../../../closed-set.md) in $X/{\sim}$, it is [compact](../../../../../compact-space.md), and $\bar f(C)$ is [compact](../../../../../compact-space.md) in the [Hausdorff space](../../../../../hausdorff-space.md) $Y$, hence [closed](../../../../../closed-set.md). Thus $\bar f$ is a [closed map](../../../../../closed-map.md). Its [inverse function](../../../../../inverse-function.md) is [continuous](../../../../../continuous-function.md), since its [preimage](../../../../../preimage.md) of $C$ is precisely $\bar f(C)$. We have proved that $\bar f$ is a [homeomorphism](../../../../../homeomorphism.md), including the [compact-to-Hausdorff continuous bijection theorem](../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) used in the argument.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
