<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a left $\mathbb ZG$-module, [group cohomology](../../../../../group-cohomology.md) is

$$
\boxed{H^n(G,M)=\operatorname{Ext}_{\mathbb ZG}^n(\mathbb Z,M),}
$$

with $\mathbb Z$ the trivial [module](../../../../../module-mathematics.md). Equivalently take a [projective resolution](../../../../../projective-resolution.md) $P_\bullet\to\mathbb Z$ and the cohomology of $\operatorname{Hom}_{\mathbb ZG}(P_\bullet,M)$. This also describes the right-derived functors of the invariant-module functor $M\mapsto M^G$.

For an explicit model, the homogeneous bar [free resolution](../../../../../free-resolution.md) has $P_n=\mathbb Z[G^{n+1}]$, with diagonal $G$-action and boundary the alternating sum of coordinate deletions. It is free over $\mathbb ZG$: each orbit has a unique representative with first coordinate $1$. The augmented complex is exact because inserting $1$ as a first coordinate supplies a contracting homotopy of underlying abelian groups; its lack of $G$-equivariance does not affect exactness. The associated inhomogeneous [group cochains](../../../../../group-cochain.md) are functions $f:G^n\to M$, with

$$
(df)(g_1,\ldots,g_{n+1})=
g_1f(g_2,\ldots,g_{n+1})
+\sum_{j=1}^n(-1)^jf(g_1,\ldots,g_jg_{j+1},\ldots,g_{n+1})
+(-1)^{n+1}f(g_1,\ldots,g_n).
$$

For [group cochains](../../../../../group-cochain.md) of degree zero, $(dm)(g)=gm-m$. Adjacent deletions cancel in pairs, giving $d^2=0$ and hence $H^n=\ker d/\operatorname{im}d$.

In degree zero this gives

$$
\boxed{H^0(G,M)=M^G=\{m:gm=m\text{ for all }g\}.}
$$

It is also $\operatorname{Hom}_{\mathbb ZG}(\mathbb Z,M)$, since a map is determined by the invariant image of $1$.

In degree one the cocycle condition is $f(gh)=f(g)+gf(h)$, so

$$
\boxed{H^1(G,M)=
\{\text{crossed homomorphisms }G\to M\}/
\{g\mapsto gm-m\}.}
$$

These are [crossed homomorphisms](../../../../../crossed-homomorphism.md) modulo [principal crossed homomorphisms](../../../../../principal-crossed-homomorphism.md). For trivial action they reduce to ordinary [group homomorphisms](../../../../../group-homomorphism.md), so $H^1(G,M)=\operatorname{Hom}(G_{\mathrm{ab}},M)$.

There are two further useful descriptions. If $I=\ker(\mathbb ZG\to\mathbb Z)$ is the [augmentation ideal](../../../../../augmentation-ideal.md), a [crossed homomorphism](../../../../../crossed-homomorphism.md) gives an equivariant map $I\to M$ by $g-1\mapsto f(g)$, because $gh-1=(g-1)+g(h-1)$. Applying $\operatorname{Hom}(-,M)$ to $0\to I\to\mathbb ZG\to\mathbb Z\to0$ therefore gives

$$
H^1(G,M)\cong
\operatorname{Hom}_{\mathbb ZG}(I,M)/
\operatorname{res}\operatorname{Hom}_{\mathbb ZG}(\mathbb ZG,M).
$$

Also a section of $M\rtimes G\to G$ has the form $g\mapsto(f(g),g)$ and is a [group homomorphism](../../../../../group-homomorphism.md) exactly when $f$ is a [crossed homomorphism](../../../../../crossed-homomorphism.md). Conjugation of sections by an element of $M$ changes $f$ by a [principal crossed homomorphism](../../../../../principal-crossed-homomorphism.md). Thus $H^1$ classifies the $M$-conjugacy classes of such sections, or equivalently of complements to $M$ in the [semidirect product](../../../../../semidirect-product.md).

In degree two, a normalized [two-cocycle](../../../../../two-cocycle.md) $c:G\times G\to M$ satisfies

$$
gc(h,l)-c(gh,l)+c(g,hl)-c(g,h)=0,\qquad c(1,g)=c(g,1)=0.
$$

Define multiplication on $M\times G$ by

$$
(m,g)(n,h)=(m+gn+c(g,h),gh).
$$

