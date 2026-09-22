<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [presheaf](../../../../../presheaf-of-sets-on-a-topological-space.md) $\mathcal F$, first form its [stalks](../../../../../stalk-of-a-sheaf.md) $\mathcal F_x=\varinjlim_{x\in U}\mathcal F(U)$. Define $\mathcal F^+(U)$ to consist of families $(s_x)_{x\in U}$, with $s_x\in\mathcal F_x$, which are locally represented by sections of $\mathcal F$: every $x\in U$ has a neighbourhood $V\subseteq U$ and $t\in\mathcal F(V)$ with $s_y=t_y$ for all $y\in V$. Addition is pointwise and restriction discards the components outside the smaller open set. The local representability condition is itself local, so compatible such families on an [open cover](../../../../../open-cover.md) glue uniquely. Thus $\mathcal F^+$ is a [sheaf of abelian groups](../../../../../sheaf-of-abelian-groups.md). This is [sheafification by locally representable germs](../../../../../sheafification-by-locally-representable-germs.md).

The canonical [presheaf morphism](../../../../../morphism-of-presheaves.md) is

$$
\boxed{\theta_U:\mathcal F(U)\longrightarrow\mathcal F^+(U),\qquad t\longmapsto(t_x)_{x\in U}.}
$$

The [universal property of sheafification](../../../../../universal-property-of-sheafification.md) says that, for any [sheaf](../../../../../sheaf-mathematics.md) $\mathcal H$, composition with $\theta$ gives a natural bijection

$$
\operatorname{Hom}(\mathcal F^+,\mathcal H)\cong\operatorname{Hom}_{\mathrm{pre}}(\mathcal F,\mathcal H).
$$

Indeed, locally representing a family by $t$ defines its image locally by the image of $t$ in $\mathcal H$. Equal [germs](../../../../../germ-of-a-sheaf-section.md) give locally equal images, and the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) gives the unique global image. If $\mathcal F$ is already a [sheaf](../../../../../sheaf-mathematics.md), a section with all [germs](../../../../../germ-of-a-sheaf-section.md) zero is zero, while every locally represented family glues to an actual section. Hence $\theta_U$ is both injective and surjective for every $U$, so **[sheafification](../../../../../sheafification.md) leaves a [sheaf](../../../../../sheaf-mathematics.md) unchanged**.

For a continuous map $f:X\to Y$, the [direct image sheaf](../../../../../direct-image-sheaf.md) is

$$
\boxed{(f_*\mathcal F)(U)=\mathcal F(f^{-1}U).}
$$

An [open cover](../../../../../open-cover.md) pulls back to an [open cover](../../../../../open-cover.md), so its [sheaf](../../../../../sheaf-mathematics.md) axioms follow directly from those of $\mathcal F$. To construct the [inverse image sheaf](../../../../../inverse-image-sheaf.md), first set

$$
P(V)=\varinjlim_{\substack{U\subseteq Y\text{ open}\\f(V)\subseteq U}}\mathcal G(U),\qquad f^{-1}\mathcal G=P^+.
$$

Restriction uses the inclusion of these neighbourhood systems when $V$ shrinks. The use of [sheafification](../../../../../sheafification.md) is important: $P$ need not itself be a [sheaf](../../../../../sheaf-mathematics.md). Continuity and the [stalk](../../../../../stalk-of-a-sheaf.md) construction give $(f^{-1}\mathcal G)_x\cong\mathcal G_{f(x)}$.

Given an [f-morphism of sheaves](../../../../../f-morphism-of-sheaves.md) $\phi$, define its map on [stalks](../../../../../stalk-of-a-sheaf.md) by

$$
\boxed{\phi_x:\mathcal G_{f(x)}\longrightarrow\mathcal F_x,\qquad[s,U]\longmapsto[\phi(U)(s),f^{-1}U].}
$$

If two representatives have the same [germ](../../../../../germ-of-a-sheaf-section.md) at $f(x)$, they agree on a neighbourhood there. Restriction compatibility makes their images agree on its inverse image, a neighbourhood of $x$, proving well-definedness. The map is a group homomorphism. We index it by $x$, since different points over the same $f(x)$ have different target [stalks](../../../../../stalk-of-a-sheaf.md).

For $s\in\mathcal G(U)$, its class in $P(f^{-1}U)$ and then in its [sheafification](../../../../../sheafification.md) defines the canonical [f-morphism of sheaves](../../../../../f-morphism-of-sheaves.md) $\theta(U)$. Its [germ](../../../../../germ-of-a-sheaf-section.md) at $x$ is simply $s_{f(x)}$. To factor any $\phi$, take a section $t\in(f^{-1}\mathcal G)(V)$. Locally on an [open cover](../../../../../open-cover.md) $V=\bigcup V_a$, it comes from a section $s_a\in\mathcal G(U_a)$ with $V_a\subseteq f^{-1}U_a$. Define the prospective image on $V_a$ by

$$
\psi(t)|_{V_a}=\phi(U_a)(s_a)|_{V_a}.
$$

On an overlap, the representatives have the same inverse-image [germs](../../../../../germ-of-a-sheaf-section.md), so their images have the same [germs](../../../../../germ-of-a-sheaf-section.md) by the maps $\phi_x$. Two [sheaf](../../../../../sheaf-mathematics.md) sections with equal [germs](../../../../../germ-of-a-sheaf-section.md) everywhere are equal. The local images therefore glue uniquely, independently of every representative and cover choice. This construction is additive and commutes with restrictions, giving a [sheaf morphism](../../../../../morphism-of-sheaves.md) $\psi:f^{-1}\mathcal G\to\mathcal F$ with

$$
\boxed{\phi(U)=\psi(f^{-1}U)\circ\theta(U).}
$$

Conversely any factorization must have the prescribed image on these locally generating sections, proving uniqueness. This is the [universal property of an inverse image sheaf](../../../../../universal-property-of-an-inverse-image-sheaf.md).

An [f-morphism of sheaves](../../../../../f-morphism-of-sheaves.md) is exactly a [sheaf morphism](../../../../../morphism-of-sheaves.md) $\mathcal G\to f_*\mathcal F$. Thus the two constructions give the [inverse-image direct-image adjunction](../../../../../inverse-image-direct-image-adjunction.md)

$$
\boxed{\operatorname{Hom}_X(f^{-1}\mathcal G,\mathcal F)\cong\operatorname{Hom}_Y(\mathcal G,f_*\mathcal F).}
$$

Naturality follows from composing the local representatives and their images with morphisms in either [sheaf](../../../../../sheaf-mathematics.md) variable. This is an adjunction for [sheaves](../../../../../sheaf-mathematics.md) of abelian groups; it is not the tensor-adjusted pullback of [modules](../../../../../module-mathematics.md) on a ringed space.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
