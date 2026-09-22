<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [fiber bundle](../../../../../fiber-bundle-split.md) with base $B$, fiber $F$ and structure group $G$ acting on $F$ from the left consists of a projection $\pi:E\to B$ and local trivializations $\phi_i:\pi^{-1}(U_i)\to U_i\times F$. On overlaps they satisfy

$$
\phi_i\phi_j^{-1}(x,f)=(x,g_{ij}(x)\cdot f),\qquad g_{ij}g_{jk}=g_{ik}.
$$

The smooth transition functions are valued in $G$. A [principal bundle](../../../../../principal-bundle.md) is the case $F=G$ with the left multiplication action on itself; its transition functions multiply the group coordinate from the left.

In each principal chart define $(x,h)\cdot a=(x,ha)$. This defines a global right action because $g_{ij}(x)(ha)=(g_{ij}(x)h)a$: coordinate changes commute with right multiplication. It is free, and acts transitively on each fiber. Thus the claimed right action follows from the left transition convention rather than being an additional choice.

If $s:B\to P$ is a global [section of a fiber bundle](../../../../../section-fiber-bundle.md), define $\Phi:B\times G\to P$ by $\Phi(x,a)=s(x)a$. Freeness and transitivity give exactly one $a$ for every point in the fiber, so $\Phi$ is bijective and equivariant. In a local trivialization where $s(x)$ has group coordinate $h_i(x)$, the inverse group coordinate is $h_i(x)^{-1}h$, proving smoothness of the inverse. Hence $\Phi$ is a principal-bundle trivialization. Conversely, the identity coordinate in a product trivialization gives $s(x)=\Phi(x,e)$. Therefore

$$
\boxed{P\text{ is trivial as a principal bundle}\iff P\text{ has a global section}.}
$$

This is the [principal bundle trivialization by a global section](../../../../../principal-bundle-trivialization-by-a-global-section.md) criterion. It is special to principal bundles; a section alone need not trivialize an arbitrary fiber bundle.

For the quotient examples, assume the Lie subgroups are closed when smooth homogeneous-space statements are intended. The map $G\to G/H_1$ is a [principal bundle](../../../../../principal-bundle.md) with structure group $H_1$ and right action $g\cdot h=gh$; $G/H_1$ is a [homogeneous space](../../../../../homogeneous-space.md) for left multiplication by $G$. Similarly, $G\to H_2\backslash G$ has free transitive left $H_2$ action on its fibers. With the usual principal right-action convention one writes $g\cdot h=h^{-1}g$. The quotient $H_2\backslash G$ is a homogeneous space for right multiplication by $G$. These quotients are groups only when the respective subgroups are normal. Nonclosed immersed Lie subgroups can produce non-Hausdorff quotients, so an arbitrary Lie subgroup does not automatically give a smooth Hausdorff base.

Left $H_2$ and right $H_1$ multiplication commute, so taking their orbit equivalence relations in either order gives the same [double coset](../../../../../double-coset.md) set

$$
H_2\backslash G/H_1=(H_2\backslash G)/H_1=H_2\backslash(G/H_1).
$$

This equality does not assert that the double quotient is a manifold or that either stage is a principal bundle. The $H_2\times H_1$ action $(a,b):g\mapsto agb^{-1}$ can have stabilizers: they correspond to $H_2\cap gH_1g^{-1}$. If the induced action is free and proper, its quotient is a smooth principal-bundle quotient; without those hypotheses orbit dimensions can change. For example, with $G=SO(3)$ and both subgroups the rotations fixing the third axis, double cosets are parametrized by $e_3\cdot ge_3\in[-1,1]$. Interior and endpoint stabilizers differ, so this is not a uniform free principal-bundle construction.

For a [principal bundle](../../../../../principal-bundle.md) $P$ and a left $G$ action on $F$, the [associated bundle](../../../../../associated-bundle.md) is

$$
P\times_G F=(P\times F)/\sim,\qquad (pa,f)\sim(p,af),
$$

with projection $[p,f]\mapsto\pi(p)$. A local principal section gives coordinates $[s_i(x),f]\leftrightarrow(x,f)$, and its changes give precisely the left action of the principal transition functions on $F$. A linear action on a vector space gives an [associated vector bundle](../../../../../associated-vector-bundle.md).

For a metric of signature $(r,s)$ on an $n$-manifold, an orthonormal frame at $x$ is an isometry $u:\mathbb R^{r,s}\to T_xM$. The [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md) $O(M,g)\to M$ has structure group $O(r,s)$, acting on the right by $u\cdot a=u\circ a$. Its associated bundle for the standard representation is the [tangent bundle](../../../../../tangent-bundle.md), since

$$
O(M,g)\times_{O(r,s)}\mathbb R^n\longrightarrow TM,\qquad [u,v]\longmapsto u(v)
$$

is well defined: $(ua)(v)=u(av)$. Every tangent vector has exactly one such associated equivalence class, and local frame coordinates show that this is a vector-bundle isomorphism. The full frame bundle works similarly with $GL(n,\mathbb R)$.

Finally, choose a basis of the Lie algebra of a [Lie group](../../../../../lie-group.md) $G$. Its left translates are a global frame, yielding the explicit [tangent bundle](../../../../../tangent-bundle.md) trivialization

$$
\boxed{G\times\mathfrak g\longrightarrow TG,\qquad(g,v)\longmapsto(dL_g)_e v.}
$$

This proves [parallelization of a Lie group by left translations](../../../../../parallelization-of-a-lie-group-by-left-translations.md) and triviality of the full frame bundle. Choosing an inner product at the identity and translating it gives a left-invariant Riemannian metric; an orthonormal basis translates to a global orthonormal frame. The global section criterion therefore trivializes the corresponding orthonormal frame bundle as well. For any other positive-definite metric on $G$, smoothly applying the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to this global frame gives the same conclusion. Thus **the tangent and frame bundles of every Lie group are trivial**; the orthonormal statement is with respect to a chosen metric as specified above.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
