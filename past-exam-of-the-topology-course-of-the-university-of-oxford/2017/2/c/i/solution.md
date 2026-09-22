<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $x_0,y_0\in Z$. For a [continuous function](../../../../../continuous-function.md) $f:Z\times Z\to\mathbb R$, every coordinate slice is [continuous](../../../../../continuous-function.md), because the maps $x\mapsto(x,y)$ and $y\mapsto(x_0,y)$ into the [product topology](../../../../../product-topology.md) are [continuous](../../../../../continuous-function.md). Their target $\mathbb R$ is [Hausdorff](../../../../../hausdorff-space.md). Part (a)(i) gives

$$
f(x,y)=f(x_0,y)=f(x_0,y_0)\qquad\text{for every }(x,y).
$$

Therefore **every such $f$ is a [constant function](../../../../../constant-function.md)**. This is the two-factor case of [continuous maps from products of cofinite spaces to Hausdorff spaces are constant](../../../../../continuous-maps-from-products-of-cofinite-spaces-to-hausdorff-spaces-are-constant.md).

The second [coordinate projection](../../../../../coordinate-projection.md) $\pi_2:Z\times\mathbb R\to\mathbb R$ is [continuous](../../../../../continuous-function.md) and nonconstant. If a [homeomorphism](../../../../../homeomorphism.md) $H:Z\times Z\to Z\times\mathbb R$ existed, $\pi_2\circ H$ would be a nonconstant [continuous function](../../../../../continuous-function.md), contradicting the preceding conclusion. Hence

$$
\boxed{Z\times Z\not\cong Z\times\mathbb R.}
$$

For the half-plane, put $H_+=[0,\infty)$ as a [set](../../../../../set-split.md), so $K=\mathbb R\times H_+$. Its two ambient [topologies](../../../../../topology-split.md) give different answers:

$$
\begin{array}{c|cc}
\text{ambient space}&K\text{ closed?}&K\text{ compact?}\\\hline
Z\times Z&\text{no}&\text{yes}\\
Z\times\mathbb R&\text{yes}&\text{no}.
\end{array}
$$

In $Z\times Z$, if $K$ were [closed](../../../../../closed-set.md), its [inverse image](../../../../../preimage.md) under the [continuous map](../../../../../continuous-map.md) $y\mapsto(x_0,y)$ would be [closed](../../../../../closed-set.md) in $Z$. That [inverse image](../../../../../preimage.md) is $H_+$, which is neither a [finite set](../../../../../finite-set.md) nor all of $Z$, so it is not [closed](../../../../../closed-set.md) in the [cofinite topology](../../../../../cofinite-topology.md). Thus $K$ is **not [closed](../../../../../closed-set.md)**.

To establish [compactness](../../../../../compact-space.md), note that the [subspace topology](../../../../../subspace-topology.md) on any [subset](../../../../../subset.md) $A$ of a [topological space](../../../../../topological-space.md) with the [cofinite topology](../../../../../cofinite-topology.md) is again cofinite. An [open cover](../../../../../open-cover.md) of a nonempty such $A$ has a nonempty member omitting at most finitely many points; finitely many more members cover those points. Hence [every subset of a cofinite space is compact](../../../../../every-subset-of-a-cofinite-space-is-compact.md). In particular both $Z$ and $H_+$ with its cofinite [subspace topology](../../../../../subspace-topology.md) are [compact](../../../../../compact-space.md). The [subspace topology](../../../../../subspace-topology.md) on $K\subseteq Z\times Z$ is their [product topology](../../../../../product-topology.md), as one checks by tracing basis rectangles. The [product of two compact spaces](../../../../../product-of-two-compact-spaces.md) is [compact](../../../../../compact-space.md), so $K$ is **[compact](../../../../../compact-space.md)** here.

For clarity, the finite-product [compactness](../../../../../compact-space.md) result needs no [Hausdorff condition](../../../../../hausdorff-space.md). Given an [open cover](../../../../../open-cover.md) of $A\times B$, cover each point by a basis rectangle lying in one covering member. For fixed $a\in A$, use [compactness](../../../../../compact-space.md) of $B$ to select finitely many rectangles whose second factors cover $B$, and intersect their first factors to get an [open neighbourhood](../../../../../open-neighbourhood.md) $U_a$ of $a$. Those finitely many original members cover $U_a\times B$. Finally finitely many $U_a$ cover $A$, producing a [finite subcover](../../../../../finite-subcover.md) of $A\times B$.

In $Z\times\mathbb R$, the second [coordinate projection](../../../../../coordinate-projection.md) has

$$
K=\pi_2^{-1}([0,\infty)).
$$

Since the ray is [closed](../../../../../closed-set.md) in the usual [real line](../../../../../real-line.md), $K$ is **[closed](../../../../../closed-set.md)**. It is **not [compact](../../../../../compact-space.md)**: its [image](../../../../../image-of-a-function.md) under a [continuous map](../../../../../continuous-map.md) under $\pi_2$ is $[0,\infty)$, which is not [compact](../../../../../compact-space.md). For an explicit obstruction, the [open intervals](../../../../../open-interval.md) $(-1,n)$, $n\geq1$, cover this ray but have no [finite subcover](../../../../../finite-subcover.md).

Finally consider the diagonal $W$ in $Z\times\mathbb R$. Define

$$
\varphi:\mathbb R\longrightarrow W,\qquad \varphi(t)=(t,t).
$$

This is a [bijection](../../../../../bijection.md). The identity [function](../../../../../function-split.md) from the usual [real line](../../../../../real-line.md) to $Z$ is [continuous](../../../../../continuous-function.md): each nonempty cofinite [open set](../../../../../open-set.md) is the [complement](../../../../../complement-of-a-set.md) of a [finite set](../../../../../finite-set.md), and [finite sets](../../../../../finite-set.md) are [closed](../../../../../closed-set.md) in the usual [real line](../../../../../real-line.md). Both coordinates of $\varphi$ are therefore [continuous](../../../../../continuous-function.md), so $\varphi$ is [continuous](../../../../../continuous-function.md) for the [product topology](../../../../../product-topology.md) and the [subspace topology](../../../../../subspace-topology.md) of $W$. Its inverse is the restricted second [coordinate projection](../../../../../coordinate-projection.md), which is [continuous](../../../../../continuous-function.md). Therefore

$$
\boxed{W\cong\mathbb R,\qquad W\not\cong Z.}
$$

For the second conclusion, $Z$ is [compact](../../../../../compact-space.md) whereas $W\cong\mathbb R$ is not [compact](../../../../../compact-space.md); [homeomorphisms](../../../../../homeomorphism.md) preserve [compactness](../../../../../compact-space.md). The [diagonal in a product with cofinite and Euclidean topologies](../../../../../diagonal-in-a-product-with-cofinite-and-euclidean-topologies.md) thus inherits the usual [topology](../../../../../topology-split.md), despite one cofinite factor.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
