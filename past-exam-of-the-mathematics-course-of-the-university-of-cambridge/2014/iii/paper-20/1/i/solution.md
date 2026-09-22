<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [comonad](../../../../../../comonad.md) as $(G,\epsilon,\delta)$ and its [category of coalgebras for a comonad](../../../../../../category-of-coalgebras-for-a-comonad.md) as $\mathcal E^G$. A [coalgebra for a comonad](../../../../../../coalgebra-for-a-comonad.md) is a map $a:A\to GA$ with $\epsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. A morphism $f:(A,a)\to(B,b)$ satisfies $bf=Gf\,a$. Let $U:\mathcal E^G\to\mathcal E$ be the [forgetful functor](../../../../../../forgetful-functor.md) and let $R(X)=(GX,\delta_X)$ be the [cofree coalgebra](../../../../../../cofree-coalgebra.md). The [adjunction](../../../../../../adjoint-functors.md) $U\dashv R$ has the explicit correspondence

$$
f:UA\to X\quad\longleftrightarrow\quad Gf\,a:A\to R(X).
$$

We construct the three pieces of the [elementary topos](../../../../../../elementary-topos.md) structure.

Because $G$ preserves [finite limits](../../../../../../finite-limit.md), each underlying finite limiting cone has a unique coalgebra structure induced by the structures on its vertices. The counit and coassociativity equations can be checked after its jointly monic projections. Thus $U$ creates [finite limits](../../../../../../finite-limit.md) and reflects isomorphisms. A morphism of coalgebras is monic exactly when its underlying morphism is monic, by the diagonal criterion using the created [pullback](../../../../../../pullback-category-theory.md).

For [exponentials in a coalgebra topos](../../../../../../exponentials-in-a-coalgebra-topos.md), fix coalgebras $(A,a)$ and $(B,b)$ and put $E=B^A$ in $\mathcal E$. On the cofree coalgebra $R(E)$ there is an underlying evaluation

$$
e:GE\times A\longrightarrow B,\qquad e=\operatorname{ev}(\epsilon_E\times1_A).
$$

The two maps

$$
b e,\qquad Ge\,(\delta_E\times a):GE\times A\longrightarrow GB
$$

use $G(GE\times A)\cong GGE\times GA$ in the second expression. Transpose them in $\mathcal E$ to maps $r,s:GE\rightrightarrows(GB)^A$, and then transpose across $U\dashv R$ to coalgebra morphisms $\widetilde r,\widetilde s:R(E)\rightrightarrows R((GB)^A)$. Take their [equalizer](../../../../../../equaliser.md) $C$ in $\mathcal E^G$.

An underlying map $UX\times A\to B$ corresponds to a coalgebra map $h:X\to R(E)$. The equation saying that the original map is a coalgebra morphism is precisely $rh=sh$, since $\delta_Eh=Gh\,x$ for the structure $x:X\to GX$. By the cofree adjunction, this is equivalent to $\widetilde rh=\widetilde sh$, hence to unique factorization through $C$. Therefore

$$
\mathcal E^G(X,C)\cong\mathcal E^G(X\times A,B),
$$

naturally in $X$. This constructs the required [exponential object](../../../../../../exponential-object.md).

For the [subobject classifier of a coalgebra topos](../../../../../../subobject-classifier-of-a-coalgebra-topos.md), let $\top:1\hookrightarrow\Omega$ be the underlying [subobject classifier](../../../../../../subobject-classifier.md), and let $\kappa:G\Omega\to\Omega$ classify the mono $G\top:G1\cong1\hookrightarrow G\Omega$. Its cofree transpose is the coalgebra endomorphism

$$
k=G\kappa\,\delta_\Omega:R\Omega\longrightarrow R\Omega.
$$

Define $\Omega_G$ as the [equalizer](../../../../../../equaliser.md) of $k$ and $1_{R\Omega}$. The transpose of $\top$ factors through this [equalizer](../../../../../../equaliser.md) and gives $\top_G:1\to\Omega_G$.

Indeed, for a [subobject](../../../../../../subobject.md) $S\hookrightarrow UX$ classified by $\chi:UX\to\Omega$, the [pullback](../../../../../../pullback-category-theory.md) $x^{-1}(GS)$ has characteristic map $\kappa G\chi\,x$. It is always contained in $S$, by naturality of the counit. Equality holds exactly when $x$ restricts to a coalgebra structure on $S$; its axioms then follow by composing with the [monomorphisms](../../../../../../monomorphism.md) $GS\hookrightarrow GX$ and $GGS\hookrightarrow GGX$. Under $U\dashv R$, the classifying map becomes $h=G\chi\,x:X\to R\Omega$. The equality of [subobjects](../../../../../../subobject.md) is $\epsilon_\Omega h=\kappa h$. Transposing this equality gives $h=kh$, so exactly the coalgebra [subobjects](../../../../../../subobject.md) correspond to maps $X\to\Omega_G$. Their [pullback](../../../../../../pullback-category-theory.md) of $\top_G$ is the desired subcoalgebra, and uniqueness follows from uniqueness of $\chi$.

Thus we have [finite limits](../../../../../../finite-limit.md), exponentials and a [subobject classifier](../../../../../../subobject-classifier.md):

$$
\boxed{\mathcal E^G\text{ is an elementary topos}.}
$$

The construction does not assume that $G$ preserves the underlying exponentials or underlying [subobject classifier](../../../../../../subobject-classifier.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
