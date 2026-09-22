<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [product in a category](../../../../../product-category-theory.md) of [prevarieties](../../../../../prevariety.md), the projections $p_X,p_Y$ must induce a bijection

$$
\operatorname{Hom}_k(T,X\times Y)
\longrightarrow\operatorname{Hom}_k(T,X)\times\operatorname{Hom}_k(T,Y),
\qquad h\longmapsto(p_Xh,p_Yh)
$$

for every [prevariety](../../../../../prevariety.md) $T$. If $Z$ and $Z'$ both have this property, their projection pairs determine morphisms $Z\to Z'$ and $Z'\to Z$. Each composite has the same projections as the identity, so uniqueness in the universal property makes both composites identities. This gives the unique isomorphism respecting the projections.

Here the classical convention is that a [prevariety](../../../../../prevariety.md) is locally an [affine variety](../../../../../affine-algebraic-set.md), with a finite affine cover, and is irreducible; an [algebraic variety](../../../../../algebraic-variety.md) is a separated [prevariety](../../../../../prevariety.md), meaning that its [diagonal morphism](../../../../../diagonal-morphism.md) has closed image. The same separation argument works in the convention that also permits reducible varieties. For separated $X,Y$, under the rearrangement $(X\times Y)^2\cong X^2\times Y^2$, the diagonal is

$$
\Delta_{X\times Y}=\Delta_X\times\Delta_Y
=\pi_{X^2}^{-1}(\Delta_X)\cap\pi_{Y^2}^{-1}(\Delta_Y).
$$

It is closed, proving separation. For completeness, irreducibility in the classical convention follows from the affine calculation below: the products of affine charts are irreducible, and their pairwise intersections are nonempty since nonempty open subsets of each irreducible factor meet. An open cover by irreducible open sets with pairwise nonempty intersections has irreducible union. Thus the product is an [algebraic variety](../../../../../algebraic-variety.md).

To establish the [coordinate ring of a product of affine varieties](../../../../../coordinate-ring-of-a-product-of-affine-varieties.md), write $A=k[X]=k[x_1,\ldots,x_r]/J$ and $B=k[Y]=k[y_1,\ldots,y_s]/L$. The algebra

$$
A\otimes_kB\cong k[x_1,\ldots,x_r,y_1,\ldots,y_s]/(J,L)
$$

has zero set $X\times Y$. To see directly that $(J,L)$ is prime when $X,Y$ are irreducible, take nonzero $F,G\in A\otimes_kB$. Express $F=\sum_i a_i\otimes b_i$ with the $b_i$ linearly independent over $k$. The set of $x\in X$ for which $F_x=\sum_i a_i(x)b_i$ is nonzero is a nonempty open set: it is the union of the nonvanishing loci of the $a_i$, and at least one $a_i$ is nonzero. The [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) guarantees that such a function cannot vanish at every point. The analogous set for $G$ is also nonempty; their intersection contains a point $x$ by irreducibility. Since $B$ is an [integral domain](../../../../../integral-domain.md), $F_xG_x\ne0$, whence $FG\ne0$. Thus $A\otimes_kB$ is an [integral domain](../../../../../integral-domain.md), and the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) identifies $(J,L)$ with the defining ideal of its zero set. The resulting affine variety has the universal property: algebra maps from $A\otimes_kB$ to $\Gamma(T,\mathcal O_T)$ correspond to pairs of algebra maps from $A,B$, and these correspond to morphisms into $X,Y$. This dictionary holds for arbitrary $T$, since coordinate functions give the morphisms on affine charts and agree on overlaps. Uniqueness of the product now proves

$$
\boxed{k[X\times Y]\cong k[X]\otimes_k k[Y].}
$$

For the final part put $T=A\otimes_kA$ and $\mu(x\otimes y)=xy$. Restriction to the [diagonal morphism](../../../../../diagonal-morphism.md) is $\mu$, so $I=\ker\mu$. Write $\delta(a)=1\otimes a-a\otimes1$. The elements $\delta(a)$ generate $I$: quotienting by them identifies the two copies of $A$ and gives precisely the multiplication quotient $T/I\cong A$. The map $D(a)=[\delta(a)]$ is $k$-linear, vanishes on $k$, and takes values in $I/I^2$. Since

$$
\delta(ab)=(1\otimes a)\delta(b)+(b\otimes1)\delta(a),
\qquad 1\otimes a\equiv a\otimes1\pmod I,
$$

it obeys $D(ab)=aD(b)+bD(a)$ for the stated first-factor action. Hence it is a [derivation of an algebra](../../../../../derivation-of-an-algebra.md). The universal property of the [module of Kähler differentials](../../../../../kahler-differential.md) supplies an $A$-linear map $\theta:\Omega^1_{A/k}\to I/I^2$ with $\theta(da)=D(a)$.

Define the $k$-linear map $q:T\to\Omega^1_{A/k}$ by $q(x\otimes y)=x\,dy$. It is $A$-linear for the first-factor action and, by the Leibniz rule, satisfies

$$
q(rs)=\mu(r)q(s)+\mu(s)q(r)\qquad(r,s\in T).
$$

Therefore $q(I^2)=0$ and restriction induces $\psi:I/I^2\to\Omega^1_{A/k}$. We have $\psi\theta(da)=da$, so $\psi\theta$ is the identity because the $da$ generate the [module of Kähler differentials](../../../../../kahler-differential.md). Conversely, if $z=\sum_i x_i\otimes y_i\in I$, then $\sum_i x_iy_i=0$ and

$$
[z]=\sum_i x_i[1\otimes y_i-y_i\otimes1]=\theta\left(\sum_i x_i\,dy_i\right)=\theta\psi([z]).
$$

Thus the [conormal module of the diagonal](../../../../../conormal-module-of-the-diagonal.md) gives

$$
\boxed{\Omega^1_{A/k}\xrightarrow{\ \sim\ }I/I^2,\qquad da\longmapsto[1\otimes a-a\otimes1].}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 113](../../paper-113-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
