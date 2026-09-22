<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) says that, for a [functor](../../../../../functor.md) $U:\mathcal A\to\mathcal B$ between [locally small categories](../../../../../locally-small-category.md), with $\mathcal A$ a [complete category](../../../../../complete-category.md), **$U$ has a left adjoint if and only if it preserves small limits and satisfies the solution-set condition**. The [solution-set condition](../../../../../solution-set-condition.md) means that for each $B\in\mathcal B$ there is a [set](../../../../../set-split.md) of arrows $b_i:B\to UA_i$ such that every $b:B\to UA$ factors as $U(a)b_i$ for some $i$ and some $a:A_i\to A$.

Here is the smallness argument behind the theorem. A [complete category](../../../../../complete-category.md) that is [locally small](../../../../../locally-small-category.md) and has a [weakly initial set](../../../../../weakly-initial-set.md) $(W_i)$ has an [initial object](../../../../../initial-object.md). Form the [product in a category](../../../../../product-category-theory.md) $W=\prod_iW_i$. It is weakly initial, since a projection $W\to W_i$ followed by a chosen arrow $W_i\to X$ gives an arrow $W\to X$. Take the simultaneous [equalizer](../../../../../equaliser.md) $e:E\to W$ of all [endomorphisms](../../../../../endomorphism.md) of $W$ with $1_W$; the family is a [set](../../../../../set-split.md) by local smallness. The object $E$ is also weakly initial. For parallel arrows $a,b:E\rightrightarrows X$, take their [equalizer](../../../../../equaliser.md) $j:Y\to E$ and a map $t:W\to Y$. Since $ejt$ is an [endomorphism](../../../../../endomorphism.md) of $W$, the defining property of $e$ gives $ejte=e$. Cancellation of the [monomorphism](../../../../../monomorphism.md) $e$ gives $jte=1_E$. Thus the [monomorphism](../../../../../monomorphism.md) $j$ has a right inverse and is an [isomorphism](../../../../../isomorphism.md), so $a=b$. Existence of arrows out of $E$ was already established, proving the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md).

If $U$ preserves small [categorical limits](../../../../../categorical-limit.md), the [comma category](../../../../../comma-category.md) $(B\downarrow U)$ is complete: take the limiting object in $\mathcal A$, and use preservation to assemble the arrows from $B$. It is [locally small](../../../../../locally-small-category.md), and the [solution-set condition](../../../../../solution-set-condition.md) provides a [weakly initial set](../../../../../weakly-initial-set.md). Its [initial object](../../../../../initial-object.md) is an arrow $\eta_B:B\to ULB$ with a natural bijection

$$
\mathcal A(LB,A)\cong\mathcal B(B,UA).
$$

For a [morphism](../../../../../morphism.md) $v:B\to B'$, define $Lv$ by $U(Lv)\eta_B=\eta_{B'}v$. Uniqueness proves functoriality and naturality, giving a [left adjoint](../../../../../adjoint-functors.md) $L\dashv U$. Conversely, a [right adjoint](../../../../../adjoint-functors.md) preserves [categorical limits](../../../../../categorical-limit.md), because applying the [adjunction](../../../../../adjoint-functors.md) converts a limiting [cone over a diagram](../../../../../cone-over-a-diagram.md) into the corresponding limiting cone of [hom-sets](../../../../../hom-set.md). Its [adjunction unit](../../../../../unit-of-an-adjunction.md) at $B$ is a singleton solution set. This proves both directions of the [general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md).

Apply it to the inclusion $J:\mathbf{KHaus}\hookrightarrow\mathbf{Top}$, where $\mathbf{KHaus}$ is the [full subcategory](../../../../../full-subcategory.md) of [compact Hausdorff spaces](../../../../../compact-hausdorff-space.md). A small [product in a category](../../../../../product-category-theory.md) of [compact Hausdorff spaces](../../../../../compact-hausdorff-space.md) is again compact Hausdorff by the [Tychonoff theorem](../../../../../tychonoff-s-theorem.md). An [equalizer](../../../../../equaliser.md) of two [continuous functions](../../../../../continuous-function.md) into a [Hausdorff space](../../../../../hausdorff-space.md) is closed, hence compact Hausdorff. Products and equalizers construct all small [categorical limits](../../../../../categorical-limit.md), and the inclusion preserves these constructions. Both [categories](../../../../../category-split.md) are [locally small](../../../../../locally-small-category.md).

