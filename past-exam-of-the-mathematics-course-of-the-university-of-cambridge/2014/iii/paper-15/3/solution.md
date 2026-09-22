<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [fiber metric](../../../../../fiber-metric.md) on a real [vector bundle](../../../../../vector-bundle.md) $E\to M$ is a smoothly varying positive-definite [inner product](../../../../../inner-product.md) on each fiber. Choose a trivializing open cover $\{U_i\}$ and a smooth [partition of unity](../../../../../partition-of-unity.md) $\{\rho_i\}$ subordinate to it. The partition theorem gives nonnegative functions summing to one, a [locally finite family of subsets](../../../../../locally-finite-family-of-subsets.md) of supports, and $\operatorname{supp}\rho_i\subset U_i$; the usual Hausdorff second-countable [smooth manifold](../../../../../smooth-manifold.md) hypotheses ensure this theorem applies. Transfer the Euclidean [inner product](../../../../../inner-product.md) to each local [vector bundle trivialization](../../../../../vector-bundle-trivialization.md), obtaining $h_i$, and set

$$
h_x(v,w)=\sum_i\rho_i(x)(h_i)_x(v,w).
$$

Each weighted term extends smoothly by zero outside $U_i$, and local finiteness makes the sum smooth in every [vector bundle trivialization](../../../../../vector-bundle-trivialization.md). At each $x$ some weight is positive, so $h_x(v,v)>0$ for every nonzero $v$. This proves existence of a [fiber metric](../../../../../fiber-metric.md), with no orientability or triviality assumption.

A [vector bundle morphism](../../../../../vector-bundle-morphism.md) covering the identity is a smooth map $F:E'\to E''$ that preserves base points and is a [linear map](../../../../../linear-map.md) on each fiber. Its induced map on the [module of smooth sections](../../../../../module-of-smooth-sections.md) is $s\mapsto F\circ s$, and is $C^\infty(M)$-linear. We prove the converse by constructing [bundle morphisms from maps of smooth sections](../../../../../bundle-morphisms-from-maps-of-smooth-sections.md).

First the given map $\alpha$ is local. If a global section $s$ vanishes on a neighborhood of $x$, take a [smooth bump function](../../../../../smooth-bump-function.md) $\chi$ supported there with $\chi=1$ near $x$. Then $\chi s=0$, so $\chi\alpha(s)=\alpha(\chi s)=0$, and hence $\alpha(s)(x)=0$. Thus sections agreeing near $x$ have images agreeing at $x$.

Choose a local frame $e_1,\ldots,e_r$ on $U$, and a bump function equal to one on a smaller neighborhood $V$ of $x$ and supported in $U$. Multiplying the frame by that bump and extending by zero gives global smooth sections $t_j$ whose restrictions to $V$ are the frame. If $s(x)=0$, write $s=\sum a_j e_j$ on $V$. A second bump extends each $a_j$ to a global smooth function $\widetilde a_j$ agreeing near $x$. By locality and $C^\infty(M)$-linearity,

$$
\alpha(s)(x)=\sum_j\widetilde a_j(x)\alpha(t_j)(x)=0.
$$

Every fiber vector $v\in E'_x$ is the value of a global smooth section, by the same bumped-frame construction. Define $F_x(v)=\alpha(s)(x)$ for any such section. The just-proved vanishing statement makes this well-defined. The maps $F_x$ are [linear maps](../../../../../linear-map.md), and locally their matrix columns are the smooth sections $\alpha(t_j)$ in a frame of $E''$. Thus $F$ is smooth, is a [vector bundle morphism](../../../../../vector-bundle-morphism.md), and satisfies $\alpha(s)=F\circ s$. Fiberwise evaluation also proves uniqueness.

Finally apply the [fiber metric](../../../../../fiber-metric.md) construction to the [tangent bundle](../../../../../tangent-bundle.md). A [Riemannian metric](../../../../../riemannian-metric.md) $g$ defines the [musical isomorphism](../../../../../musical-isomorphism.md)

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g(v,\cdot).}
$$

Positive definiteness makes it a fiberwise bijection; its inverse is smooth because inverse metric matrices vary smoothly. Hence **$TM$ and $T^*M$ are isomorphic as real smooth vector bundles on every such manifold.** The isomorphism depends on the chosen metric and is not canonical.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
