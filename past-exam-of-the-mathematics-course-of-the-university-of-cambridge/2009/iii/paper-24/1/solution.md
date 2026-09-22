<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the elementary, or weak, [topos](../../../../../elementary-topos.md) axioms: [finite limits](../../../../../finite-limit.md) and a [power object](../../../../../power-object.md) $PA$ for every object $A$, naturally representing $\operatorname{Sub}(A\times X)$. No arbitrary products or coproducts are assumed. In particular $\Omega=P1$ is the [subobject classifier](../../../../../subobject-classifier.md). Inverse image of the membership relation defines $Pf:PB\to PA$ for $f:A\to B$.

Interchanging the factors in a relation gives natural bijections

$$
\mathcal E(A,PB)\cong\operatorname{Sub}(A\times B)\cong\mathcal E(B,PA).
$$

Thus the [contravariant power-object functor](../../../../../contravariant-power-object-functor.md) $P:\mathcal E^{\mathrm{op}}\to\mathcal E$ has left adjoint $P^{\mathrm{op}}$. Its [adjunction unit](../../../../../unit-of-an-adjunction.md) $\eta_A:A\to PPA$ sends a generalized element $a$ to the predicate on $PA$ given by membership of $a$.

This unit is monic. If $x,y:T\to A$ have the same image under $\eta_A$, membership of $x$ and $y$ agrees in every $T$-parameterized [subobject](../../../../../subobject.md) of $A$. Apply this to the graph of $x$ in $A\times T$: membership of $x$ is true, so membership of $y$ is true, which means $y=x$. This argument uses parameterized relations, not an assumption that global elements detect morphisms.

The [functor](../../../../../functor.md) $P$ reflects isomorphisms. Suppose $Pf$ is invertible. Then $PPf$ is invertible, and naturality $PPf\,\eta_A=\eta_Bf$ together with monicity of $\eta_A$ shows that $f$ is monic. Regard $f$ as a [subobject](../../../../../subobject.md) of $B$. Its inverse image along itself is the whole of $A$, just as for the whole [subobject](../../../../../subobject.md) of $B$. Those two [subobjects](../../../../../subobject.md) correspond to maps $1\to PB$; since $Pf$ is monic, they coincide. Therefore the [subobject](../../../../../subobject.md) $f$ is all of $B$, and $f$ is an isomorphism.

We now prove the preservation condition for the [crude monadicity theorem](../../../../../crude-monadicity-theorem.md). A [reflexive pair](../../../../../reflexive-pair.md) in $\mathcal E^{\mathrm{op}}$ is a [coreflexive pair](../../../../../coreflexive-pair.md) $f,g:B\rightrightarrows A$ in $\mathcal E$, with $rf=rg=1_B$ for some $r:A\to B$. Let $e:E\hookrightarrow B$ be its [equalizer](../../../../../equaliser.md). For any [monomorphism](../../../../../monomorphism.md) $m$, define $\exists_m$ on [power objects](../../../../../power-object.md) by composing a parameterized [subobject](../../../../../subobject.md) with $m$; no general image construction is needed because $m$ is monic. Inverse image followed by this extension obeys $Pm\,\exists_m=1$.

Here both $f,g$ are monic. For a parameterized [subobject](../../../../../subobject.md) $S$ of $B$, an element $b$ belongs to $g^{-1}(f(S))$ exactly when $gb=fb'$ for some $b'\in S$. Applying $r$ gives $b=b'$, so this condition is precisely $b\in S$ and $fb=gb$. Consequently, as morphisms of [power objects](../../../../../power-object.md),

$$
Pf\,\exists_f=1_{PB},\qquad Pg\,\exists_f=\exists_e Pe,\qquad Pe\,\exists_e=1_{PE}.
$$

If $h:PB\to Z$ equalizes $Pf,Pg$, these identities give

$$
h=hPf\,\exists_f=hPg\,\exists_f=h\exists_e Pe.
$$

It therefore factors uniquely through $Pe$, which is a split [epimorphism](../../../../../epimorphism.md) with section $\exists_e$. Since $fe=ge$, $Pe$ also equalizes $Pf,Pg$. Hence $Pe$ is their [coequalizer](../../../../../coequalizer.md). This proves explicitly that [power objects turn coreflexive equalizers into coequalizers](../../../../../power-objects-turn-coreflexive-equalizers-into-coequalizers.md).

Finite [equalizers](../../../../../equaliser.md) in $\mathcal E$ give all [coequalizers](../../../../../coequalizer.md) of reflexive pairs in $\mathcal E^{\mathrm{op}}$, and we have shown that $P$ preserves them and reflects isomorphisms. The [crude monadicity theorem](../../../../../crude-monadicity-theorem.md) now yields

$$
\boxed{P\text{ is monadic},\qquad\mathcal E^{\mathrm{op}}\simeq\mathcal E^{PP}.}
$$

Fix a set $I$ of cardinality $\kappa$. If $\mathcal E$ has $I$-indexed [products in a category](../../../../../product-category-theory.md), its [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) for the double-power [monad](../../../../../monad.md) has them, since the forgetful [functor](../../../../../functor.md) creates existing limits. The displayed equivalence then gives $I$-products in $\mathcal E^{\mathrm{op}}$, hence $I$-[coproducts in a category](../../../../../coproduct.md) in $\mathcal E$.

For the converse, suppose those coproducts exist. The diagonal $\Delta:\mathcal E\to\mathcal E^I$ is a [logical functor](../../../../../logical-functor.md), because all the elementary topos structure in $\mathcal E^I$ is pointwise, and it has left adjoint $\coprod_I$. Apply [power-object monadicity](../../../../../power-object-monadicity.md) to both toposes. Under their monadic identifications, $\Delta^{\mathrm{op}}$ is the lift of $\Delta$ to the double-power [Eilenberg-Moore categories](../../../../../eilenberg-moore-category.md). The base [functor](../../../../../functor.md) $\Delta$ is a right adjoint to $\coprod_I$, so the [adjoint lifting theorem for monad algebra functors](../../../../../adjoint-lifting-theorem-for-monad-algebra-functors.md) gives a left adjoint to its algebra lift. Its required reflexive [coequalizers](../../../../../coequalizer.md) exist in $\mathcal E^{\mathrm{op}}$, since they are opposites of finite [equalizers](../../../../../equaliser.md) in $\mathcal E$. Taking opposites gives a right adjoint to $\Delta$, which is exactly the $I$-product [functor](../../../../../functor.md). Thus the [products and coproducts of fixed cardinality in a topos](../../../../../products-and-coproducts-of-fixed-cardinality-in-a-topos.md) satisfy

$$
\boxed{\mathcal E\text{ has }\kappa\text{-products}\iff\mathcal E\text{ has }\kappa\text{-coproducts}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
