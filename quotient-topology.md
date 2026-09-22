# Quotient topology

↑ **Parent:** [Topology](topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_topology)

The [quotient topology](quotient-topology.md) turns an instruction to glue points together into a precise [topological space](topological-space.md). Start with a [topological space](topological-space.md) $(X,\tau_X)$ and an [equivalence relation](equivalence-relation.md) $\sim$. The [quotient set](quotient-set.md) $X/{\sim}$ consists of [equivalence classes](equivalence-class.md), and its [canonical projection of a quotient set](canonical-projection-of-a-quotient-set.md) is

$$
q:X\longrightarrow X/{\sim},\qquad q(x)=[x].
$$

The [quotient topology](quotient-topology.md) is defined by the rule using [preimages](preimage.md) of [open sets](open-set.md):

$$
\tau_q=\{U\subseteq X/{\sim}:q^{-1}(U)\in\tau_X\}.
$$

Thus a [subset](subset.md) of the [quotient space](quotient-topological-space.md) is [open](open-set.md) if and only if its entire [preimage](preimage.md) is [open](open-set.md) in $X$. Each [fiber](fiber-of-a-function.md) $q^{-1}(\{[x]\})$ is the whole [equivalence class](equivalence-class.md) $[x]$, so the [preimage](preimage.md) includes every point glued to any of its members.[§2.3, Definitions 2.3.1 and 2.3.7 and Lemma 2.3.6](point-set-topology-by-romyar-sharifi.md)

This is the finest [topology](topology-split.md) making $q$ a [continuous map](continuous-map.md): every [topology](topology-split.md) with that property can contain only [subsets](subset.md) whose [preimages](preimage.md) are [open](open-set.md). It really is a [topology](topology-split.md), because [preimages](preimage.md) preserve the [empty set](empty-set.md), the whole [set](set-split.md), arbitrary [unions](set-union.md), and finite [intersections](set-intersection.md). The gluing example below shows why checking a complete [preimage](preimage.md) matters, especially at the seam.

The [quotient topology](quotient-topology.md) also makes [continuous maps](continuous-map.md) out of a glued space easy to construct. A [continuous map](continuous-map.md) $f:X\to Z$ descends to a unique [continuous map](continuous-map.md) $\bar f:X/{\sim}\to Z$ exactly when it is constant on every [fiber](fiber-of-a-function.md) of $q$, meaning $x\sim y\Rightarrow f(x)=f(y)$. Define $\bar f([x])=f(x)$; the [equivalence class representative](equivalence-class-representative.md) cannot affect the answer. For every [open set](open-set.md) $V\subseteq Z$,

$$
q^{-1}\bigl(\bar f^{-1}(V)\bigr)=f^{-1}(V).
$$

The right side is [open](open-set.md), so the [quotient topology](quotient-topology.md) makes $\bar f^{-1}(V)$ [open](open-set.md). Conversely, if $f=\bar f\circ q$ for a [continuous map](continuous-map.md) $\bar f$, then [composition of continuous functions](composition-of-continuous-functions.md) makes $f$ [continuous](continuous-function.md), and equal [equivalence classes](equivalence-class.md) force equal values. This is the [universal property of the quotient topology](universal-property-of-the-quotient-topology.md). [3.02 Quotient topology: continuous maps](topology-and-groups/3-02-quotient-topology-continuous-maps.md)

A [surjective](surjective-function.md) [continuous map](continuous-map.md) is not automatically a [quotient map](quotient-map.md). On the same two-point [set](set-split.md) $D=\{a,b\}$, take the [identity map](identity-function.md) from the [discrete topology](discrete-space.md) to the [indiscrete topology](indiscrete-topology.md). It is [continuous](continuous-function.md) and [surjective](surjective-function.md), but $\{a\}$ is not [open](open-set.md) in the target even though its [preimage](preimage.md) is [open](open-set.md) in the domain. The [quotient topology](quotient-topology.md) for this [identity map](identity-function.md) would be the [discrete topology](discrete-space.md). Thus [continuity](continuous-function.md) supplies only one direction of the rule using [preimages](preimage.md) of [open sets](open-set.md); a [quotient map](quotient-map.md) requires both.

**Table of contents**

- [Quotient topological space](quotient-topological-space.md)
- [Quotient map](quotient-map.md)
- [Universal property of the quotient topology](universal-property-of-the-quotient-topology.md)
- [Non-Hausdorff quotient of the real line by rational translation](non-hausdorff-quotient-of-the-real-line-by-rational-translation.md)
- [Square quotient model of the two-sphere](square-quotient-model-of-the-two-sphere.md)

## ↑ Ancestors (5)

1. [Topology](topology-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Indiscrete topology](indiscrete-topology.md)
- [Metric on the antipodal sphere quotient](metric-on-the-antipodal-sphere-quotient.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-21/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-29/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/12g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/13e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/13e/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/13g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/21f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/2f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/21f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/10g/i/solution.md)
- [Quotient topological space](quotient-topological-space.md)
- [Quotient topology](quotient-topology.md)