Fix a [topological space](../../../../../topological-space.md) $X$ and a [continuous function](../../../../../continuous-function.md) $f:X\to K$ into a [compact Hausdorff space](../../../../../compact-hausdorff-space.md). The [closure](../../../../../closure-topology.md) $K_f=\overline{f(X)}$ is compact Hausdorff and has a [dense subset](../../../../../dense-set.md) of [cardinality](../../../../../cardinality.md) at most $|X|$. The permitted cardinal estimate gives

$$
|K_f|\leq 2^{2^{|X|}}.
$$

For $X=\varnothing$, use $K_f=\varnothing$. Choose a [set](../../../../../set-split.md) of representatives of all compact Hausdorff topologies on underlying sets of cardinality at most this bound, and all [continuous functions](../../../../../continuous-function.md) from $X$ to those representatives. Every $f$ factors through one of them, using the inclusion $K_f\hookrightarrow K$. This is the [solution-set condition](../../../../../solution-set-condition.md). Consequently **the inclusion of compact Hausdorff spaces has a left adjoint**, the [compact Hausdorff reflection](../../../../../compact-hausdorff-reflection.md):

$$
\boxed{\mathbf{KHaus}(RX,K)\cong\mathbf{Top}(X,JK).}
$$

The universal arrow $X\to RX$ has [dense](../../../../../dense-set.md) image: factoring it through its closed image and applying uniqueness supplies an inverse to that image inclusion. It need not be an embedding when $X$ is not sufficiently separated; the assertion is a [compact Hausdorff reflection](../../../../../compact-hausdorff-reflection.md), rather than a claim that every [topological space](../../../../../topological-space.md) embeds in a compact Hausdorff space.

For completeness, the alternative [Special adjoint functor theorem](../../../../../special-adjoint-functor-theorem.md) can be proved from the same initial-object argument. Its limit form assumes that $\mathcal A$ is complete, locally small and [well-powered](../../../../../well-powered-category.md), with a [small cogenerating family](../../../../../cogenerating-set.md) $(Q_i)_{i\in I}$; then $U:\mathcal A\to\mathcal B$, with $\mathcal B$ locally small, has a [left adjoint](../../../../../adjoint-functors.md) precisely when it preserves small limits. To prove sufficiency, start with $b:B\to UA$ and intersect all [subobjects](../../../../../subobject.md) $M\hookrightarrow A$ through which $b$ factors after applying $U$. Well-poweredness makes this a small [intersection of subobjects](../../../../../intersection-of-subobjects.md), and preservation of limits gives a smallest supporting object $(M,b_M)$. For maps $s,t:M\rightrightarrows Q_i$, equality $U(s)b_M=U(t)b_M$ makes their [equalizer](../../../../../equaliser.md) another supporting subobject. Minimality forces that equalizer to be invertible, so $s=t$. Therefore

$$
\mathcal A(M,Q_i)\hookrightarrow\mathcal B(B,UQ_i),\qquad s\longmapsto U(s)b_M
$$

is an [injective function](../../../../../injective-function.md). The [evaluation embedding into cogenerator products](../../../../../evaluation-embedding-into-cogenerator-products.md) embeds $M$ in $\prod_iQ_i^{S_i}$, where $S_i$ is the realized subset of the fixed [set](../../../../../set-split.md) $\mathcal B(B,UQ_i)$. There are only a set of choices of these subsets, only a set of subobjects of each resulting product, and only a set of arrows from $B$ to each $U$-image. They give a solution set, so the already proved [general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) applies. Necessity is again preservation of limits by a right adjoint. For $\mathbf{KHaus}$, [monomorphisms](../../../../../monomorphism.md) are embeddings onto closed subspaces, and $[0,1]$ is a [coseparator](../../../../../coseparator.md) because [continuous functions](../../../../../continuous-function.md) to it separate points. Thus the [Special adjoint functor theorem](../../../../../special-adjoint-functor-theorem.md) gives the same reflection directly.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
