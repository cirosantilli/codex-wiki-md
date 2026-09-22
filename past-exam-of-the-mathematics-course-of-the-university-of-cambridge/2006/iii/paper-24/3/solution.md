<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [locally small category](../../../../../locally-small-category.md) $\mathcal C$, the covariant [Yoneda lemma](../../../../../yoneda-lemma.md) gives a bijection

$$
\boxed{\operatorname{Nat}(\mathcal C(c,-),H)\cong H(c),\qquad\tau\longmapsto\tau_c(1_c),}
$$

natural in $c$ and the [functor](../../../../../functor.md) $H:\mathcal C\to\mathbf{Set}$. The inverse sends $x\in H(c)$ to the [natural transformation](../../../../../natural-transformation.md) whose component at $d$ maps $u:c\to d$ to $H(u)x$. Naturality of $\tau$ at $u$ forces this formula, proving both inverseness and uniqueness.

Write $\mathcal E=\int F$ for the [category of elements](../../../../../category-of-elements.md) of $F$. Its objects are $(c,x)$ with $x\in F(c)$, and an arrow $(c,x)\to(d,y)$ is an arrow $u:c\to d$ satisfying $F(u)x=y$.

Given an object $\alpha:P\to F$ of the [slice category](../../../../../slice-category.md) $[\mathcal C,\mathbf{Set}]/F$, define

$$
\Phi(\alpha)(c,x)=\{p\in P(c):\alpha_c(p)=x\}.
$$

An arrow $u:(c,x)\to(d,y)$ acts by the restriction of $P(u)$; [naturality](../../../../../naturality.md) of $\alpha$ makes this restriction well-defined. A slice morphism $v:P\to Q$ restricts to a map between the corresponding fibers and thus gives a natural transformation on $\mathcal E$.

Conversely, given $H:\mathcal E\to\mathbf{Set}$, set

$$
P_H(c)=\coprod_{x\in F(c)}H(c,x),\qquad P_H(u)(x,h)=(F(u)x,H(u)h),
$$

and let $\alpha_H:P_H\to F$ be projection to $x$. The [functor](../../../../../functor.md) laws and naturality follow from those for $F$ and $H$. On morphisms use the maps on each summand. Taking a fiber of this disjoint union recovers $H(c,x)$ canonically. Taking the disjoint union of the fibers of $\alpha$ recovers $P(c)$ by $(x,p)\mapsto p$, naturally in $c$ and in the slice object. These are inverse [natural isomorphisms](../../../../../natural-isomorphism.md), proving

$$
\boxed{[\mathcal C,\mathbf{Set}]/F\simeq[\mathcal E,\mathbf{Set}].}
$$

This is the [slice of a set-valued functor category](../../../../../slice-of-a-set-valued-functor-category.md) construction.

Now assume $\mathcal C$ is a [small category](../../../../../small-category.md), so $\mathcal E$ is small. Define a [diagram in a category](../../../../../diagram-category-theory.md)

$$
D:\mathcal E^{\mathrm{op}}\longrightarrow[\mathcal C,\mathbf{Set}],\qquad D(c,x)=\mathcal C(c,-).
$$

For $u:(c,x)\to(d,y)$ in $\mathcal E$, its reverse arrow acts by precomposition $\mathcal C(d,-)\to\mathcal C(c,-)$. There is a [cocone](../../../../../cocone-under-a-diagram.md) to $F$ with component $g\mapsto F(g)x$. To verify its colimit property directly, use pointwise [colimits](../../../../../colimit.md) of sets. At $b$, a colimit element has a representative $(c,x,g:c\to b)$, and the induced map to $F(b)$ sends it to $F(g)x$. This map is surjective, since $z\in F(b)$ is represented by $(b,z,1_b)$. Moreover, the element-category arrow $g:(c,x)\to(b,F(g)x)$ gives precisely the colimit relation

$$
[(c,x,g)]=[(b,F(g)x,1_b)].
$$

Thus all representatives with the same image are equal in the colimit, proving injectivity. The resulting bijections are natural in $b$. We have proved the [canonical colimit presentation of a covariant set-valued functor](../../../../../canonical-colimit-presentation-of-a-covariant-set-valued-functor.md):

$$
\boxed{F\cong\operatorname{colim}_{(c,x)\in\mathcal E^{\mathrm{op}}}\mathcal C(c,-).}
$$

A [Cartesian closed category](../../../../../cartesian-closed-category.md) has finite [products in a category](../../../../../product-category-theory.md) and an [exponential object](../../../../../exponential-object.md) $H^G$ for each pair, representing maps from a product with $G$. In $[\mathcal C,\mathbf{Set}]$, the terminal functor and binary products are computed pointwise. Define the [exponential of covariant set-valued functors](../../../../../exponential-of-covariant-set-valued-functors.md) by

$$
(H^G)(c)=\operatorname{Nat}(\mathcal C(c,-)\times G,H).
$$

Smallness makes this a set. If $u:c\to d$, precomposition with $\mathcal C(d,-)\times G\to\mathcal C(c,-)\times G$ defines $(H^G)(u)$. Functoriality is immediate from associativity of composition. Its [evaluation map of an exponential object](../../../../../evaluation-map-of-an-exponential-object.md) is

$$
\operatorname{ev}_c(\tau,z)=\tau_c(1_c,z).
$$

For $u:c\to d$, naturality of $\tau$ shows $H(u)\tau_c(1_c,z)=\tau_d(u,G(u)z)$, which is exactly the naturality equation for evaluation.

Given $\theta:P\times G\to H$, define its [currying](../../../../../currying.md) at $p\in P(c)$ by

$$
(\widehat\theta_c(p))_b(f,z)=\theta_b(P(f)p,z),\qquad f:c\to b,\quad z\in G(b).
$$

Naturality of $\theta$ proves that this is a natural transformation in $b$, and its compatibility with arrows $c\to d$ proves that $\widehat\theta:P\to H^G$ is natural. Evaluation recovers $\theta$ by setting $f=1_c$. Conversely, for $\sigma:P\to H^G$, its naturality implies

$$
(\sigma_c(p))_b(f,z)=(\sigma_b(P(f)p))_b(1_b,z),
$$

so currying the evaluation composite recovers $\sigma$. These formulas give the required [natural bijection](../../../../../natural-bijection.md), hence **$[\mathcal C,\mathbf{Set}]$ is Cartesian closed**.

Finally, for every $F$ the small category $\mathcal E=\int F$ has a Cartesian closed functor category by the same construction. The slice equivalence above transports its terminal object, products and exponentials to $[\mathcal C,\mathbf{Set}]/F$. The original functor category also has pointwise finite limits. Therefore **it is locally Cartesian closed**. Every construction here is explicit; no adjoint functor theorem is used.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
