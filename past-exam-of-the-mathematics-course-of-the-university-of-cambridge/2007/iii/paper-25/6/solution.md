<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [monoidal category](../../../../../monoidal-category.md) consists of a [category](../../../../../category-split.md) $\mathcal C$, a bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a unit object $I$, and [natural isomorphisms](../../../../../natural-isomorphism.md)

$$
a_{X,Y,Z}:(X\otimes Y)\otimes Z\to X\otimes(Y\otimes Z),\quad
\lambda_X:I\otimes X\to X,\quad
\rho_X:X\otimes I\to X.
$$

The [associator](../../../../../associator.md) and [unitors](../../../../../unitor.md) satisfy the [pentagon identity for a monoidal category](../../../../../pentagon-identity-for-a-monoidal-category.md) and [triangle identity for a monoidal category](../../../../../triangle-identity-for-a-monoidal-category.md)

$$
\begin{aligned}
a_{W,X,Y\otimes Z}\,a_{W\otimes X,Y,Z}
&=(1_W\otimes a_{X,Y,Z})\,a_{W,X\otimes Y,Z}\,(a_{W,X,Y}\otimes1_Z),\\
(1_X\otimes\lambda_Y)a_{X,I,Y}&=\rho_X\otimes1_Y.
\end{aligned}
$$

All compositions here have the displayed parenthesized sources and targets; no strictness assumption is being made.

The [monoidal coherence theorem](../../../../../monoidal-coherence-theorem.md) says that between two formal tensor expressions having the same ordered list of letters after deletion of formal units, every map made from [associators](../../../../../associator.md), [unitors](../../../../../unitor.md), their inverses, identities, tensor [products in a category](../../../../../product-category-theory.md) and compositions is the same. Thus every diagram of such structural maps commutes. It does not permit permutation of letters or identify different additional maps such as braidings.

We prove this by canonical normalization. We first derive three necessary unit identities from the axioms, avoiding a circular appeal to coherence:

$$
\rho_{X\otimes Y}=(1_X\otimes\rho_Y)a_{X,Y,I},\qquad
\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y,\qquad
\lambda_I=\rho_I.
$$

For the first identity, take the pentagon on $X,Y,I,Z$ and postcompose by $1_X\otimes(1_Y\otimes\lambda_Z)$. [Naturality](../../../../../naturality.md) of $a$ and the triangle identify its left-hand path as $a_{X,Y,Z}(\rho_{X\otimes Y}\otimes1_Z)$; they identify its right-hand path as

$$
a_{X,Y,Z}\bigl(((1_X\otimes\rho_Y)a_{X,Y,I})\otimes1_Z\bigr).
$$

Cancel $a_{X,Y,Z}$. Taking $Z=I$ permits cancellation of the operation $-\otimes I$, since the [natural isomorphism](../../../../../natural-isomorphism.md) $\rho$ makes that [functor](../../../../../functor.md) faithful. This proves the first identity. The identical argument with tensor order reversed, [associator](../../../../../associator.md) reversed and left and right [unitors](../../../../../unitor.md) exchanged proves the second. Finally, [naturality](../../../../../naturality.md) of $\lambda$ at the map $\lambda_X:I\otimes X\to X$ gives $\lambda_{I\otimes X}=1_I\otimes\lambda_X$, after cancellation of $\lambda_X$. Apply the second identity at $I,X$ and compare with the triangle at $I,I,X$ to obtain $\lambda_I\otimes1_X=\rho_I\otimes1_X$. Set $X=I$ and use the same faithfulness to conclude $\lambda_I=\rho_I$. This establishes the [unit identities derived from the monoidal pentagon and triangle](../../../../../unit-identities-derived-from-the-monoidal-pentagon-and-triangle.md).

For an ordered word $u$, define a right-associated normal tensor, including a terminal unit, by

$$
N(\varnothing)=I,\qquad N(Au)=A\otimes N(u).
$$

Define canonical concatenation maps $c_{u,v}:N(u)\otimes N(v)\to N(uv)$ recursively:

$$
c_{\varnothing,v}=\lambda_{N(v)},\qquad
c_{Au,v}=(1_A\otimes c_{u,v})a_{A,N(u),N(v)}.
$$

All these maps are invertible. The derived unit identities give, by induction on $u$,

$$
c_{u,\varnothing}=\rho_{N(u)}.
$$

The empty base case is $\lambda_I=\rho_I$; the induction step is exactly the right-unitor identity above.

A second induction, again on $u$, proves the concatenation identity

$$
c_{uv,w}(c_{u,v}\otimes1_{N(w)})
=c_{u,vw}(1_{N(u)}\otimes c_{v,w})a_{N(u),N(v),N(w)}.
$$

For $u=\varnothing$, [naturality](../../../../../naturality.md) of $\lambda$ and $\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y$ give the equality. For $u=Au'$, expand each occurrence with first word beginning in $A$ by the recursive formula. [Naturality](../../../../../naturality.md) moves the maps $c_{u',v}$ and $c_{v,w}$ through the [associators](../../../../../associator.md). The two paths of [associators](../../../../../associator.md) on $A,N(u'),N(v),N(w)$ agree by the pentagon; the remaining maps inside the factor $A\otimes-$ agree by the induction hypothesis for $u'$. This proves the concatenation identity for every triple of words, including empty words.

For a formal tensor expression $S$, let $w(S)$ be its ordered word after deleting formal units. Define an isomorphism $\nu_S:S\to N(w(S))$ recursively by

$$
\nu_A=\rho_A^{-1},\qquad \nu_I=1_I,\qquad
\nu_{S\otimes T}=c_{w(S),w(T)}(\nu_S\otimes\nu_T).
$$

Here the first case means a formal letter $A$, and the second means the distinguished formal unit. Applying the concatenation identity and [naturality](../../../../../naturality.md) of $a$ gives

$$
\nu_{S\otimes(T\otimes U)}a_{S,T,U}=\nu_{(S\otimes T)\otimes U}.
$$

Similarly, [naturality](../../../../../naturality.md) of the [unitors](../../../../../unitor.md) and the two empty-word concatenation identities give

$$
\nu_S\lambda_S=\nu_{I\otimes S},\qquad
\nu_S\rho_S=\nu_{S\otimes I}.
$$

Thus normalization commutes with each generating [associator](../../../../../associator.md) or [unitor](../../../../../unitor.md). It also commutes with their inverses. The recursive tensor formula shows the same for a generating map applied inside any larger tensor expression, and composition preserves the property. Consequently every structural map $g:S\to T$ satisfies $\nu_Tg=\nu_S$, whence

$$
\boxed{g=\nu_T^{-1}\nu_S.}
$$

This depends only on the source and target expressions, so any two structural paths agree. That proves coherence, including all insertions and removals of units, by the [word normalization proof of monoidal coherence](../../../../../word-normalization-proof-of-monoidal-coherence.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
