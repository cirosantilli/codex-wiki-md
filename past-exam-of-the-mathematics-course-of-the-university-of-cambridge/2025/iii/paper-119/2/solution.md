<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $F:\mathcal C\rightleftarrows\mathcal D:G$ with $F\dashv G$, the [unit and counit of an adjunction](../../../../../unit-and-counit-of-an-adjunction.md) are

$$
\eta:1_{\mathcal C}\to GF,
\qquad
\varepsilon:FG\to1_{\mathcal D},
$$

obtained by transposing identity morphisms. They satisfy the triangular identities $\varepsilon_FF\eta=1_F$ and $G\varepsilon\eta_G=1_G$.

If $G$ is [full and faithful](../../../../../full-and-faithful-functor.md), fullness gives a map $u:B\to FGB$ with $G(u)=\eta_{GB}$; the second triangular identity and faithfulness show that $u$ is inverse to $\varepsilon_B$. Conversely, if $\varepsilon$ is an isomorphism, then for $h:GB\to GB'$ the unique arrow whose transpose is $h$ is

$$
B\xrightarrow{\varepsilon_B^{-1}}FGB\xrightarrow{Fh}FGB'\xrightarrow{\varepsilon_{B'}}B',
$$

which proves that $G$ is full, and the triangular identities prove faithfulness. Hence (i) and (ii) are equivalent. Condition (ii) immediately gives (iii). Conversely, a natural isomorphism $FG\cong1_{\mathcal D}$ combines with the adjunction bijection to show naturally that $\mathcal D(B,B')\to\mathcal C(GB,GB')$ is bijective; by naturality and the triangular identities this is the map induced by $G$ up to invertible natural conjugation, so $G$ is full and faithful. Thus all three conditions are equivalent.

Suppose $L\dashv F\dashv R$. If $L$ is full and faithful, the unit $1\to FL$ is an isomorphism. For $A,B$ in the codomain of $F$, the two adjunctions then give natural bijections

$$
\mathcal D(A,FRB)
\cong\mathcal C(LA,RB)
\cong\mathcal D(FLA,B)
\cong\mathcal D(A,B).
$$

By the [Yoneda lemma](../../../../../yoneda-lemma.md), the counit $FRB\to B$ is an isomorphism, so the [fully faithful adjoint criterion](../../../../../fully-faithful-adjoint-criterion.md) makes $R$ full and faithful. The converse is dual.

Now assume $F$ is full and faithful. For $L\dashv F$, its counit $\epsilon:LF\to1$ is invertible; for $F\dashv R$, its unit $\alpha:1\to RF$ is invertible. Define

$$
\theta=(\alpha_L)^{-1}R\eta:R\longrightarrow L.
$$

Applying $F$, then using naturality and the triangular identities, reduces this composite to the same map as

$$
R\xrightarrow{(\epsilon_R)^{-1}}LFR\xrightarrow{L\beta}L.
$$

Since $F$ is faithful, the two displayed composites are equal.

For a morphism $u:FB\to A$, let $\widehat u=Ru\,\alpha_B:B\to RA$ be its transpose under $F\dashv R$. The identities just proved give

$$
\theta_A\widehat u=Lu\,\epsilon_B^{-1}.
$$

If every $\theta_A$ is monic and $Lu=Lv$, this equation gives $\widehat u=\widehat v$, hence $u=v$; thus $L$ is faithful on arrows whose domains are in the image of $F$. Conversely, if $\theta_Af=\theta_Ag$ for $f,g:B\to RA$, naturality of $\epsilon$ and the second formula for $\theta$ give

$$
L(\beta_A Ff)=L(\beta_A Fg).
$$

Both maps have domain $FB$, so the assumed faithfulness gives $\beta_AFf=\beta_AFg$. These are the transposes of $f$ and $g$, hence $f=g$. Therefore $\theta$ is pointwise monic exactly under the stated faithfulness condition.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
