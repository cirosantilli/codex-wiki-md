<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $F:\mathcal C\to\mathcal D$ be a [final functor](../../../../../final-functor.md), and let $\lambda_c:GFc\to V$ be a [cocone under a diagram](../../../../../cocone-under-a-diagram.md) $GF$. For $d\in\mathcal D$, choose an object $(c,a:d\to Fc)$ of the nonempty [comma category](../../../../../comma-category.md) $(d\downarrow F)$ and define

$$
\bar\lambda_d=\lambda_c\,G(a):Gd\to V.
$$

If $t:(c,a)\to(c',a')$ is a [morphism](../../../../../morphism.md) in that comma category, then $Ft\,a=a'$, so the cocone equation gives $\lambda_cG(a)=\lambda_{c'}G(Ft)G(a)=\lambda_{c'}G(a')$. Equality also holds along a reversed arrow, and hence along any zigzag. Connectedness makes the definition independent of the chosen object. For $v:d\to d'$, use $(c,a:d'\to Fc)$ and $(c,av:d\to Fc)$ to obtain $\bar\lambda_d=\bar\lambda_{d'}Gv$. Thus $\bar\lambda$ is a cocone under $G$. Taking $(c,1_{Fc})$ shows that it extends $\lambda$.

Every extension must satisfy $\bar\lambda_d=\lambda_cG(a)$ by its cocone equation, proving uniqueness. The construction commutes with postcomposition by a [morphism](../../../../../morphism.md) $V\to V'$. Hence restriction gives a natural bijection between the [sets](../../../../../set-split.md) of cocones of $G$ and $GF$ with any fixed vertex. A universal cocone for $GF$ therefore extends to a universal cocone for $G$. In particular,

$$
\boxed{\operatorname{colim}_{\mathcal D}G\cong\operatorname{colim}_{\mathcal C}GF,}
$$

whenever the latter exists, and existence of all [colimits](../../../../../colimit.md) of shape $\mathcal C$ implies existence of all colimits of shape $\mathcal D$.

For the factorization of an arbitrary [functor](../../../../../functor.md) $H:\mathcal C\to\mathcal E$, let

$$
P(e)=\pi_0(e\downarrow H),
$$

the [set](../../../../../set-split.md) of [connected components of a category](../../../../../connected-component-of-a-category.md), where components are defined by finite zigzags. Precomposition by $v:e\to e'$ gives a [functor](../../../../../functor.md) $(e'\downarrow H)\to(e\downarrow H)$ and therefore a map $P(v):P(e')\to P(e)$. Identity and composition laws make $P$ a [categorical presheaf](../../../../../presheaf-category-theory.md). This is a set-valued construction when the relevant comma categories are small or have only a set of components, as in the usual small-category convention for this factorization.

Take $\mathcal D$ to be the [category of elements](../../../../../category-of-elements.md) of this presheaf. Its objects are pairs $(e,S)$ with $S\in P(e)$; a morphism $(e,S)\to(e',S')$ is an arrow $v:e\to e'$ satisfying $P(v)(S')=S$. Define $G:\mathcal D\to\mathcal E$ by forgetting $S$. Given $v:e\to e'$ and an object $(e',S')$, the unique lift into that object has source $(e,P(v)(S'))$ and underlying arrow $v$. This proves that $G$ is a [discrete fibration](../../../../../discrete-fibration.md).

Define $F(c)=(Hc,[(c,1_{Hc})])$. For $t:c\to c'$, take $F(t)=Ht$. The arrow $t$ in $(Hc\downarrow H)$ joins $(c,1_{Hc})$ to $(c',Ht)$, so the required component equation holds. It follows that $F$ is a functor and $GF=H$.

Finally, an object of $((e,S)\downarrow F)$ is a pair $(c,v:e\to Hc)$ whose component in $(e\downarrow H)$ is $S$. Its morphisms are exactly the morphisms of that comma category between objects in $S$. Consequently $((e,S)\downarrow F)$ is precisely the full connected component $S$, and is nonempty and connected. Thus $F$ is final, and **every such functor factors as a final functor followed by a discrete fibration**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
