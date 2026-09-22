# Quotient topological space

↑ **Parent:** [Quotient topology](quotient-topology.md)

A [quotient topological space](quotient-topological-space.md) is a [quotient set](quotient-set.md) equipped with the [quotient topology](quotient-topology.md). For a concrete gluing, give the [closed interval](closed-real-interval.md) $I=[0,1]$ its usual [subspace topology](subspace-topology.md), identify $0\sim1$, and leave every interior point in its own [singleton](singleton-mathematics.md) [equivalence class](equivalence-class.md). The resulting [quotient space](quotient-topological-space.md) is a [circle](circle.md): the two endpoints become one point, while interior points remain distinct.

<a id="image-gluing-the-interval-endpoints-produces-a-circle-with-matching-colors-showing-the-projection"></a>
![](quotient-interval-endpoints-circle.png)

**[Figure 8](#image-gluing-the-interval-endpoints-produces-a-circle-with-matching-colors-showing-the-projection). Gluing the interval endpoints produces a circle, with matching colors showing the projection**.

The exact [continuous map](continuous-map.md) to the [unit circle](complex-unit-circle.md) in the plane is

$$
p(t)=\bigl(\cos(2\pi t),\sin(2\pi t)\bigr),\qquad
\bar p([t])=p(t).
$$

Here [sine](sine.md) and [cosine](cosine.md) give $p(0)=p(1)=(1,0)$, and $p(s)=p(t)$ holds exactly when $s=t$ or $\{s,t\}=\{0,1\}$. Thus $p$ induces a [bijection](bijection.md) $\bar p:I/{\sim}\to S^1$. [3.01 Quotient topology](topology-and-groups/3-01-quotient-topology.md) The [universal property of the quotient topology](universal-property-of-the-quotient-topology.md) makes $\bar p$ [continuous](continuous-function.md). The [quotient of a compact space](quotient-of-a-compact-space.md) is [compact](compact-space.md), and the [unit circle](complex-unit-circle.md) is [Hausdorff](hausdorff-space.md), so the [compact-to-Hausdorff continuous bijection theorem](compact-to-hausdorff-continuous-bijection-theorem.md) makes $\bar p$ a [homeomorphism](homeomorphism.md). This verifies the [topology](topology-split.md), not merely the point identifications.

To inspect an [open](open-set.md) [neighbourhood](neighbourhood-mathematics.md) of the seam, choose $0<\varepsilon<1/2$ and let $U_\varepsilon=p([0,\varepsilon)\cup(1-\varepsilon,1])$. Its full [preimage](preimage.md) is

$$
p^{-1}(U_\varepsilon)=[0,\varepsilon)\cup(1-\varepsilon,1].
$$

Both pieces are [open](open-set.md) in the [subspace topology](subspace-topology.md) on $I$, so $U_\varepsilon$ is [open](open-set.md) in the [circle](circle.md). In contrast, $A=[0,\varepsilon)$ is [open](open-set.md) in $I$, but

$$
p^{-1}\bigl(p(A)\bigr)=[0,\varepsilon)\cup\{1\}
$$

is not [open](open-set.md) in $I$: it contains $1$ without any [neighbourhood](neighbourhood-mathematics.md) of $1$. Hence $p(A)$ is not [open](open-set.md) in the [circle](circle.md). A [quotient map](quotient-map.md) can therefore fail to be an [open map](open-map.md).

<a id="image-an-open-neighbourhood-crosses-both-sides-of-the-glued-seam-a-one-sided-arc-fails-the-full-preimage-test"></a>
![](quotient-circle-open-preimages.png)

**[Figure 9](#image-an-open-neighbourhood-crosses-both-sides-of-the-glued-seam-a-one-sided-arc-fails-the-full-preimage-test). An open neighbourhood crosses both sides of the glued seam; a one-sided arc fails the full-preimage test**.

For a [continuous function](continuous-function.md) $f:I\to\mathbb R$, the only gluing condition is $f(0)=f(1)$. For example, $f(t)=\cos(2\pi t)$ defines a [continuous function](continuous-function.md) on the [circle](circle.md), whereas $f(t)=t$ does not. This lets us use an [interval](interval-mathematics.md) as a coordinate for a [periodic function](periodic-function.md) while making the seam invisible. More general [quotient spaces](quotient-topological-space.md) encode glued geometric pieces in the same way: describe [continuous maps](continuous-map.md) before gluing and check that their values agree on every [equivalence class](equivalence-class.md).

The [Hausdorff](hausdorff-space.md) property need not survive a [quotient topology](quotient-topology.md). In the [non-Hausdorff quotient of the real line by rational translation](non-hausdorff-quotient-of-the-real-line-by-rational-translation.md), $x\sim y$ means $x-y\in\mathbb Q$. A nonempty [open](open-set.md) [preimage](preimage.md) $W$ must contain all translates by [rational numbers](rational-number.md) of any [open interval](open-interval.md) inside it. The [density of the rational numbers](density-of-the-rational-numbers.md) then forces $W=\mathbb R$: for any $y$, some [rational number](rational-number.md) $r$ has $y-r$ in that [interval](interval-mathematics.md). Thus this [quotient space](quotient-topological-space.md) has the [indiscrete topology](indiscrete-topology.md). The [irrationality of the square root of two](irrationality-of-the-square-root-of-two.md) gives distinct [equivalence classes](equivalence-class.md) for $0$ and $\sqrt2$, so this [quotient space](quotient-topological-space.md) is not [Hausdorff](hausdorff-space.md). Unlike the endpoint-gluing [circle](circle.md), this gluing identifies a [dense subset](dense-set.md) with each point.

## ↑ Ancestors (6)

1. [Quotient topology](quotient-topology.md)
2. [Topology](topology-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/13e/a/solution.md)
- [Quotient topological space](quotient-topological-space.md)
