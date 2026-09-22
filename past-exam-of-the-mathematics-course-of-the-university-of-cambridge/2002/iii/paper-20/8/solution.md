<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For $c\in\mathcal C$ and $d\in\mathcal D$, define maps of [hom-sets](../../../../../hom-set.md)

$$
\alpha(f)=Gf\,\eta_c:\mathcal D(Fc,d)\to\mathcal C(c,Gd),\qquad
\beta(g)=\varepsilon_dFg:\mathcal C(c,Gd)\to\mathcal D(Fc,d).
$$

They are natural in $c,d$, using [naturality](../../../../../naturality.md) of $\eta,\varepsilon$. The one supplied [triangle identity for an adjunction](../../../../../triangle-identities-for-an-adjunction.md) gives

$$
\alpha\beta(g)=G\varepsilon_d\,GFg\,\eta_c=G\varepsilon_d\,\eta_{Gd}g=g.
$$

[Naturality](../../../../../naturality.md) of $\varepsilon$ also gives

$$
\beta\alpha(f)=\varepsilon_dFGfF\eta_c=f\varepsilon_{Fc}F\eta_c=f e_c,
\qquad e_c=\varepsilon_{Fc}F\eta_c.
$$

Since $\alpha\beta=1$, the composite $\beta\alpha$ is idempotent. Evaluating its equation $(\beta\alpha)^2=\beta\alpha$ on $f=1_{Fc}$ gives $e_c^2=e_c$. As $e$ is a composite of [natural transformations](../../../../../natural-transformation.md), this proves that **$e$ is an idempotent in the [functor category](../../../../../functor-category.md)**, including the required [naturality](../../../../../naturality.md).

Suppose this [one-triangle adjunction idempotent](../../../../../one-triangle-adjunction-idempotent.md) splits as [natural transformations](../../../../../natural-transformation.md) $F\xrightarrow r H\xrightarrow i F$ with $ri=1_H$ and $ir=e$. The maps $h\mapsto hr$ and $f\mapsto fi$ give inverse [bijections](../../../../../bijection.md) between $\mathcal D(Hc,d)$ and the [subset](../../../../../subset.md) of $\mathcal D(Fc,d)$ consisting of maps with $fe_c=f$. Indeed $(hr)e_c=hrir=hr$, $(hr)i=h$, and $(fi)r=fe_c=f$. The maps $\alpha,\beta$ give inverse [bijections](../../../../../bijection.md) between that [subset](../../../../../subset.md) and $\mathcal C(c,Gd)$, since $\beta\alpha(f)=fe_c$ and $\alpha\beta=1$. Combining them gives the [natural bijection](../../../../../natural-bijection.md)

$$
\mathcal D(Hc,d)\cong\mathcal C(c,Gd),\qquad h\longmapsto G(hr)\eta_c,
$$

with inverse $g\mapsto\varepsilon_dF(g)i_c$. Hence $H\dashv G$. Its [adjunction unit](../../../../../unit-of-an-adjunction.md) is $Gr\,\eta$ and its [adjunction counit](../../../../../counit-of-an-adjunction.md) is $\varepsilon\,i_G$.

Conversely, suppose $H\dashv G$, with [natural bijection](../../../../../natural-bijection.md) $\theta:\mathcal D(Hc,d)\cong\mathcal C(c,Gd)$. Set $\tau=\theta^{-1}\alpha$ and $\sigma=\beta\theta$. Then $\tau\sigma=1$ and $\sigma\tau(f)=fe_c$. By the covariant [Yoneda lemma](../../../../../yoneda-lemma.md), the transformation $\tau:\mathcal D(Fc,-)\to\mathcal D(Hc,-)$ is precomposition with a unique [morphism](../../../../../morphism.md) $i_c:Hc\to Fc$, and $\sigma$ is precomposition with a unique [morphism](../../../../../morphism.md) $r_c:Fc\to Hc$. The equation $\tau\sigma=1$ evaluated at $1_{Hc}$ gives $r_ci_c=1_{Hc}$; the equation $\sigma\tau(f)=fe_c$ evaluated at $1_{Fc}$ gives $i_cr_c=e_c$. [Naturality](../../../../../naturality.md) in $c$ of $\tau,\sigma$ implies, again by the same [Yoneda lemma](../../../../../yoneda-lemma.md), that $i,r$ are [natural transformations](../../../../../natural-transformation.md). Thus they split $e$ in the whole [functor category](../../../../../functor-category.md), rather than merely at individual objects. We have proved

$$
\boxed{G\text{ has a left adjoint}\iff e=\varepsilon_FF\eta\text{ splits in }[\mathcal C,\mathcal D].}
$$

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
