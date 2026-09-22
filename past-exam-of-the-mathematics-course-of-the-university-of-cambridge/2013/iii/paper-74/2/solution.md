<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [Cartesian comonad](../../../../../cartesian-comonad.md) as $(G,\varepsilon,\delta)$, with $G$ preserving [finite limits](../../../../../finite-limit.md). A [coalgebra for a comonad](../../../../../coalgebra-for-a-comonad.md) is $(A,a)$ with $a:A\to GA$, $\varepsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. Its [forgetful functor](../../../../../forgetful-functor.md) $U:\mathcal E^G\to\mathcal E$ is faithful, creates [finite limits](../../../../../finite-limit.md), and has the [cofree coalgebra](../../../../../cofree-coalgebra.md) right adjoint $R(X)=(GX,\delta_X)$. We construct the two remaining [topos](../../../../../elementary-topos.md) structures explicitly.

For [exponential objects](../../../../../exponential-object.md), take coalgebras $(A,a),(B,b)$ and start with $R(B^A)$. Put $X=G(B^A)$, with structure $\xi=\delta_{B^A}$, and let

$$
e:X\times A\longrightarrow B,\qquad e=\operatorname{ev}(\varepsilon_{B^A}\times1_A).
$$

Transpose the following two maps $X\times A\to GB$ into maps $u,v:X\to(GB)^A$:

$$
be,\qquad Ge\circ(\xi\times a),
$$

using $G(X\times A)\cong GX\times GA$. The cofree [adjunction](../../../../../adjoint-functors.md) transposes $u,v$ once more into coalgebra morphisms $R(B^A)\rightrightarrows R((GB)^A)$. Let $Q$ be their [equalizer](../../../../../equaliser.md). A coalgebra map $(C,c)\to R(B^A)$ corresponds to an arbitrary ambient map $h:C\times A\to B$. It factors through $Q$ precisely when

$$
bh=Gh\circ(c\times a),
$$

which is exactly the condition that $h$ be a coalgebra morphism. Therefore $Q$ represents $\mathcal E^G(C\times A,B)$ and is the required [exponential in a coalgebra topos](../../../../../exponentials-in-a-coalgebra-topos.md).

For the [subobject classifier](../../../../../subobject-classifier.md), let $\kappa:G\Omega\to\Omega$ classify the mono $G\top:G1\cong1\hookrightarrow G\Omega$. In the cofree coalgebra $R\Omega$, form

$$
\Omega_G=\operatorname{Eq}\bigl(1_{R\Omega},G\kappa\,\delta_\Omega\bigr).
$$

Both arrows are coalgebra morphisms. The cofree transpose of $\top:1\to\Omega$ factors through this [equalizer](../../../../../equaliser.md) and gives its true arrow. To verify classification, let $S\hookrightarrow X$ have ambient characteristic map $\chi:X\to\Omega$. It supports a subcoalgebra of $(X,x)$ exactly when it is invariant under $x$, equivalently

$$
S=x^{-1}(GS),\qquad \chi=\kappa G\chi\,x.
$$

The counit proves the reverse containment in the first equation; the forward containment supplies the restricted structure map, whose coalgebra laws follow through the mono. Under the cofree [adjunction](../../../../../adjoint-functors.md), the second equation says exactly that $G\chi\,x:X\to R\Omega$ factors through $\Omega_G$. Pulling back its true arrow recovers $S$, since $\kappa G\chi\,x=\chi$. This proves the universal property of the [subobject classifier of a coalgebra topos](../../../../../subobject-classifier-of-a-coalgebra-topos.md). Hence **$\mathcal E^G$ is a [topos](../../../../../elementary-topos.md)**.

Now let $f:\mathcal E\to\mathcal F$ be a [geometric morphism](../../../../../geometric-morphism.md), with $L=f^*\dashv H=f_*$. The comonad $G=LH$ is Cartesian: $L$ preserves [finite limits](../../../../../finite-limit.md) and the right adjoint $H$ preserves limits. Put $\mathcal D=\mathcal E^G$, already a [topos](../../../../../elementary-topos.md). The forgetful [adjunction](../../../../../adjoint-functors.md) $U\dashv R$ defines $p:\mathcal E\to\mathcal D$ with $p^*=U$, so **$p^*$ is faithful**.

The comparison [functor](../../../../../functor.md)

$$
K:\mathcal F\to\mathcal D,\qquad K(Y)=(LY,L\eta_Y)
$$

preserves [finite limits](../../../../../finite-limit.md). It has a right adjoint $J$, given on a coalgebra $(A,a)$ by

$$
J(A,a)=\operatorname{Eq}\bigl(Ha,\eta_{HA}:HA\rightrightarrows HGA\bigr).
$$

Indeed, the transposed arrow $Y\to HA$ corresponds to a coalgebra map $KY\to(A,a)$ exactly when it equalizes these two maps. Applying the finite-limit-preserving $L$ shows that $LJ(A,a)$ is the [equalizer](../../../../../equaliser.md) of

$$
Ga,\delta_A:GA\rightrightarrows G^2A.
$$

That [equalizer](../../../../../equaliser.md) is $a:A\to GA$. If $t:Z\to GA$ equalizes the pair, then $a\varepsilon_At=\varepsilon_{GA}Ga\,t=\varepsilon_{GA}\delta_At=t$, proving the claimed universal property. Consequently the counit $KJ(A,a)\to(A,a)$ is invertible. The [fully faithful adjoint criterion](../../../../../fully-faithful-adjoint-criterion.md) makes **$J$ full and faithful**.

Thus $K\dashv J$ defines a [geometric embedding](../../../../../geometric-embedding.md) $i:\mathcal D\to\mathcal F$, and $UK=L$ identifies the composite with $f$. The requested factorization is

$$
\boxed{\mathcal E\xrightarrow{\ p\ }\mathcal D\xrightarrow{\ i\ }\mathcal F,\qquad f=i\circ p,}
$$

where $p$ is a [surjective geometric morphism](../../../../../surjective-geometric-morphism.md) and $i_*=J$ is full and faithful.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
