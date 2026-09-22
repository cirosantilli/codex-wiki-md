<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At a point $x\in X$, all restrictions of the [constant presheaf of sets](../../../../../constant-presheaf-of-sets.md) are identities. Two representatives $(U,t)$ and $(V,t')$ give the same [germ](../../../../../germ-of-a-sheaf-section.md) precisely when $t=t'$, so its [stalk](../../../../../stalk-of-a-sheaf.md) is canonically $T$. The disjoint union of the stalks is therefore the set $X\times T$.

The topology of the associated [étale space of a presheaf](../../../../../etale-space-of-a-presheaf.md) has basic opens obtained from sections over open $U$. For the constant section $t$, that basic open is $U\times\{t\}$. These are exactly the basic opens of the product topology with $T$ discrete. Consequently the germ-space identification is a homeomorphism over $X$, and the projection

$$
\boxed{p:X\times T_{\mathrm{disc}}\longrightarrow X}
$$

is a local homeomorphism.

A continuous section over $V$ has the form $x\mapsto(x,f(x))$, where $f:V\to T_{\mathrm{disc}}$ is continuous, equivalently [locally constant](../../../../../locally-constant-function.md). Its sections form the [constant sheaf of sets](../../../../../constant-sheaf-of-sets.md):

$$
\boxed{\Delta T(V)=\{f:V\to T:f\text{ is locally constant}\}.}
$$

The [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) follows by gluing the functions; continuity is local. This includes $\Delta T(\varnothing)$ being a singleton, even when the constant presheaf's value on the empty open set was $T$. The construction is its [sheafification](../../../../../sheafification.md).

A function $u:T\to T'$ acts by postcomposition on [locally constant](../../../../../locally-constant-function.md) functions, defining a [functor](../../../../../functor.md) $\Delta:\mathbf{Set}\to\mathbf{Sh}(X)$. It preserves identities and composition.

To prove the [adjunction](../../../../../adjoint-functors.md) with the [global sections functor](../../../../../global-sections-functor.md), let $F$ be a sheaf. A sheaf morphism $\lambda:\Delta T\to F$ gives a function

$$
T\longrightarrow F(X),\qquad
t\longmapsto\lambda_X(\text{constant function }t).
$$

Conversely, suppose global sections $s_t\in F(X)$ are prescribed for every $t\in T$. For a [locally constant](../../../../../locally-constant-function.md) $f:V\to T$, its fibres $V_t=f^{-1}(t)$ are disjoint open sets covering $V$. Restrict $s_t$ to $V_t$ and glue these sections. They agree on intersections, which are empty, so unique gluing defines $\lambda_V(f)$. Restriction to smaller opens commutes with this construction, making $\lambda$ a sheaf morphism.

Applying the two constructions successively returns the original data: a [locally constant](../../../../../locally-constant-function.md) function is locally one of the constant functions, and sheaf morphisms respect those restrictions and unique gluing. Naturality in $T$ and $F$ follows from postcomposition and restriction. Hence

$$
\boxed{\operatorname{Hom}_{\mathbf{Sh}(X)}(\Delta T,F)
\cong\operatorname{Set}(T,\Gamma F),\qquad \Delta\dashv\Gamma.}
$$

For an empty space the same proof works: all global sections sets are singletons, and the sheaf category is degenerate. Constant sheaves are generally [locally constant](../../../../../locally-constant-function.md) rather than globally constant on disconnected opens.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
