<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the length of a formal tensor expression recursively by

$$
|I|=0,\qquad |x|=1,\qquad |u\otimes v|=|u|+|v|.
$$

The canonical [strict monoidal functor](../../../../../../strict-monoidal-functor.md) $Q:\mathcal Fbr\to\mathbf B$ sends $u$ to $|u|$, sends every [associator](../../../../../../associator.md) and [unitor](../../../../../../unitor.md) to an identity braid, and sends $c_{u,v}$ to the block [braiding](../../../../../../braiding.md) $c_{|u|,|v|}$. The pentagon and triangle become identity equations; the [braiding](../../../../../../braiding.md) axioms become the corresponding block-braid equations. Thus the assignment respects the defining relations, and

$$
Q(u\otimes v)=Qu+Qv,\qquad QI=0
$$

on the nose. It is a [braided monoidal functor](../../../../../../braided-monoidal-functor.md) with identity comparison maps.

To prove that $Q$ is an [equivalence of categories](../../../../../../equivalence-of-categories.md), choose a standard parenthesization $x^{[n]}$ of $n$ copies of $x$, with $x^{[0]}=I$. On $x^{[n]}$, define the image of $\sigma_i$ by canonically exposing the $i$th and $(i+1)$st factors, applying $c_{x,x}$ there, and restoring the chosen parentheses. The [monoidal coherence theorem](../../../../../../monoidal-coherence-theorem.md) makes this independent of the structural rebracketing. Crossings on disjoint pairs commute by the tensor interchange law. The adjacent [braid group relations](../../../../../../braid-group-relations.md) follows from the hexagon laws and [naturality](../../../../../../naturality.md) of the [braiding](../../../../../../braiding.md), as in the Yang–Baxter calculation below. Hence these assignments give [group homomorphisms](../../../../../../group-homomorphism.md) $B_n\to\operatorname{Aut}(x^{[n]})$ and a [functor](../../../../../../functor.md) $S:\mathbf B\to\mathcal Fbr$.

Equip $S$ with the canonical rebracketing maps $x^{[m]}\otimes x^{[n]}\to x^{[m+n]}$. Their [monoidal functor](../../../../../../monoidal-functor.md) axioms follow from the [monoidal coherence theorem](../../../../../../monoidal-coherence-theorem.md); the block-braiding compatibility follows by iterating the two hexagon laws. Therefore $S$ is a [strong monoidal functor](../../../../../../strong-monoidal-functor.md) compatible with the [braiding](../../../../../../braiding.md).

We have $QS=1_{\mathbf B}$, including its comparison maps. For every formal expression $u$, there is a canonical structural isomorphism

$$
\theta_u:x^{[|u|]}\longrightarrow u
$$

obtained by rebracketing and inserting the units appearing in $u$. These maps form a [natural isomorphism](../../../../../../natural-isomorphism.md) $SQ\Rightarrow1_{\mathcal Fbr}$. To check [naturality](../../../../../../naturality.md), it suffices to check the generating [morphisms](../../../../../../morphism.md): for [associators](../../../../../../associator.md) and [unitors](../../../../../../unitor.md) it is exactly [monoidal coherence](../../../../../../monoidal-coherence-theorem.md); for $c_{u,v}$ it follows from the hexagon expansion into the elementary crossings defining $S$. Composition and tensor product then preserve the equation. The same structural coherence shows that $\theta$ is monoidal.

**Thus $Q$ has a specified quasi-inverse and is the required equivalence:**

$$
\boxed{Q:\mathcal Fbr\simeq\mathbf B\quad\text{is braided and strict monoidal}.}
$$

Only ordinary [monoidal coherence](../../../../../../monoidal-coherence-theorem.md), together with the defining [braiding](../../../../../../braiding.md) axioms, has been used; a separate braided coherence theorem is unnecessary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
