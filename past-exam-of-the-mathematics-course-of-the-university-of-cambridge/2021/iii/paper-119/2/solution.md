<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an [adjoint functor](../../../../../adjoint-functors.md) pair $F:\mathcal D\rightleftarrows\mathcal C:G$, the [unit and counit of an adjunction](../../../../../unit-and-counit-of-an-adjunction.md) are

$$
\eta:1_{\mathcal D}\Rightarrow GF,
\qquad
\varepsilon:FG\Rightarrow1_{\mathcal C}.
$$

Under the adjunction bijection, $\eta_A$ corresponds to $1_{FA}$ and $\varepsilon_B$ corresponds to $1_{GB}$. They satisfy the triangle identities

$$
\varepsilon_{FA}F(\eta_A)=1_{FA},
\qquad
G(\varepsilon_B)\eta_{GB}=1_{GB}.
$$

Conversely, natural transformations with these identities recover the adjunction through the mutually inverse maps

$$
f:FA\to B\longmapsto G(f)\eta_A,
\qquad
g:A\to GB\longmapsto\varepsilon_BF(g).
$$

The [fully faithful adjoint criterion](../../../../../fully-faithful-adjoint-criterion.md) gives the first equivalence directly. If $F$ is [full and faithful](../../../../../full-and-faithful-functor.md), there is a unique $r_A:GFA\to A$ with $F(r_A)=\varepsilon_{FA}$; the triangle identity and faithfulness show that $r_A$ and $\eta_A$ are inverse, so the unit is an isomorphism. If the unit is an isomorphism, the displayed adjunction bijection shows that

$$
\mathcal D(A,A')\longrightarrow\mathcal C(FA,FA')
$$

is bijective, so $F$ is full and faithful. This also proves that either condition gives a natural isomorphism $GF\cong1_{\mathcal D}$.

For the remaining direction, suppose merely that $GF$ is naturally isomorphic to the identity. Transport the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md) along this isomorphism. Its underlying endofunctor is then the identity, its unit is a natural endomorphism $u:1\Rightarrow1$, and its multiplication is a natural endomorphism $m:1\Rightarrow1$ with $mu=1$. Naturality makes $u_A$ commute with $m_A$, so also $um=1$. Hence the transported unit, and therefore $\eta$, is an isomorphism. The three conditions are equivalent.

Now let $F\dashv G\dashv H$. If $F$ is full and faithful, then $GF\cong1_{\mathcal D}$. For $A,B\in\mathcal D$, the two adjunctions give natural bijections

$$
\mathcal D(B,GHA)
\cong\mathcal C(FB,HA)
\cong\mathcal D(GFB,A)
\cong\mathcal D(B,A).
$$

The [Yoneda lemma](../../../../../yoneda-lemma.md) therefore gives $GHA\cong A$, naturally in $A$. The [fully faithful adjoint criterion](../../../../../fully-faithful-adjoint-criterion.md) applied to $G\dashv H$ shows that $H$ is full and faithful. Conversely, if $H$ is full and faithful, then $GH\cong1_{\mathcal D}$ and

$$
\mathcal D(GFA,B)
\cong\mathcal C(FA,HB)
\cong\mathcal D(A,GHB)
\cong\mathcal D(A,B).
$$

Another application of the [Yoneda lemma](../../../../../yoneda-lemma.md) gives $GFA\cong A$, so $F$ is full and faithful. Thus $F$ is full and faithful exactly when $H$ is.

Assume henceforth that $G$ is full and faithful. Then the counit $\varepsilon:FG\to1_{\mathcal C}$ and unit $\alpha:1_{\mathcal C}\to HG$ are natural isomorphisms. Consider

$$
\theta_1=(\alpha F)^{-1}(H\eta),
\qquad
\theta_2=(F\beta)(\varepsilon H)^{-1}:H\Rightarrow F.
$$

Applying the faithful functor $G$, then using naturality and the four triangle identities, turns both composites into

$$
GH\xrightarrow{\beta}1_{\mathcal D}\xrightarrow{\eta}GF.
$$

Therefore $\theta_1=\theta_2$; denote their common value by $\theta$, the [double-adjoint comparison transformation](../../../../../double-adjoint-comparison-transformation.md).

The pointwise monicity criterion is clearest from the following natural square, in which both vertical maps are bijections:

$$
\begin{array}{ccc}
\mathcal C(B,HA)&\xrightarrow{\theta_A\circ-}&\mathcal C(B,FA)\\
\downarrow&&\downarrow\\
\mathcal D(GB,A)&\xrightarrow{F}&\mathcal C(FGB,FA).
\end{array}
$$

The left vertical map is the adjunction $G\dashv H$, while the right one precomposes with the isomorphism $\varepsilon_B:FGB\to B$. Thus every $\theta_A$ is a [monomorphism](../../../../../monomorphism.md) exactly when $F$ is faithful on all morphisms $GB\to A$, namely morphisms whose domains lie in the image of $G$.

Dually, the natural square

$$
\begin{array}{ccc}
\mathcal C(FA,B)&\xrightarrow{-\circ\theta_A}&\mathcal C(HA,B)\\
\downarrow&&\downarrow\\
\mathcal D(A,GB)&\xrightarrow{H}&\mathcal C(HA,HGB)
\end{array}
$$

has bijective vertical maps, using $F\dashv G$ on the left and the isomorphism $\alpha_B:B\to HGB$ on the right. Hence every $\theta_A$ is an [epimorphism](../../../../../epimorphism.md) exactly when $H$ is faithful on all morphisms $A\to GB$, namely morphisms whose codomains lie in the image of $G$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
