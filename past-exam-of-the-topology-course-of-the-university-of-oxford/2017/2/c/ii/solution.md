<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $Q=(Z\times I)/\mathcal R$. Since $Q$ is [homeomorphic](../../../../../homeomorphism.md) to the [circle](../../../../../circle.md), it is [Hausdorff](../../../../../hausdorff-space.md). For fixed $t\in I$, the [function](../../../../../function-split.md)

$$
Z\longrightarrow Q,\qquad x\longmapsto p(x,t)
$$

is [continuous](../../../../../continuous-function.md), being a coordinate slice of the [quotient map](../../../../../quotient-map.md). Part (a)(i) therefore makes it constant. Choose $x_0\in Z$ and set

$$
g:I\longrightarrow Q,\qquad g(t)=p(x_0,t).
$$

Then $g$ is [continuous](../../../../../continuous-function.md) and

$$
p(x,t)=g(t)\qquad\text{for every }x\in Z,\ t\in I.
$$

Since the [quotient map](../../../../../quotient-map.md) $p$ is a [surjection](../../../../../surjective-function.md), so is $g$. This is [Hausdorff factorization through a cofinite product factor](../../../../../hausdorff-factorization-through-a-cofinite-product-factor.md): a [continuous map](../../../../../continuous-map.md) into a [Hausdorff space](../../../../../hausdorff-space.md) cannot distinguish the points of the coordinate with the [cofinite topology](../../../../../cofinite-topology.md).

If $g$ were injective, it would be a [continuous bijection](../../../../../continuous-bijection.md) from the [compact](../../../../../compact-space.md) [closed interval](../../../../../closed-real-interval.md) $I$ to the [Hausdorff space](../../../../../hausdorff-space.md) $Q$. Part (a)(ii) would make it a [homeomorphism](../../../../../homeomorphism.md), contradicting the fact that the [circle and interval are not homeomorphic](../../../../../circle-and-interval-are-not-homeomorphic.md).

To recall that obstruction explicitly, remove the interior point $1/2$ from $I$. The resulting [topological subspace](../../../../../topological-subspace.md) is separated by the nonempty relatively [open sets](../../../../../open-set.md) $[0,1/2)$ and $(1/2,1]$, so it is not [connected](../../../../../connected-space.md). The [circle](../../../../../circle.md) with any one point removed is [connected](../../../../../connected-space.md): after a rotation, it is the [image](../../../../../image-of-a-function.md) under a [continuous map](../../../../../continuous-map.md) of the [connected](../../../../../connected-space.md) [open interval](../../../../../open-interval.md) $(0,2\pi)$ under $t\mapsto(\cos t,\sin t)$. A [homeomorphism](../../../../../homeomorphism.md) and its restriction preserve [connectedness](../../../../../connected-space.md), giving a contradiction.

Thus $g$ is not injective. Choose distinct $a,b\in I$ with $g(a)=g(b)$. Then

$$
\boxed{p(x,a)=g(a)=g(b)=p(x,b)\quad\text{for every }x\in Z.}
$$

In particular the requested $x,a,b$ exist. The argument proves the stronger conclusion that the same two interval coordinates work for every $x$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
