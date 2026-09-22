<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal B$ be a [topological basis](../../../../../basis-of-a-topology.md) consisting of [clopen sets](../../../../../clopen-set.md). For $U\in\mathcal B$ its [characteristic function](../../../../../characteristic-function-split.md) $\chi_U:X\to\{0,1\}$ is [continuous](../../../../../continuous-function.md), since the preimages of both singleton values are [open](../../../../../open-set.md). Define

$$
e:X\to\{0,1\}^{\mathcal B},\qquad e(x)=(\chi_U(x))_{U\in\mathcal B}.
$$

The coordinate criterion for [product topology](../../../../../product-topology.md) makes this map [continuous](../../../../../continuous-function.md). If $x\ne y$, the $T_0$ property gives an [open set](../../../../../open-set.md) containing one and not the other. A [topological basis](../../../../../basis-of-a-topology.md) element contained in that [open set](../../../../../open-set.md) still distinguishes them, so their corresponding characteristic coordinates differ. Therefore $e$ is [injective](../../../../../injective-function.md).

Finally, for each [topological basis](../../../../../basis-of-a-topology.md) element $U$,

$$
U=e^{-1}(\{z:z_U=1\}).
$$

The right-hand side is the preimage of an [open](../../../../../open-set.md) cylinder in the product of discrete two-point [topological spaces](../../../../../topological-space.md). These cylinders recover a [topological basis](../../../../../basis-of-a-topology.md) for the [topology](../../../../../topology-split.md) of $X$, proving [continuity](../../../../../continuous-function.md) of the inverse onto the image. Hence

$$
\boxed{X\text{ embeds homeomorphically into }\{0,1\}^{\mathcal B}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
