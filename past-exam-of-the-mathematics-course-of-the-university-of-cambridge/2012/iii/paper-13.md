# Paper 13

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_13.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_13.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the usual convention that a [variety](../../../algebraic-geometry.md#algebraic-variety) is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety). For a [quasi-projective algebraic set](../../../algebraic-geometry.md#quasi-projective-algebraic-set) $T$, its [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) is the supremum of the lengths $r$ of strict chains

$$
T_0\subsetneq T_1\subsetneq\cdots\subsetneq T_r
$$

of nonempty [irreducible closed subsets](../../../algebraic-geometry.md#irreducible-closed-subset) of $T$. It is the maximum of the [algebraic dimensions](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) of its [irreducible components](../../../algebraic-geometry.md#irreducible-component). On an [affine algebraic set](../../../algebraic-geometry.md#affine-algebraic-set), the correspondence between [irreducible closed subsets](../../../algebraic-geometry.md#irreducible-closed-subset) and [prime ideals](../../../commutative-algebra.md#prime-ideal) reverses inclusion, so this is the [Krull dimension](../../../commutative-algebra.md#krull-dimension) of the [coordinate ring](../../../algebraic-geometry.md#coordinate-ring). On a [quasi-projective algebraic set](../../../algebraic-geometry.md#quasi-projective-algebraic-set), it is the supremum of the [Krull dimensions](../../../commutative-algebra.md#krull-dimension) of the [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) of its [affine open subsets](../../../ringed-space.md#affine-open-subscheme). At a [closed point](../../../topology.md#closed-point) $x$, the [Krull dimension](../../../commutative-algebra.md#krull-dimension) of the [local ring](../../../commutative-algebra.md#local-ring) measures chains through $x$.

Here is a [closed-point dimension lemma for affine domains](../../../algebraic-geometry.md#closed-point-dimension-lemma-for-affine-domains) that avoids [transcendence degree](../../../algebra.md#transcendence-degree). Put $A=k[X]$. By [Noether normalization](../../../algebraic-geometry.md#noether-normalization), there is a [integral extension](../../../commutative-algebra.md#integral-extension)

$$
B=k[z_1,\ldots,z_d]\subset A.
$$

The number of variables is $d$ because [integral extensions preserve Krull dimension](../../../commutative-algebra.md#integral-extensions-preserve-krull-dimension) and $\dim B=d$. For any [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $\mathfrak m$ of $A$, its contraction $\mathfrak n$ to $B$ is a [maximal ideal](../../../commutative-algebra.md#maximal-ideal). Since $k$ is an [algebraically closed field](../../../algebra.md#algebraically-closed-field), $\mathfrak n=(z_1-c_1,\ldots,z_d-c_d)$ has [height of a prime ideal](../../../commutative-algebra.md#height-of-a-prime-ideal) $d$. The [going-down theorem](../../../commutative-algebra.md#going-down-theorem) applies because $B$ is an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain) and $A$ is a [integral domain](../../../commutative-algebra.md#integral-domain). It lifts a length-$d$ chain below $\mathfrak n$ to one below $\mathfrak m$. Hence

$$
\boxed{\dim A_{\mathfrak m}=\operatorname{ht}\mathfrak m=d.}
$$

The opposite inequality follows from $\dim A=d$.

For the nonempty [open subset](../../../topology.md#open-set) $U$, choose a nonempty [principal open subset](../../../ringed-space.md#principal-open-subscheme) $D(g)\subset U$ and a [closed point](../../../topology.md#closed-point) $x\in D(g)$. Every [prime ideal](../../../commutative-algebra.md#prime-ideal) below $\mathfrak m_x$ avoids $g$, so the preceding chain survives in the [localization](../../../commutative-algebra.md#localization-of-a-ring) $A_g$. Consequently $\dim D(g)\ge d$. Conversely, any chain of [irreducible closed subsets](../../../algebraic-geometry.md#irreducible-closed-subset) in $U$ gives a chain of the same length after taking closures in $X$: intersecting those closures with $U$ recovers the original subsets. Therefore

$$
\boxed{\dim U=\dim X=d.}
$$

For the [principal hypersurface dimension lemma](../../../algebraic-geometry.md#principal-hypersurface-dimension-lemma), let $P$ be a [minimal prime ideal](../../../commutative-algebra.md#minimal-prime-ideal) over $(f)$. Since $f\ne0$ in the [integral domain](../../../commutative-algebra.md#integral-domain) $A$, $P\ne(0)$. The [Krull principal ideal theorem](../../../commutative-algebra.md#krull-principal-ideal-theorem) gives $\operatorname{ht}P=1$. Choose a [closed point](../../../topology.md#closed-point) $x$ on $V(P)$ lying on none of the other finitely many [irreducible components](../../../algebraic-geometry.md#irreducible-component) of $V(f)$. Such a point exists because those other components cut out proper [closed subsets](../../../topology.md#closed-set) of the [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) $V(P)$, and [closed points](../../../topology.md#closed-point) are dense. Set $R=A_{\mathfrak m_x}$. Then $\dim R=d$ and

$$
\sqrt{fR}=PR.
$$

Write $s=\dim R/fR$. Choose a [system of parameters](../../../commutative-algebra.md#system-of-parameters) $\bar y_1,\ldots,\bar y_s$ in $R/fR$ and lift it to $R$. The [ideal](../../../commutative-algebra.md#ideal) $(f,y_1,\ldots,y_s)$ has radical equal to the [maximal ideal](../../../commutative-algebra.md#maximal-ideal) of $R$. The [Krull height theorem](../../../commutative-algebra.md#krull-height-theorem) yields $d\le s+1$. On the other hand, any chain of [prime ideals](../../../commutative-algebra.md#prime-ideal) containing $f$ can be extended strictly at the bottom by the zero [prime ideal](../../../commutative-algebra.md#prime-ideal) of the [integral domain](../../../commutative-algebra.md#integral-domain) $R$, giving $s\le d-1$. Thus $s=d-1$. Since $R/PR$ is a [localization](../../../commutative-algebra.md#localization-of-a-ring) of $A/P$, $\dim A/P\ge d-1$. Extending a chain in $A/P$ by $(0)\subsetneq P$ also gives $\dim A/P\le d-1$. Hence **every component has the required dimension**:

$$
\boxed{\dim V(P)=d-1.}
$$

This argument uses [Noether normalization](../../../algebraic-geometry.md#noether-normalization), [going-down theorem](../../../commutative-algebra.md#going-down-theorem), and the [Krull height theorem](../../../commutative-algebra.md#krull-height-theorem), never the [dimension from the function field](../../../algebraic-geometry.md#dimension-from-the-function-field) theorem. Irreducibility is essential: if the word [variety](../../../algebraic-geometry.md#algebraic-variety) were instead allowed to mean an arbitrary reducible [affine algebraic set](../../../algebraic-geometry.md#affine-algebraic-set), neither assertion would hold without extra hypotheses. For example, a disjoint union of an [affine plane](../../../ringed-space.md#affine-plane) and an [affine line](../../../ringed-space.md#affine-line) has an open component of smaller [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set); a function equal to $1$ on the plane and a coordinate on the line has a nonempty zero set of [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) $0$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Put $A=k[X]$. There is an explicit [isomorphism](../../../algebra.md#isomorphism) from the [principal open subset](../../../ringed-space.md#principal-open-subscheme) $U_f$ to the [affine algebraic set](../../../algebraic-geometry.md#affine-algebraic-set)

$$
Z=V(sf-1)\subset X\times\mathbb A^1,\qquad x\longmapsto(x,f(x)^{-1}).
$$

Its inverse is projection, and both maps are [regular maps](../../../algebraic-geometry.md#morphism-of-algebraic-varieties). The [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) is

$$
k[Z]=A[s]/(sf-1)\cong A_f,
$$

by the [universal property of localization](../../../commutative-algebra.md#universal-property-of-localization). Since [regular functions](../../../ringed-space.md#regular-function) on an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) are its [coordinate ring](../../../algebraic-geometry.md#coordinate-ring), this proves the natural $k$-[algebra isomorphism](../../../algebra.md#algebra-isomorphism)

$$
\boxed{k[U_f]\cong k[X]_f.}
$$

Now $W=D(x)\cup D(y)$. A [regular function](../../../ringed-space.md#regular-function) on $W$ determines one element of the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) $k(x,y)$, and its restrictions belong to $k[x,y]_x$ and $k[x,y]_y$. Conversely, elements of their intersection glue because they agree on $D(xy)$. Thus

$$
k[W]=k[x,y]_x\cap k[x,y]_y\subset k(x,y).
$$

If a reduced fraction has denominator dividing a power of $x$ and also a power of $y$, [unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain) makes its denominator a [unit](../../../algebra.md#unit-in-a-ring). Therefore **puncturing the plane does not change its ring of global [regular functions](../../../ringed-space.md#regular-function)**:

$$
\boxed{k[W]=k[x,y].}
$$

If $W$ were an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), its inclusion $j:W\hookrightarrow\mathbb A^2$ would correspond to the identity [isomorphism](../../../algebra.md#isomorphism) $k[x,y]\to k[W]$. The equivalence between [affine varieties](../../../algebraic-geometry.md#affine-algebraic-set) and their [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) would make $j$ an [isomorphism](../../../algebra.md#isomorphism), contradicting the missing origin. Hence **$W$ is not affine**. This illustrates [regular functions on the punctured affine plane](../../../ringed-space.md#regular-functions-on-the-punctured-affine-plane): the [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) alone does not recover a nonaffine [variety](../../../algebraic-geometry.md#algebraic-variety).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Take the [three-dimensional affine quadric cone](../../../algebraic-geometry.md#three-dimensional-affine-quadric-cone)

$$
X=V(xy-zw)\subset\mathbb A^4,\qquad
Y=V_X(x,z),\qquad Z=V_X(y,w).
$$

The [polynomial](../../../polynomial.md) $xy-zw$ is an [irreducible polynomial](../../../polynomial.md#irreducible-polynomial): as a polynomial in $x$ over $k[y,z,w]$, it is primitive because $y$ and $zw$ are [coprime elements of a unique factorization domain](../../../algebra.md#coprime-elements-of-a-unique-factorization-domain), and it is a linear [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) over $k(y,z,w)$. [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials) then applies. Thus $X$ is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) that is an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), of [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) $3$ by the [principal hypersurface dimension lemma](../../../algebraic-geometry.md#principal-hypersurface-dimension-lemma) in [affine space](../../../geometry-and-topology.md#affine-space) $\mathbb A^4$.

The [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) of $Y$ and $Z$ are respectively $k[y,w]$ and $k[x,z]$. Both are [affine planes](../../../ringed-space.md#affine-plane), hence [irreducible closed subsets](../../../algebraic-geometry.md#irreducible-closed-subset) of [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) $2$. Their intersection is precisely the origin. Therefore

$$
\boxed{\dim X=3,\quad\dim Y=\dim Z=2,\quad\dim(Y\cap Z)=0.}
$$

The origin is the [singular point of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) of this [three-dimensional affine quadric cone](../../../algebraic-geometry.md#three-dimensional-affine-quadric-cone). The example shows why a [smoothness of an algebraic variety](../../../algebraic-geometry.md#smoothness-of-an-algebraic-variety) hypothesis matters in [intersection dimension estimates](../../../algebraic-geometry.md#intersection-dimension-bound-on-a-smooth-variety).

## 2

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [blowup of an algebraic variety](../../../algebraic-geometry.md#blowing-up-algebraic-geometry) supplies a reduced special fibre with all three requested defects. Let $B=\mathbb A^3$ have coordinates $(x,y,z)$, let $p=(0,1,0)$, and let $\pi:X=\operatorname{Bl}_pB\to B$. Take $Y=\mathbb A^1$ and the [regular map](../../../algebraic-geometry.md#morphism-of-algebraic-varieties)

$$
f:X\longrightarrow Y,\qquad f=(xy)\circ\pi.
$$

For an explicit construction, $X$ is the closed [subvariety](../../../algebraic-geometry.md#closed-subvariety) of $\mathbb A^3\times\mathbb P^2$, with projective coordinates $[u:v:w]$, defined by

$$
xv=(y-1)u,\qquad xw=zu,\qquad (y-1)w=zv.
$$

These equations say that $(x,y-1,z)$ is proportional to $(u,v,w)$. The three standard projective charts are [affine spaces](../../../geometry-and-topology.md#affine-space) $\mathbb A^3$, so $X$ is a [smooth variety](../../../algebraic-geometry.md#smooth-algebraic-variety) which is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) embedded in a [quasi-projective algebraic set](../../../algebraic-geometry.md#quasi-projective-algebraic-set). Its [algebraic exceptional divisor](../../../algebraic-geometry.md#algebraic-exceptional-divisor) is $E=\pi^{-1}(p)\cong\mathbb P^2$.

If $t\ne0$, the surface $xy=t$ misses $p$, and the [blowup of an algebraic variety](../../../algebraic-geometry.md#blowing-up-algebraic-geometry) is an [isomorphism](../../../algebra.md#isomorphism) over it. Hence

$$
\boxed{X_t\cong\operatorname{Spec}k[x,x^{-1},z]\cong\mathbb G_m\times\mathbb A^1.}
$$

It is a [smooth variety](../../../algebraic-geometry.md#smooth-algebraic-variety), an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety), and has [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) $2$.

For $t=0$, the [fibre of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism) has three [irreducible components](../../../algebraic-geometry.md#irreducible-component): the [strict transform of an algebraic subvariety](../../../algebraic-geometry.md#strict-transform-of-an-algebraic-subvariety) $\widetilde{V(x)}$, the unchanged plane $V(y)$, and the [algebraic exceptional divisor](../../../algebraic-geometry.md#algebraic-exceptional-divisor) $E\cong\mathbb P^2$. The centre $p$ lies on $V(x)$ but not on $V(y)$; this is why all three components have multiplicity one. To verify reducedness and the crossing directly near $E$, use the chart $v\ne0$, putting

$$
a=x/(y-1),\qquad b=y-1,\qquad c=z/(y-1).
$$

Here $x=ab$, $y=1+b$, $z=bc$, and $f=ab(1+b)$. Near $b=0$, the factor $1+b$ is a [unit](../../../algebra.md#unit-in-a-ring), so the [fibre of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism) is $ab=0$, a reduced union of two crossing planes. The $u$-chart gives $f=x(1+xv)$, whose second factor is a [unit](../../../algebra.md#unit-in-a-ring) along $E$; the $w$-chart gives $f=zu(1+zv)$ and the same reduced crossing. Away from $E$, reducedness follows from $xy=0$ in $B$. Thus the scheme-theoretic [fibre of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism) is itself reduced.

It has [singular points of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) already along $V(x,y)$, which misses $p$: locally its equation is $xy=0$, with [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space) of [dimension of a vector space](../../../vector-space.md#dimension-vector-space) $3$ but [local dimension of an algebraic variety](../../../algebraic-geometry.md#local-dimension-of-an-algebraic-variety) $2$. Finally, $E$ is a closed [subvariety](../../../algebraic-geometry.md#closed-subvariety) of $X_0$. A closed [subvariety](../../../algebraic-geometry.md#closed-subvariety) of an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) is an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), whereas $\mathbb P^2$ is not: all its [global regular functions](../../../ringed-space.md#global-regular-function) are constant, which cannot be the [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) of a positive-dimensional [affine variety](../../../algebraic-geometry.md#affine-algebraic-set). Consequently **$X_0$ is singular, reducible, and nonaffine**, as required. Choosing the centre off the intersection of the original planes avoids introducing a nonreduced special [fibre of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use the dense standard [affine charts](../../../ringed-space.md#affine-chart-of-a-variety). Their product is

$$
\mathbb A^n\times\mathbb A^m\cong\mathbb A^{n+m},
$$

which is also a dense [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) of $\mathbb P^{n+m}$. The identification of these charts gives **a birational isomorphism** between the two [projective varieties](../../../projective-space.md#projective-variety).

To distinguish them, calculate their [divisor class groups](../../../algebraic-geometry.md#divisor-class-group) explicitly. Let $H\subset\mathbb P^r$ be a coordinate [hyperplane](../../../vector-space.md#hyperplane). Its complement is $\mathbb A^r$, whose [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) is a [unique factorization domain](../../../algebra.md#unique-factorization-domain). Any [Weil divisor](../../../algebraic-geometry.md#weil-divisor) on $\mathbb P^r$ restricts on this chart to a [principal Weil divisor](../../../algebraic-geometry.md#principal-weil-divisor); subtract that [principal Weil divisor](../../../algebraic-geometry.md#principal-weil-divisor) on $\mathbb P^r$, leaving a [Weil divisor](../../../algebraic-geometry.md#weil-divisor) supported on $H$. Thus $[H]$ generates $\operatorname{Cl}(\mathbb P^r)$. If $aH=\operatorname{div}(q)$, then $q$ has zero [Weil divisor](../../../algebraic-geometry.md#weil-divisor) on $\mathbb A^r$. A reduced fraction in a [unique factorization domain](../../../algebra.md#unique-factorization-domain) with zero orders at every [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) must be a [unit](../../../algebra.md#unit-in-a-ring), so $q\in k^*$. It follows that $a=0$. We have proved

$$
\boxed{\operatorname{Cl}(\mathbb P^r)\cong\mathbb Z\quad(r>0).}
$$

In the product, let $H_1$ and $H_2$ be coordinate [hyperplanes](../../../vector-space.md#hyperplane) in the factors and put

$$
D_1=H_1\times\mathbb P^m,\qquad D_2=\mathbb P^n\times H_2.
$$

The complement of $D_1\cup D_2$ is $\mathbb A^{n+m}$, again with a [unique factorization domain](../../../algebra.md#unique-factorization-domain) as its [coordinate ring](../../../algebraic-geometry.md#coordinate-ring). The same restriction-and-subtraction argument says that $[D_1],[D_2]$ generate the [divisor class group](../../../algebraic-geometry.md#divisor-class-group). If

$$
aD_1+bD_2=\operatorname{div}(q),
$$

then on that [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) $q$ has neither zeros nor poles along any [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor). [Unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain) makes $q$ a [unit](../../../algebra.md#unit-in-a-ring) of $k[s_1,\ldots,s_n,t_1,\ldots,t_m]$, hence a constant. It follows that $a=b=0$. Therefore

$$
\boxed{\operatorname{Cl}(\mathbb P^n\times\mathbb P^m)\cong\mathbb Z^2.}
$$

Both spaces are [smooth varieties](../../../algebraic-geometry.md#smooth-algebraic-variety), so their [divisor class groups](../../../algebraic-geometry.md#divisor-class-group) also equal their [Picard groups](../../../ringed-space.md#picard-group). An [isomorphism](../../../algebra.md#isomorphism) preserves the [divisor class group](../../../algebraic-geometry.md#divisor-class-group); $\mathbb Z^2$ and $\mathbb Z$ are not [isomorphic](../../../algebra.md#isomorphism). Thus **the spaces are birational but not isomorphic**. The assumptions $n,m>0$ ensure that both boundary [prime Weil divisors](../../../algebraic-geometry.md#prime-weil-divisor) actually occur.

## 3

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Suppose there were distinct [singular points of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) $P,Q$. Let $L$ be their joining [projective line](../../../finite-group-theory.md#projective-line). The homogeneous restriction $F|_L$ has degree $3$. At a [singular point of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) of a plane [algebraic curve](../../../algebraic-geometry.md#algebraic-curve), the local defining equation has no constant or linear term, so its restriction to any line through that point vanishes to order at least $2$, unless the restriction is identically zero. Therefore a nonzero $F|_L$ would have at least four zeros counted with multiplicity, two at $P$ and two at $Q$, which a degree-$3$ homogeneous [polynomial](../../../polynomial.md) on $\mathbb P^1$ cannot have.

Hence $F|_L=0$. After choosing coordinates with $L=V(z)$, this says that every monomial of $F$ contains $z$, so $z$ divides $F$. That contradicts the [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) hypothesis on the cubic. Thus

$$
\boxed{\text{An irreducible plane cubic has at most one singular point.}}
$$

This elementary version of the [Bézout theorem](../../../algebraic-geometry.md#bezout-s-theorem) argument works in every [characteristic](../../../algebra.md#characteristic-of-a-field), without assuming that the [partial derivatives](../../../calculus.md#partial-derivative) of the cubic have their characteristic-zero form.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Write $x,y$ for the two coordinates. The PDF gives $\mu=e^{\pi i/3}$, a primitive sixth root of unity. The matrices satisfy

$$
\sigma^6=1,\qquad \tau^2=-I=\sigma^3,\qquad
\tau\sigma\tau^{-1}=\sigma^{-1}.
$$

These relations reduce every word to $\sigma^j$ or $\tau\sigma^j$, $0\le j<6$. The six first matrices are diagonal and distinct, and the six second matrices are antidiagonal and distinct. Thus **$G$ has exactly twelve elements**; it is a [binary dihedral group](../../../finite-group-theory.md#dicyclic-group).

First calculate the [polynomial invariant ring](../../../representation-theory.md#polynomial-invariant-ring) of $\langle\sigma\rangle$. A monomial $x^a y^b$ is invariant exactly when $a-b$ is divisible by $6$. Removing the smaller exponent shows that it is a product of powers of

$$
A=x^6,\qquad B=y^6,\qquad C=xy.
$$

The sole relation is $AB=C^6$. Indeed, reduction by this relation leaves monomials $C^jA^a$ and $C^jB^b$ with $b>0$, whose images in $\mathbb C[x,y]$ have distinct exponent pairs. Hence

$$
\mathbb C[x,y]^{\langle\sigma\rangle}
\cong\mathbb C[A,B,C]/(AB-C^6).
$$

On these generators, $\tau$ interchanges $A,B$ and sends $C$ to $-C$. Put $S=A+B$ and $T=A-B$. Since $2$ is invertible, the preceding [ring](../../../commutative-algebra.md#ring) is

$$
\mathbb C[S,C,T]/(T^2-S^2+4C^6).
$$

Every element has a unique form $P(S,C)+TQ(S,C)$. The induced involution fixes $S$ and negates both $C$ and $T$. Its invariants are therefore exactly the expressions

$$
P_0(S,C^2)+CTQ_0(S,C^2).
$$

Set

$$
U=x^6+y^6,\qquad V=x^2y^2,\qquad W=xy(x^6-y^6).
$$

We obtain the relation

$$
W^2=V(U^2-4V^3).
$$

The unique normal form above also proves that there are no further relations: $P_0(U,V)+WQ_0(U,V)=0$ forces both polynomials to vanish. Thus the [polynomial invariant ring](../../../representation-theory.md#polynomial-invariant-ring) is

$$
\boxed{\mathbb C[x,y]^G\cong
\mathbb C[U,V,W]/(W^2-VU^2+4V^4).}
$$

For completeness, the [algebraic quotient by a finite group](../../../algebraic-geometry.md#algebraic-quotient-by-a-finite-group) is the [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) with this [coordinate ring](../../../algebraic-geometry.md#coordinate-ring). Each element $h$ of $\mathbb C[x,y]$ satisfies the monic orbit polynomial $\prod_{g\in G}(Z-g h)$ with invariant coefficients, so the quotient map is a [finite morphism](../../../algebraic-geometry.md#finite-morphism). Invariants separate distinct finite orbits: interpolate a [polynomial](../../../polynomial.md) taking value $0$ on one orbit and $1$ on the other, and average it over $G$. Thus its fibres are precisely the orbits. The defining polynomial and resulting [algebraic quotient by a finite group](../../../algebraic-geometry.md#algebraic-quotient-by-a-finite-group) are

$$
\boxed{p(U,V,W)=W^2-VU^2+4V^4,\qquad
\mathbb A^2/G\cong V(p)\subset\mathbb A^3.}
$$

Using the converted TeX's fourth root would instead give a different group and a different [binary dihedral invariant hypersurface](../../../representation-theory.md#binary-dihedral-invariant-hypersurface); the sixth root from the original PDF is essential.

## 4

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Work on [affine open subsets](../../../ringed-space.md#affine-open-subscheme). Their [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) are [Noetherian rings](../../../algebra.md#noetherian-ring) and [integrally closed domains](../../../commutative-algebra.md#integrally-closed-domain). At a [prime ideal](../../../commutative-algebra.md#prime-ideal) of [height of a prime ideal](../../../commutative-algebra.md#height-of-a-prime-ideal) one, the [local ring](../../../commutative-algebra.md#local-ring) is a one-dimensional [Noetherian local ring](../../../algebra.md#noetherian-local-ring) which is an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain), hence a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) and therefore a [regular local ring](../../../commutative-algebra.md#regular-local-ring). At the generic point the [local ring](../../../commutative-algebra.md#local-ring) is a [field](../../../algebra.md#field), hence a [regular local ring](../../../commutative-algebra.md#regular-local-ring). For a brief justification of the one-dimensional [local ring](../../../commutative-algebra.md#local-ring) fact, take $0\ne a\in\mathfrak m$ in a one-dimensional [Noetherian local ring](../../../algebra.md#noetherian-local-ring) $R$ which is an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain). Some $\mathfrak m^n\subset(a)$; choose the least such $n$, and choose $b\in\mathfrak m^{n-1}\setminus(a)$. Then $q=b/a\notin R$, but $q\mathfrak m\subset R$. If $q\mathfrak m\subset\mathfrak m$, the [determinant trick](../../../module-theory.md#determinant-trick) applied to the finitely generated faithful module $\mathfrak m$ would make $q$ integral over $R$, a contradiction. Hence the ideal $q\mathfrak m$ contains a unit and equals $R$. Thus $\mathfrak m=q^{-1}R$ is principal. A one-dimensional [Noetherian local ring](../../../algebra.md#noetherian-local-ring) with principal maximal ideal is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring). Therefore a [normal variety](../../../ringed-space.md#normal-variety) is [regular in codimension one](../../../ringed-space.md#regular-in-codimension-one).

The ground [field](../../../algebra.md#field) is an [algebraically closed field](../../../algebra.md#algebraically-closed-field), hence a [perfect field](../../../algebra.md#perfect-field), so having a [regular local ring](../../../commutative-algebra.md#regular-local-ring) is equivalent to being a [smooth point of a variety](../../../algebraic-geometry.md#smooth-point-of-a-variety) here. Moreover, the [smooth locus of a variety](../../../algebraic-geometry.md#smooth-locus-of-a-variety) is open, making the [singular locus](../../../algebraic-geometry.md#singular-locus) closed. If an [irreducible component](../../../algebraic-geometry.md#irreducible-component) of the [singular locus](../../../algebraic-geometry.md#singular-locus) had [algebraic codimension](../../../algebraic-geometry.md#codimension-of-an-algebraic-subvariety) zero or one, its generic point would have a [regular local ring](../../../commutative-algebra.md#regular-local-ring) by the preceding argument, a contradiction. Consequently every such component has [algebraic codimension](../../../algebraic-geometry.md#codimension-of-an-algebraic-subvariety) at least two.

One can read the numerical bound directly from chains of [prime ideals](../../../commutative-algebra.md#prime-ideal), without identifying [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) with [transcendence degree](../../../algebra.md#transcendence-degree). For a [prime ideal](../../../commutative-algebra.md#prime-ideal) $P$ of [height of a prime ideal](../../../commutative-algebra.md#height-of-a-prime-ideal) at least two in an [affine chart](../../../ringed-space.md#affine-chart-of-a-variety), append a chain $(0)\subsetneq P_1\subsetneq P$ below any chain in the quotient by $P$. Its length increases by two. Thus $\dim A/P\le\dim A-2$. Since a nonempty [affine open subset](../../../ringed-space.md#affine-open-subscheme) of the [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) $X$ has [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) $d$,

$$
\boxed{\dim\operatorname{Sing}(X)\le d-2.}
$$

For $d=0$ or $1$, this means the [singular locus](../../../algebraic-geometry.md#singular-locus) is empty; take $\dim\varnothing=-\infty$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $a=t_1$, $b=t_2$, $c=t_3$, and $A=\mathbb C[a,b,c]/(ac-b^2)$. It is the [quadratic cone invariant ring](../../../representation-theory.md#quadratic-cone-invariant-ring)

$$
A\cong\mathbb C[u^2,uv,v^2]=\mathbb C[u,v]^{\{\pm1\}},
$$

where the involution negates both $u$ and $v$. The invariant monomials have even total degree and are generated by $u^2,uv,v^2$; reduction by $ac=b^2$ proves the asserted presentation.

To verify the [normal variety](../../../ringed-space.md#normal-variety) property, suppose $q\in\operatorname{Frac}(A)$ is integral over $A$. The same monic equation makes $q$ integral over $\mathbb C[u,v]$. This [polynomial ring](../../../commutative-algebra.md#polynomial-ring) is an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain), so $q\in\mathbb C[u,v]$. Since $q$ belongs to the [fraction field](../../../commutative-algebra.md#field-of-fractions) of $A$, it is invariant under the involution, and hence belongs to $A$. Thus **$X$ is normal**. The [gradient](../../../calculus.md#gradient) of its equation is $(c,-2b,a)$, so the [Jacobian criterion](../../../algebraic-geometry.md#jacobian-criterion) shows that the origin $o$ is its only [singular point of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety). In particular **$X$ is not smooth**.

Take the [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) $D=V_X(a,b)$ and $x=o$. We show that $D$ is not a [Cartier divisor](../../../cartier-divisor.md) at $o$. In the [local ring](../../../commutative-algebra.md#local-ring)

$$
R=A_{(a,b,c)},\qquad\mathfrak m=(a,b,c)R,
$$

its prime [ideal](../../../commutative-algebra.md#ideal) is $I=(a,b)R$. The quotient $I/\mathfrak mI$ has [dimension of a vector space](../../../vector-space.md#dimension-vector-space) $2$ over $\mathbb C$: $a,b$ generate it, and they are independent since $\mathfrak mI\subset\mathfrak m^2$ while the relation $ac-b^2$ has no linear term. By [Nakayama lemma](../../../mathematics.md#nakayama-lemma), $I$ cannot be generated by one element.

On a [normal variety](../../../ringed-space.md#normal-variety), the ideal of an effective [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) is the [divisorial ideal](../../../algebraic-geometry.md#divisorial-ideal) of functions with order at least one along that divisor and order at least zero along every other [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor). If $D$ were a [Cartier divisor](../../../cartier-divisor.md) at $o$, a local defining [rational function](../../../isolated-singularity.md#rational-function) $h$ would identify this ideal with $hR$, because an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain) is the intersection of its height-one [localizations at a prime ideal](../../../commutative-algebra.md#localization-at-a-prime-ideal) inside its [fraction field](../../../commutative-algebra.md#field-of-fractions). That would make $I$ principal, contradicting the calculation. Therefore $D$ has a nonzero class in the local [divisor class group](../../../algebraic-geometry.md#divisor-class-group).

Now let $D'=D+\operatorname{div}(q)$ be any [linearly equivalent Weil divisor](../../../algebraic-geometry.md#linear-equivalence-of-weil-divisors). If $o$ were outside its [support of a Weil divisor](../../../algebraic-geometry.md#support-of-a-weil-divisor), there would be an [open subset](../../../topology.md#open-set) containing $o$ on which $D'$ is zero. On that neighbourhood $D=-\operatorname{div}(q)$ would be a [principal Weil divisor](../../../algebraic-geometry.md#principal-weil-divisor), hence a [Cartier divisor](../../../cartier-divisor.md), which is impossible. Therefore **this point is unavoidable in every representative**:

$$
\boxed{o\in\operatorname{Supp}(D')\quad\text{for every }D'\sim D.}
$$

The argument does not assume that $D'$ is effective. For comparison, $\operatorname{div}(a)=2D$ because on the chart $c\ne0$, $a=b^2/c$; the obstruction has order two, as in the [Divisor class group of an A-type surface singularity](../../../algebraic-geometry.md#divisor-class-group-of-an-a-type-surface-singularity).

## 5

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For a [smooth projective curve](../../../projective-space.md#smooth-projective-curve) $C$, let $g=h^1(C,\mathcal O_C)$ be its [geometric genus](../../../normalization-of-an-algebraic-curve.md#geometric-genus), let $K_C$ be a [canonical divisor](../../../algebraic-geometry.md#canonical-divisor), and write $\ell(D)=h^0(C,\mathcal O_C(D))$ for the [dimension of a vector space](../../../vector-space.md#dimension-vector-space) of the [Riemann-Roch space](../../../algebraic-geometry.md#riemann-roch-space). The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) says

$$
\boxed{\ell(D)-\ell(K_C-D)=\deg D+1-g}
$$

for every [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$ on $C$.

Here is the [cohomological proof of Riemann-Roch for curves](../../../algebraic-geometry.md#cohomological-proof-of-riemann-roch-for-curves). At a [closed point](../../../topology.md#closed-point) $P$, the [local ring](../../../commutative-algebra.md#local-ring) is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring). A local uniformizer shows that increasing the allowed pole order by one gives the [short exact sequence](../../../module-theory.md#short-exact-sequence) of [sheaves](../../../algebraic-geometry.md#sheaf-mathematics)

$$
0\longrightarrow\mathcal O_C(D-P)\longrightarrow\mathcal O_C(D)
\longrightarrow k(P)\longrightarrow0.
$$

The last term is a length-one [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf); its precise identification with $k$ is noncanonical, but its [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) has $h^0=1$ and $h^1=0$. All the relevant groups of [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) are finite-dimensional because $C$ is a [projective variety](../../../projective-space.md#projective-variety), and coherent [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) above degree one vanishes on a [algebraic curve](../../../algebraic-geometry.md#algebraic-curve). The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) therefore gives

$$
\chi(\mathcal O_C(D))=\chi(\mathcal O_C(D-P))+1,
\qquad \chi(\mathcal F)=h^0(C,\mathcal F)-h^1(C,\mathcal F).
$$

Since $k$ is an [algebraically closed field](../../../algebra.md#algebraically-closed-field), every [closed point](../../../topology.md#closed-point) has degree one. Iterating this identity for both positive and negative coefficients of $D$ proves

$$
\chi(\mathcal O_C(D))=\deg D+\chi(\mathcal O_C).
$$

Every [global regular function](../../../ringed-space.md#global-regular-function) on a [projective variety](../../../projective-space.md#projective-variety) which is an [irreducible variety](../../../algebraic-geometry.md#irreducible-variety) is constant; hence $h^0(C,\mathcal O_C)=1$ and $\chi(\mathcal O_C)=1-g$.

Finally apply [Serre duality](../../../ringed-space.md#serre-duality) for a [smooth projective curve](../../../projective-space.md#smooth-projective-curve):

$$
H^1(C,\mathcal O_C(D))^*
\cong H^0(C,\omega_C\otimes\mathcal O_C(-D))
=H^0(C,\mathcal O_C(K_C-D)).
$$

Taking [dimensions of a vector space](../../../vector-space.md#dimension-vector-space) and inserting this in the [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) identity proves the displayed [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem). The substantial inputs from [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) are finiteness and vanishing for coherent [sheaves](../../../algebraic-geometry.md#sheaf-mathematics) on a [projective curve](../../../projective-space.md#projective-curve), and [Serre duality](../../../ringed-space.md#serre-duality); the change of [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) is proved directly by the point exact sequence. In particular the argument handles negative as well as effective [divisors on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

An [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) works over every [algebraically closed field](../../../algebra.md#algebraically-closed-field), including one algebraic over a finite field. Give it explicitly in $\mathbb P^2$ by

$$
E:\quad
\begin{cases}
y^2z=x^3-xz^2,&\operatorname{char}k\ne2,\\
y^2z+yz^2=x^3,&\operatorname{char}k=2.
\end{cases}
$$

In the first case the only point at infinity is $O=[0:1:0]$, where the derivative with respect to $z$ is nonzero. In the affine chart $z=1$, a [singular point of an algebraic variety](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) would have $y=0$, $x^3-x=0$, and $3x^2-1=0$. The possible roots $x=0,1,-1$ cannot satisfy the last equation in [characteristic](../../../algebra.md#characteristic-of-a-field) different from $2$: at $0$ it is $-1$, and at $\pm1$ it is $2$. In the second case the three homogeneous [partial derivatives](../../../calculus.md#partial-derivative) are $x^2,z^2,y^2$, up to harmless signs, and cannot vanish simultaneously at a projective point. Thus both cubics are [smooth varieties](../../../algebraic-geometry.md#smooth-algebraic-variety). A reducible plane cubic would have intersecting positive-degree components by [Bézout theorem](../../../algebraic-geometry.md#bezout-s-theorem), and be singular at an intersection; therefore these smooth cubics are [irreducible varieties](../../../algebraic-geometry.md#irreducible-variety). The [genus-degree formula](../../../algebraic-geometry.md#genus-degree-formula) gives $g=(3-1)(3-2)/2=1$. With the marked point $O$ they are [elliptic curves](../../../normalization-of-an-algebraic-curve.md#elliptic-curve).

For a [smooth algebraic curve](../../../algebraic-geometry.md#smooth-algebraic-curve), its [divisor class group](../../../algebraic-geometry.md#divisor-class-group) is its [Picard group](../../../ringed-space.md#picard-group). Its degree-zero subgroup is

$$
\operatorname{Pic}^0(E)=\{[D]:\deg D=0\}.
$$

The map $P\mapsto[P-O]$ gives an [isomorphism](../../../algebra.md#isomorphism) of [abelian groups](../../../group.md#abelian-group)

$$
E(k)\cong\operatorname{Pic}^0(E).
$$

To recall why it is a bijection, [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) in [geometric genus](../../../normalization-of-an-algebraic-curve.md#geometric-genus) one says every degree-one [divisor class](../../../algebraic-geometry.md#divisor-class) has exactly one independent section: a [canonical divisor](../../../algebraic-geometry.md#canonical-divisor) has degree zero, so the dual degree-$-1$ term has no section. Thus the class contains one effective [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) of degree one, namely a point $P$, and that point is unique. Translating by $-O$ gives the claimed bijection; this is precisely the [chord-and-tangent group law](../../../normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law) on the [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve).

Choose a prime integer $\ell$ different from $\operatorname{char}k$. The [multiplication-by-n morphism](../../../ringed-space.md#multiplication-by-n-morphism) $[\ell]:E\to E$ has derivative $\ell$ times the identity at $O$, so it is nonconstant. A nonconstant [morphism of algebraic varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties) between [smooth projective curves](../../../projective-space.md#smooth-projective-curve) is surjective: its image is closed by [proper morphism](../../../ringed-space.md#proper-morphism) and cannot have [algebraic dimension](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) zero. Since $k$ is an [algebraically closed field](../../../algebra.md#algebraically-closed-field), this makes $[\ell]$ surjective on $k$-points. Therefore

$$
E(k)=\ell E(k).
$$

Yet $E(k)$ is infinite. For each $x\in k$, the affine equation has a solution for $y$ in the [algebraically closed field](../../../algebra.md#algebraically-closed-field); since $k$ is infinite, this gives infinitely many points.

By the [Fundamental theorem of finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups), a [finitely generated abelian group](../../../group.md#finitely-generated-abelian-group) $A$ satisfying $A=\ell A$ has no free part and is a finite [torsion group](../../../group-theory.md#torsion-group) of order prime to $\ell$. The infinite group $E(k)$ cannot have this property while being finitely generated. Thus $\operatorname{Pic}^0(E)$ is not finitely generated. A subgroup of a [finitely generated abelian group](../../../group.md#finitely-generated-abelian-group) is finitely generated, so

$$
\boxed{\operatorname{Cl}(E)\text{ is not a finitely generated abelian group}.}
$$

This proof uses divisibility and infinitude, rather than uncountability, so it remains valid over countable [algebraically closed fields](../../../algebra.md#algebraically-closed-field).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
