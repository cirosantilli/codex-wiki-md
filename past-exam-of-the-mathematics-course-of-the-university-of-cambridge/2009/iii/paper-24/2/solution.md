<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $(G,\varepsilon,\delta)$ be a [Cartesian comonad](../../../../../cartesian-comonad.md), so its endofunctor preserves [finite limits](../../../../../finite-limit.md). A [coalgebra for a comonad](../../../../../coalgebra-for-a-comonad.md) is $(A,a)$ with $a:A\to GA$, $\varepsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. Its morphisms satisfy $bf=Gf\,a$. Write $U:\mathcal E^G\to\mathcal E$ for the [forgetful functor](../../../../../forgetful-functor.md) and $R(X)=(GX,\delta_X)$ for the [cofree coalgebra](../../../../../cofree-coalgebra.md). Transposition is

$$
\mathcal E^G((A,a),R(X))\cong\mathcal E(A,X),\qquad f\longmapsto\varepsilon_X f,\quad h\longmapsto Gh\,a.
$$

The [forgetful functor](../../../../../forgetful-functor.md) creates [finite limits](../../../../../finite-limit.md), since $G$ preserves them. We construct both [exponential objects](../../../../../exponential-object.md) and the [subobject classifier](../../../../../subobject-classifier.md).

For coalgebras $(A,a),(B,b)$, set $D=B^A$ and $W=(GB)^A$ in the ambient [topos](../../../../../elementary-topos.md). Define $p,q:GD\to W$ by transposing

$$
p^\flat=b\,\operatorname{ev}(\varepsilon_D\times1_A),\qquad q^\flat=G\operatorname{ev}(1_{GD}\times a),
$$

where $GD\times GA\cong G(D\times A)$. Their cofree transposes are coalgebra morphisms

$$
\widehat p=Gp\,\delta_D,\quad\widehat q=Gq\,\delta_D:R(D)\rightrightarrows R(W).
$$

Let $H$ be their coalgebra [equalizer](../../../../../equaliser.md). For a coalgebra $(C,c)$, an arrow $C\to R(D)$ corresponds to a map $h:C\times A\to B$. Its evaluation respects coalgebra structure exactly when

$$
bh=Gh\,(c\times a).
$$

Under the displayed transpositions this is precisely the condition that it equalize $\widehat p,\widehat q$. Thus $\mathcal E^G(C,H)\cong\mathcal E^G(C\times A,B)$ naturally, and $H$ is the required [exponential in a coalgebra topos](../../../../../exponentials-in-a-coalgebra-topos.md).

Let $\kappa:G\Omega\to\Omega$ classify $G\top:G1\cong1\hookrightarrow G\Omega$. In $R(\Omega)$ take the [equalizer](../../../../../equaliser.md)

$$
\Omega_G\hookrightarrow R(\Omega)\mathrel{\substack{\xrightarrow{1}\\[-2pt]\xrightarrow[G\kappa\,\delta_\Omega]{}}}R(\Omega).
$$

The truth map into $R(\Omega)$ is $G\top$ and factors through this [equalizer](../../../../../equaliser.md). To verify its universal property, take an underlying [subobject](../../../../../subobject.md) $m:S\hookrightarrow A$ of a coalgebra. It carries a compatible coalgebra structure exactly when $a$ maps $S$ into $GS$. Such a structure, if it exists, is unique because $Gm$ is monic; its laws follow by cancellation of $m,Gm,G^2m$. Moreover $a^{-1}(GS)\subseteq S$ always: applying $\varepsilon_A$ to a point of $GS$ lands in $S$. Thus stability is equivalent to $S=a^{-1}(GS)$.

If $\chi:A\to\Omega$ classifies $S$, this last equality is exactly

$$
\chi=\kappa G\chi\,a.
$$

