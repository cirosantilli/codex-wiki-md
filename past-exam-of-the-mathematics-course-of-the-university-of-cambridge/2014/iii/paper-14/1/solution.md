<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Heegaard splitting](../../../../../heegaard-splitting.md) of a closed oriented [three-manifold](../../../../../3-manifold.md) is a decomposition $Y=H_0\cup_\Sigma H_1$ into two [handlebodies](../../../../../handlebody.md), with their common boundary the [Heegaard surface](../../../../../heegaard-surface.md) $\Sigma$. With boundary present, the corresponding pieces are [compression bodies](../../../../../compression-body.md), whose negative boundaries account for $\partial Y$.

For the given [triangulation](../../../../../triangulation.md), take the [barycentric subdivision](../../../../../barycentric-subdivision.md). A regular neighbourhood $H_0$ of the original one-skeleton is a [handlebody](../../../../../handlebody.md): thicken vertices to balls and edges to [one-handles](../../../../../one-handle.md), then contract a spanning tree. The complementary region is a regular neighbourhood $H_1$ of the dual one-skeleton, whose vertices are tetrahedron centres and whose edges cross triangular faces. It too is a [handlebody](../../../../../handlebody.md). Both graphs are connected, and their common boundary supplies the [Heegaard splitting](../../../../../heegaard-splitting.md). If the original [triangulation](../../../../../triangulation.md) has $v$ vertices and $e$ edges, its [Heegaard surface](../../../../../heegaard-surface.md) has [genus](../../../../../genus-of-a-surface.md) $e-v+1$; the dual count gives the same number by $v-e+f-t=0$.

Choose an oriented [meridian of a knot](../../../../../meridian-of-a-knot.md) $\mu$ and the [Seifert longitude](../../../../../seifert-longitude.md) $\lambda$ supplied by a [Seifert surface](../../../../../seifert-surface.md) for the null-homologous [knot](../../../../../knot.md). For relatively prime integers $p,q$, [rational Dehn surgery](../../../../../rational-dehn-surgery.md) removes the interior of a [tubular neighborhood](../../../../../tubular-neighborhood.md) and attaches a [solid torus](../../../../../solid-torus.md) with its [meridian of a solid torus](../../../../../meridian-of-a-solid-torus.md) on the unoriented slope $p\mu+q\lambda$. The choices $(p,q)$ and $(-p,-q)$ describe the same slope; $q=0$ is the original meridional filling. The boundary gluing reverses boundary orientation so that the oriented [three-manifold](../../../../../3-manifold.md) extends across the filling.

For integral coefficients $n_i$, attach [two-handles](../../../../../two-handle.md) to $B^4$ along the components of the [framed link](../../../../../framed-link.md), with their indicated [Seifert framing](../../../../../seifert-framing.md) shifts. The boundary operation removes $S^1\times D^2$ and inserts $D^2\times S^1$, with meridian $n_i\mu_i+\lambda_i$. Thus the compact oriented [surgery trace](../../../../../surgery-trace.md) satisfies

$$
\boxed{\partial W(L)=Y.}
$$

For a finite rational coefficient, use a negative [continued fraction](../../../../../continued-fraction.md)

$$
\frac pq=a_0-\frac1{a_1-\dfrac1{\cdots-1/a_k}}.
$$

Replace that component by an integrally framed chain of successive meridians with coefficients $a_0,\ldots,a_k$. Repeated [slam-dunk moves](../../../../../slam-dunk-move.md) give back $p/q$. Perform this replacement for every rationally framed component, leaving meridional fillings out. The resulting integral [framed link](../../../../../framed-link.md) has the same filled boundary, so its [surgery trace](../../../../../surgery-trace.md) proves that **every such rational filling bounds a compact oriented four-manifold**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