The displayed cocycle identity is precisely associativity; normalization gives the identity and inverses exist. This produces a [group extension](../../../../../group-extension.md) $1\to M\to E_c\to G\to1$ with the prescribed action on $M$.

Conversely a set-theoretic section $s:G\to E$, $s(1)=1$, gives $c(g,h)=s(g)s(h)s(gh)^{-1}$ in the additive [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md). Associativity gives the cocycle condition. Replacing $s(g)$ by $b(g)s(g)$ changes $c$ by

$$
(db)(g,h)=gb(h)-b(gh)+b(g).
$$

The resulting extensions are equivalent through a change of coordinates in $M\times G$. Conversely any extension equivalence preserving both [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) and quotient yields such a change of section. Hence

$$
\boxed{H^2(G,M)\ \longleftrightarrow\
\text{equivalence classes of extensions of }G\text{ by }M
\text{ with the specified action}.}
$$

The zero class corresponds exactly to a split extension. With trivial action these are central [group extensions](../../../../../group-extension.md); addition of classes corresponds to the [Baer sum](../../../../../baer-sum.md). This proves the [second group cohomology classifies group extensions](../../../../../second-group-cohomology-classifies-group-extensions.md) interpretation.

For $G=\mathbb Z^2$ and trivial coefficients $\mathbb Z$, put $R=\mathbb Z[x^{\pm1},y^{\pm1}]$. The [Koszul resolution for a rank-two free abelian group](../../../../../koszul-resolution-for-a-rank-two-free-abelian-group.md) is

$$
0\longrightarrow R\xrightarrow{d_2}R^2\xrightarrow{d_1}R
\xrightarrow{x,y\mapsto1}\mathbb Z\longrightarrow0,
$$

where $d_1(a,b)=(x-1)a+(y-1)b$ and $d_2(c)=(-(y-1)c,(x-1)c)$. To check exactness at $R^2$, reduce $d_1(a,b)=0$ modulo $x-1$. Since $y-1$ is not a zero divisor in $\mathbb Z[y^{\pm1}]$, write $b=(x-1)c$, and cancellation gives $a=-(y-1)c$. Injectivity of $d_2$ follows because $R$ is a domain. The augmentation [kernel](../../../../../kernel-of-a-linear-map.md) is generated by $x-1,y-1$, proving the other exactness statement.

Applying $\operatorname{Hom}_R(-,\mathbb Z)$ makes both differentials zero, since $x,y$ act trivially. Thus

$$
\boxed{H^0(\mathbb Z^2,\mathbb Z)=\mathbb Z,\quad
H^1(\mathbb Z^2,\mathbb Z)=\mathbb Z^2,\quad
H^2(\mathbb Z^2,\mathbb Z)=\mathbb Z,\quad H^n=0\ (n>2).}
$$

Degree-one classes assign arbitrary integers to the two generators. Geometrically these are also the cohomology groups of the [torus](../../../../../torus.md), a [classifying space](../../../../../classifying-space.md) for $\mathbb Z^2$; its cohomology ring is the [exterior algebra](../../../../../exterior-algebra.md) on the two degree-one classes.

The integer $n$ in degree two has an explicit extension representative. On triples $(a,b,m)\in\mathbb Z^3$, set

$$
(a,b,m)(c,d,l)=(a+c,b+d,m+l+nad).
$$

The bilinear term is a [two-cocycle](../../../../../two-cocycle.md). With generators $x=(1,0,0)$, $y=(0,1,0)$ and central $z=(0,0,1)$,

$$
\boxed{E_n=\langle x,y,z:\ z\text{ central},\ [x,y]=z^n\rangle.}
$$

Every central extension of $\mathbb Z^2$ by $\mathbb Z$ has this form: choose lifts of the two generators and the fixed generator of the [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md), then their [group commutator](../../../../../group-commutator.md) determines $n$ and every element has a unique form $z^my^bx^a$. Changing the lifts by central elements leaves that commutator unchanged. Thus distinct integers give inequivalent extensions, and the cocycles $nad$ add with $n$. The case $n=0$ is $\mathbb Z^3$; $n=1$ is the integer Heisenberg group. This realizes the [integral central extensions of a rank-two free abelian group](../../../../../integral-central-extensions-of-a-rank-two-free-abelian-group.md) concretely.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