The cofree transpose $\widehat\chi=G\chi\,a:A\to R(\Omega)$ satisfies this equation precisely when it factors through $\Omega_G$. Indeed transposing the equality $\widehat\chi=G\kappa\,\delta_\Omega\widehat\chi$ gives the equation above. Pulling back its truth map recovers $S$, because $\kappa$ classifies $G\top$. Hence $\Omega_G$ is the [subobject classifier of a coalgebra topos](../../../../../subobject-classifier-of-a-coalgebra-topos.md). We have obtained [finite limits](../../../../../finite-limit.md), exponentials and a classifier, proving **$\mathcal E^G$ is a topos**.

Now let $f:\mathcal H\to\mathcal E$ be a [geometric morphism](../../../../../geometric-morphism.md), and put $L=f^*$, $V=f_*$, with unit $\eta$. Both [functors](../../../../../functor.md) preserve [finite limits](../../../../../finite-limit.md), so $G=LV$ is a [Cartesian comonad](../../../../../cartesian-comonad.md) on $\mathcal H$. Put $\mathcal D=\mathcal H^G$. Its comparison [functor](../../../../../functor.md)

$$
K:\mathcal E\longrightarrow\mathcal D,\qquad K(X)=(LX,L\eta_X)
$$

is left exact and has right adjoint

$$
J(A,a)=\operatorname{Eq}\bigl(Va,\eta_{VA}:VA\rightrightarrows V L V A\bigr).
$$

To check the adjunction, transpose an underlying map $LX\to A$ to $X\to VA$. The coalgebra-morphism equation becomes exactly the equality of the two composites into $V L V A$, so the transposed arrow factors uniquely through the displayed [equalizer](../../../../../equaliser.md).

The counit $KJ(A,a)\to(A,a)$ is invertible. Applying $L$ to the defining [equalizer](../../../../../equaliser.md) gives the [equalizer](../../../../../equaliser.md) of $Ga,\delta_A:GA\rightrightarrows G^2A$. The structure map $a:A\to GA$ is exactly that [equalizer](../../../../../equaliser.md): it equalizes by coassociativity; if $t:T\to GA$ equalizes, apply $\varepsilon_{GA}$ to obtain $t=a\varepsilon_A t$, giving its unique factorization through $a$. Thus the underlying comparison counit is an isomorphism, and the [forgetful functor](../../../../../forgetful-functor.md) reflects isomorphisms. Therefore $J$ is [full and faithful](../../../../../full-and-faithful-functor.md).

The adjunctions $U\dashv R$ and $K\dashv J$ define

$$
\boxed{\mathcal H\xrightarrow{p}\mathcal D\xrightarrow{i}\mathcal E,\qquad f=i\circ p.}
$$

Here $p^*=U$ is faithful, so $p$ is a [surjective geometric morphism](../../../../../surjective-geometric-morphism.md); $i_*=J$ is full and faithful, so $i$ is a [geometric embedding](../../../../../geometric-embedding.md). Their inverse-image composite is $UK=L$, establishing the [surjection-embedding factorization of a geometric morphism](../../../../../surjection-embedding-factorization-of-a-geometric-morphism.md).

For uniqueness, let $S$ be the class of arrows in $\mathcal E$ inverted by $f^*$. In any surjection-embedding factorization $f=i'p'$, conservativity of $p'^*$ shows that $S$ is also the class inverted by $i'^*$. The essential image of the fully faithful $i'_*$ consists exactly of the $S$-local objects $Y$, namely those for which $\mathcal E(B,Y)\to\mathcal E(A,Y)$ is bijective for every $A\to B$ in $S$. One direction follows from the adjunction. For the converse, the reflector unit $Y\to i'_*i'^*Y$ belongs to $S$; locality gives a retraction, and locality of the reflected object makes that retraction also a right inverse. Thus the unit is invertible. The image subcategory is consequently determined by $f$, independently of the factorization. The two intermediate toposes are equivalent over $\mathcal E$, and their inverse-image composites with the embeddings determine the surjection legs. This proves **uniqueness up to equivalence**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
