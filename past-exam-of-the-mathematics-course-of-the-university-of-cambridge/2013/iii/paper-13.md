# Paper 13

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_13.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_13.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) is understood to preserve $1$. Start with $\varphi:A\to B$. Its map on [spectra of rings](../../../ringed-space.md#spectrum-of-a-commutative-ring) is

$$
g:\operatorname{Spec}B\longrightarrow\operatorname{Spec}A,
\qquad \mathfrak q\longmapsto\varphi^{-1}(\mathfrak q).
$$

Contraction gives a [prime ideal](../../../commutative-algebra.md#prime-ideal), and $g^{-1}(D(a))=D(\varphi(a))$. Thus $g$ is [continuous](../../../calculus.md#continuous-function) for the [Zariski topology](../../../algebraic-geometry.md#zariski-topology). On each [principal open subscheme](../../../ringed-space.md#principal-open-subscheme), the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme) map is the [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism)

$$
A_a\longrightarrow B_{\varphi(a)},\qquad
\frac{b}{a^m}\longmapsto\frac{\varphi(b)}{\varphi(a)^m}.
$$

These maps commute with restrictions, so they define a [sheaf morphism](../../../algebraic-geometry.md#morphism-of-sheaves) $\mathcal O_X\to g_*\mathcal O_Y$. At $\mathfrak q$, with $\mathfrak p=\varphi^{-1}(\mathfrak q)$, its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) map is $A_{\mathfrak p}\to B_{\mathfrak q}$. The inverse image of the [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $\mathfrak qB_{\mathfrak q}$ is $\mathfrak pA_{\mathfrak p}$, so this is a [local homomorphism](../../../commutative-algebra.md#local-homomorphism-of-local-rings). We have constructed a [morphism of locally ringed spaces](../../../ringed-space.md#morphism-of-locally-ringed-spaces).

Conversely, let $(g,g^\#)$ be a [morphism of locally ringed spaces](../../../ringed-space.md#morphism-of-locally-ringed-spaces). Its map on [global sections](../../../ringed-space.md#global-section) gives $\varphi:A\to B$, using $\Gamma(X,\mathcal O_X)=A$ and $\Gamma(Y,\mathcal O_Y)=B$. Fix $\mathfrak q\in Y$ and put $\mathfrak p=g(\mathfrak q)$. Compatibility with the [stalk](../../../ringed-space.md#stalk-of-a-sheaf) maps and the [local homomorphism](../../../commutative-algebra.md#local-homomorphism-of-local-rings) property give

$$
a\in\mathfrak p
\iff a/1\in\mathfrak pA_{\mathfrak p}
\iff g^\#_{\mathfrak q}(a/1)\in\mathfrak qB_{\mathfrak q}
\iff\varphi(a)\in\mathfrak q.
$$

Consequently $\mathfrak p=\varphi^{-1}(\mathfrak q)$, so the underlying map is forced. On $D(a)$, the [sheaf morphism](../../../algebraic-geometry.md#morphism-of-sheaves) is forced as well: it extends $\varphi$ and sends $a$ to a [unit](../../../algebra.md#unit-in-a-ring), hence agrees with the displayed map by the [universal property of localization](../../../commutative-algebra.md#universal-property-of-localization). The [principal open subschemes](../../../ringed-space.md#principal-open-subscheme) form a basis, so the entire [sheaf morphism](../../../algebraic-geometry.md#morphism-of-sheaves) is determined. Taking [global sections](../../../ringed-space.md#global-section) of the construction recovers $\varphi$. **The two constructions are inverse**, proving the [affine-target adjunction for schemes](../../../ringed-space.md#affine-target-adjunction-for-schemes) in the affine-source case:

$$
\boxed{\operatorname{Hom}_{\mathrm{LRS}}(\operatorname{Spec}B,\operatorname{Spec}A)
\cong\operatorname{Hom}_{\mathrm{Ring}}(A,B).}
$$

To describe the [real affine plane scheme points](../../../ringed-space.md#real-affine-plane-scheme-points), write $R=\mathbb R[t_1,t_2]$. It is a [unique factorization domain](../../../algebra.md#unique-factorization-domain) of [Krull dimension](../../../commutative-algebra.md#krull-dimension) two. Its points are exactly the following [prime ideals](../../../commutative-algebra.md#prime-ideal):

- $(0)$, the [generic point](../../../algebraic-geometry.md#generic-point) of the whole [affine plane](../../../ringed-space.md#affine-plane).
- $(P)$ for each nonconstant [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) $P\in R$, taken up to multiplication by a nonzero real constant. These are the height-one points, each the [generic point](../../../algebraic-geometry.md#generic-point) of the [integral scheme](../../../ringed-space.md#integral-scheme) $V(P)$.
- The [maximal ideals](../../../commutative-algebra.md#maximal-ideal), or [closed points](../../../topology.md#closed-point). By the [Zariski lemma](../../../algebraic-geometry.md#zariski-s-lemma), their [residue fields](../../../commutative-algebra.md#residue-field) are finite algebraic extensions of $\mathbb R$. Because $\mathbb R$ is a [real closed field](../../../algebra.md#real-closed-field), those fields are $\mathbb R$ or $\mathbb C$. The first type is $(t_1-a,t_2-b)$ with $(a,b)\in\mathbb R^2$. The second type is the kernel of evaluation $R\to\mathbb C$ at a nonreal pair $(a,b)\in\mathbb C^2\setminus\mathbb R^2$; the pairs $(a,b)$ and $(\bar a,\bar b)$ give the same [maximal ideal](../../../commutative-algebra.md#maximal-ideal), and these are the only repetitions.

For completeness, any height-one [prime ideal](../../../commutative-algebra.md#prime-ideal) contains an [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) $P$; since $(P)$ is already a height-one [prime ideal](../../../commutative-algebra.md#prime-ideal), it must equal $(P)$. Every remaining nonzero [prime ideal](../../../commutative-algebra.md#prime-ideal) has height two and is maximal, by [Krull dimension](../../../commutative-algebra.md#krull-dimension). For a nonreal pair, evaluation generates all of $\mathbb C$ over $\mathbb R$, so its kernel is maximal. Conversely, each [residue field](../../../commutative-algebra.md#residue-field) isomorphic to $\mathbb C$ has exactly the two conjugate real-algebra embeddings into $\mathbb C$, proving the assertion about repetitions.

This describes the topology too: $V(I)$ consists of the [prime ideals](../../../commutative-algebra.md#prime-ideal) containing $I$, and the closure of a point $\mathfrak p$ is $V(\mathfrak p)$. In particular, the closure of $(0)$ is the whole [affine plane](../../../ringed-space.md#affine-plane), while the closure of $(P)$ contains precisely the [closed points](../../../topology.md#closed-point) on $P=0$, together with $(P)$ itself. **The spectrum is much larger than the set $\mathbb R^2$.** For example, $(t_1^2+1)$ is a height-one point although its curve has no real points. Its [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme) has $\mathcal O(D(h))=R_h$ and [stalk](../../../ringed-space.md#stalk-of-a-sheaf) $R_{\mathfrak p}$ at $\mathfrak p$.

The induced [morphism of schemes](../../../ringed-space.md#morphism-of-schemes)

$$
\pi:\operatorname{Spec}\mathbb C[t_1,t_2]\longrightarrow\operatorname{Spec}R
$$

is contraction of [prime ideals](../../../commutative-algebra.md#prime-ideal), with the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme) maps given above. On [closed points](../../../topology.md#closed-point), it sends $(t_1-a,t_2-b)$ to the kernel of real-polynomial evaluation at $(a,b)$. A real [closed point](../../../topology.md#closed-point) has one complex point above it; a nonreal [closed point](../../../topology.md#closed-point) has two, interchanged by [complex conjugation](../../../complex-analysis.md#complex-conjugation). The source [generic point](../../../algebraic-geometry.md#generic-point) maps to the target [generic point](../../../algebraic-geometry.md#generic-point). The source height-one points are generated by irreducible complex polynomials $Q$. Their contractions are height-one [prime ideals](../../../commutative-algebra.md#prime-ideal) $(P)$, and $Q$ is a factor of $P$ over $\mathbb C$. An irreducible real $P$ either stays irreducible over $\mathbb C$ or splits into two distinct conjugate irreducible factors. Indeed, [complex conjugation](../../../complex-analysis.md#complex-conjugation) acts transitively on its distinct factors, or a proper orbit product would give a real factor of $P$; every orbit has size at most two. Repeated factors are excluded by separability in [characteristic zero](../../../algebra.md#characteristic-zero). Thus one or two height-one points lie above $(P)$.

The [complexification fibres of a real scheme](../../../ringed-space.md#complexification-fibres-of-a-real-scheme) give a uniform description of all [scheme-theoretic fibres](../../../ringed-space.md#scheme-theoretic-fibre), including the nonclosed points, is especially useful. The extension of [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) is

$$
\mathbb C[t_1,t_2]\cong R[s]/(s^2+1),
$$

a free $R$-[module](../../../module-theory.md#module-mathematics) with basis $1,s$. At $\mathfrak p\in\operatorname{Spec}R$, with [residue field](../../../commutative-algebra.md#residue-field) $K=\kappa(\mathfrak p)$, the [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is

$$
\boxed{\pi^{-1}(\mathfrak p)_{\mathrm{sch}}
=\operatorname{Spec}\bigl(K[s]/(s^2+1)\bigr).}
$$

If $-1$ is a square in $K$, the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives $K\times K$, hence two points. Otherwise it is a quadratic [field extension](../../../algebra.md#field-extension), hence one point. The polynomial has no repeated root in [characteristic zero](../../../algebra.md#characteristic-zero), so all these [scheme-theoretic fibres](../../../ringed-space.md#scheme-theoretic-fibre) are [reduced schemes](../../../ringed-space.md#reduced-scheme). This also proves surjectivity. Conjugation acts on each two-point fibre by exchanging its points and fixes each one-point fibre. As a [finite morphism](../../../algebraic-geometry.md#finite-morphism), $\pi$ is closed, so its underlying topological space is the quotient by [complex conjugation](../../../complex-analysis.md#complex-conjugation). The fibre formula explains why a real closed point gives one complex point, whereas the generic point gives a single point with [residue field](../../../commutative-algebra.md#residue-field) $\mathbb C(t_1,t_2)$.

## 2

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

An [irreducible scheme](../../../ringed-space.md#irreducible-scheme) is a nonempty [scheme](../../../ringed-space.md#scheme) whose underlying [topological space](../../../topology.md#topological-space) cannot be expressed as the union of two proper closed subsets. Equivalently, any two nonempty [open subsets](../../../topology.md#open-set) meet. A [reduced scheme](../../../ringed-space.md#reduced-scheme) is one whose [local rings](../../../commutative-algebra.md#local-ring) have no nonzero [nilpotent elements](../../../commutative-algebra.md#nilpotent). Equivalently, every [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) has a [reduced ring](../../../commutative-algebra.md#reduced-ring) of [regular functions](../../../ringed-space.md#regular-function). We may define an [integral scheme](../../../ringed-space.md#integral-scheme) as a nonempty [scheme](../../../ringed-space.md#scheme) for which the [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) of every nonempty [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) is an [integral domain](../../../commutative-algebra.md#integral-domain). We shall show that this is equivalent to being reduced and irreducible. The nonempty convention matters: the empty [scheme](../../../ringed-space.md#scheme) is reduced but is not irreducible or integral.

For a [commutative ring](../../../commutative-algebra.md#commutative-ring) $A$, the [spectrum of a ring](../../../ringed-space.md#spectrum-of-a-commutative-ring) is reduced exactly when $A$ is a [reduced ring](../../../commutative-algebra.md#reduced-ring). One direction follows since [localization](../../../commutative-algebra.md#localization-of-a-ring) preserves reducedness. Conversely, if $a$ is a nonzero [nilpotent element](../../../commutative-algebra.md#nilpotent), choose a [prime ideal](../../../commutative-algebra.md#prime-ideal) containing its proper annihilator. Then $a/1$ cannot vanish at that [localization](../../../commutative-algebra.md#localization-of-a-ring), contradicting reducedness of its [local ring](../../../commutative-algebra.md#local-ring).

The [spectrum of a ring](../../../ringed-space.md#spectrum-of-a-commutative-ring) is irreducible exactly when its [nilradical](../../../commutative-algebra.md#nilradical) $N=\sqrt{(0)}$ is a [prime ideal](../../../commutative-algebra.md#prime-ideal). To see the essential implication directly, if $ab\in N$, then $D(a)\cap D(b)=D(ab)$ is empty. Irreducibility forces $D(a)$ or $D(b)$ to be empty, hence $a\in N$ or $b\in N$. Also $N$ is proper because the spectrum is nonempty. Conversely, if $N$ is a [prime ideal](../../../commutative-algebra.md#prime-ideal), the point $N$ has closure $V(N)=\operatorname{Spec}A$, so the spectrum is irreducible. Combining the two criteria gives

$$
\boxed{A\text{ is an integral domain}
\iff\operatorname{Spec}A\text{ is reduced and irreducible}.}
$$

Now suppose $X$ is reduced and irreducible. Every nonempty [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) is also reduced and irreducible: irreducibility passes to nonempty [open subsets](../../../topology.md#open-set), because their nonempty open subsets are nonempty opens of $X$. The affine criterion makes each [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) an [integral domain](../../../commutative-algebra.md#integral-domain), so $X$ is integral. Conversely, suppose all its nonempty affine [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) are [integral domains](../../../commutative-algebra.md#integral-domain). Their [localizations](../../../commutative-algebra.md#localization-of-a-ring) show that $X$ is reduced. If $X$ were reducible, there would be disjoint nonempty [open subsets](../../../topology.md#open-set); choose nonempty [affine open subschemes](../../../ringed-space.md#affine-open-subscheme) $U=\operatorname{Spec}A$ and $V=\operatorname{Spec}B$ inside them. Their disjoint union is itself an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $\operatorname{Spec}(A\times B)$. Since $A,B$ are nonzero, $(1,0)(0,1)=0$ contradicts the domain condition. Therefore

$$
\boxed{X\text{ is integral}\iff X\text{ is reduced and irreducible}.}
$$

The [generic point](../../../algebraic-geometry.md#generic-point) of an [integral scheme](../../../ringed-space.md#integral-scheme) $X$ is the unique point $\eta$ with $\overline{\{\eta\}}=X$. For existence, take a nonempty [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V=\operatorname{Spec}A$. Its point $(0)$ has closure containing $V$, which is dense in $X$, so its closure in $X$ is all of $X$. For uniqueness, both proposed [generic points](../../../algebraic-geometry.md#generic-point) lie in every nonempty [open subset](../../../topology.md#open-set), hence in $V$, where the only dense point is $(0)$. The [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) is

$$
K(X)=\mathcal O_{X,\eta}=\operatorname{Frac}(A).
$$

Here the [stalk](../../../ringed-space.md#stalk-of-a-sheaf) description shows that the [field of fractions](../../../commutative-algebra.md#field-of-fractions) is independent of the choice of nonempty [affine open subscheme](../../../ringed-space.md#affine-open-subscheme).

Every nonempty [open subscheme](../../../ringed-space.md#open-subscheme) $U$ contains $\eta$, so taking a [germ](../../../ringed-space.md#germ-of-a-sheaf-section) there defines $\Gamma(U,\mathcal O_X)\to K(X)$. If a section has zero germ, restrict it to any nonempty [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V\subseteq U$. Its image in $\operatorname{Frac}\Gamma(V,\mathcal O_X)$ is zero. Since this [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) is an [integral domain](../../../commutative-algebra.md#integral-domain), the section is zero on $V$. Such affines cover $U$, and the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) makes the section zero on $U$. Thus the [generic-point embedding of regular functions](../../../ringed-space.md#generic-point-embedding-of-regular-functions) is

$$
\boxed{\Gamma(U,\mathcal O_X)\hookrightarrow K(X).}
$$

For a [nonreduced reducible fibre between integral schemes](../../../ringed-space.md#nonreduced-reducible-fibre-between-integral-schemes), take both source and target to be the [affine line](../../../ringed-space.md#affine-line) over $\mathbb C$, and use the [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism)

$$
\mathbb C[t]\longrightarrow\mathbb C[x],\qquad t\longmapsto x^2(x-1)^2.
$$

Both [coordinate rings](../../../algebraic-geometry.md#coordinate-ring) are [integral domains](../../../commutative-algebra.md#integral-domain), so both [schemes](../../../ringed-space.md#scheme) are integral. At the target [closed point](../../../topology.md#closed-point) $t=0$, the [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) has ring

$$
\mathbb C[x]/\bigl(x^2(x-1)^2\bigr)
\cong\mathbb C[x]/(x^2)\times\mathbb C[x]/((x-1)^2),
$$

by the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem). Its underlying space has two distinct [closed points](../../../topology.md#closed-point), so it is reducible. The class of $x(x-1)$ is nonzero but has square zero, so it is not reduced. **Even a morphism between integral schemes can have a fibre consisting of two nonreduced double points.**

## 3

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The point to retain in the direct-image theorem is [quasi-compactness](../../../topology.md#compact-space) of inverse images of affine opens and of overlaps; no separation assumption has been supplied. The underlying space of a [Noetherian scheme](../../../ringed-space.md#noetherian-scheme) is Noetherian, so every [open subset](../../../topology.md#open-set) of $X$ is [quasi-compact](../../../topology.md#compact-space). Fix an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V=\operatorname{Spec}A$ of $Y$, put $W=f^{-1}V$, and choose a finite [open cover](../../../topology.md#open-cover) by [affine open subschemes](../../../ringed-space.md#affine-open-subscheme) $W=\bigcup_i U_i$. For each pair $i,j$, choose a finite affine cover $(W_{ij\ell})_\ell$ of $U_i\cap U_j$. Empty overlaps contribute no terms.

Write $M=\Gamma(W,\mathcal F)$. The [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) gives the [exact sequence](../../../homology.md#exact-sequence)

$$
0\longrightarrow M\longrightarrow
\prod_i\Gamma(U_i,\mathcal F)
\xrightarrow{\delta}
\prod_{i,j,\ell}\Gamma(W_{ij\ell},\mathcal F),
$$

where $\delta$ is the difference of the two restrictions to each overlap chart. All terms are $A$-[modules](../../../module-theory.md#module-mathematics) through $f$. For $a\in A$, the inverse image of $D(a)$ cuts each $U_i$ and $W_{ij\ell}$ by a [principal open subscheme](../../../ringed-space.md#principal-open-subscheme). Because $\mathcal F$ is a [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf), sections on these smaller affine charts are the corresponding [module localizations](../../../commutative-algebra.md#localization-of-a-module) at $a$. [Exactness of localization](../../../commutative-algebra.md#exactness-of-localization) and its commutation with finite products now identify the localized equalizer with the equalizer for the restricted cover. Thus

$$
\Gamma(f^{-1}D(a),\mathcal F)\cong M_a.
$$

The isomorphisms respect restrictions, proving $(f_*\mathcal F)|_V\cong\widetilde M$ on the basis of [principal open subschemes](../../../ringed-space.md#principal-open-subscheme). Since $V$ was arbitrary, **$f_*\mathcal F$ is a quasi-coherent sheaf**. The finite covers of overlaps are what allow the proof to work for nonseparated [Noetherian schemes](../../../ringed-space.md#noetherian-scheme); this is the [quasi-coherence of direct image under a quasi-compact quasi-separated morphism](../../../ringed-space.md#quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism).

For a [quasi-coherent sheaf](../../../ringed-space.md#quasi-coherent-sheaf) which is not coherent but has coherent [direct image](../../../ringed-space.md#direct-image-sheaf), use $f:\mathbb P^1_k\to\operatorname{Spec}k$ and

$$
\mathcal F=\bigoplus_{n=1}^{\infty}\mathcal O_{\mathbb P^1}(-1).
$$

This [infinite negative-twist sum with zero global sections](../../../projective-space.md#infinite-negative-twist-sum-with-zero-global-sections) is quasi-coherent: on each standard [affine chart](../../../ringed-space.md#affine-chart-of-a-variety) it is the sheaf associated with a direct sum of free rank-one [modules](../../../module-theory.md#module-mathematics). Its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) at every point, modulo the [maximal ideal](../../../commutative-algebra.md#maximal-ideal), is an infinite-dimensional [vector space](../../../vector-space.md). A finitely generated [module](../../../module-theory.md#module-mathematics) would have a finite-dimensional quotient, so $\mathcal F$ is not a [coherent sheaf](../../../ringed-space.md#coherent-sheaf).

Nevertheless, $\Gamma(\mathbb P^1,\mathcal O(-1))=0$. This follows from [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space), or directly by gluing on the two standard affine charts: if $z=t_1/t_0$, a section is a polynomial $p(z)$ on the first chart and $q(z^{-1})$ on the second with $p(z)=z^{-1}q(z^{-1})$, which forces both to vanish. [Global sections](../../../ringed-space.md#global-section) commute with this direct sum: they are the kernel of the difference map for the two-chart cover, and [direct sums](../../../vector-space.md#direct-sum) commute with that finite equalizer of [modules](../../../module-theory.md#module-mathematics). Hence

$$
\boxed{f_*\mathcal F=0,}
$$

which is coherent on $\operatorname{Spec}k$. Both [schemes](../../../ringed-space.md#scheme) in this example are Noetherian.

For a [finite morphism](../../../algebraic-geometry.md#finite-morphism), such an example is impossible. On an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V=\operatorname{Spec}A$ of the target, its inverse image is $\operatorname{Spec}B$, with $B$ a finite $A$-[module](../../../module-theory.md#module-mathematics). Write $\mathcal F|_{f^{-1}V}=\widetilde M$. Its [direct image](../../../ringed-space.md#direct-image-sheaf) corresponds to $M$ considered as an $A$-[module](../../../module-theory.md#module-mathematics). If the [direct image](../../../ringed-space.md#direct-image-sheaf) is coherent, $M$ is finitely generated over $A$. The same generators also generate it over $B$, because $A$ acts through $B$. Since $B$ is Noetherian, $\widetilde M$ is coherent. Conversely, a finite set of $B$-generators combined with a finite set of $A$-generators of $B$ gives finitely many $A$-generators of $M$. Thus [coherence reflected by finite direct image](../../../ringed-space.md#coherence-reflected-by-finite-direct-image) gives the stronger equivalence

$$
\boxed{\mathcal F\text{ coherent}\iff f_*\mathcal F\text{ coherent}
\quad(f\text{ finite}).}
$$

Finally, let $Y=\operatorname{Spec}k[x,y]$, let $X=Y\setminus\{(x,y)\}$ be the [punctured affine plane](../../../ringed-space.md#punctured-affine-plane), and let $j:X\hookrightarrow Y$ be the [open immersion](../../../ringed-space.md#open-immersion). Both are [integral schemes](../../../ringed-space.md#integral-scheme), but $j$ is not an [isomorphism of schemes](../../../ringed-space.md#isomorphism-of-schemes) because it omits a point. The cover $X=D(x)\cup D(y)$ gives

$$
\Gamma(X,\mathcal O_X)
=k[x,y]_x\cap k[x,y]_y=k[x,y]
$$

inside the [field of fractions](../../../commutative-algebra.md#field-of-fractions) $k(x,y)$. Indeed, in a reduced fraction, membership in the first [localization](../../../commutative-algebra.md#localization-of-a-ring) forces every denominator factor to be associated to $x$, while membership in the second forces it to be associated to $y$. [Unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain) and coprimality force the denominator to be a [unit](../../../algebra.md#unit-in-a-ring). By the theorem just proved, $j_*\mathcal O_X$ is quasi-coherent on the affine $Y$, hence determined by this [module](../../../module-theory.md#module-mathematics) of [global sections](../../../ringed-space.md#global-section). The natural map $\mathcal O_Y\to j_*\mathcal O_X$ corresponds to the identity of $k[x,y]$, so

$$
\boxed{j_*\mathcal O_X\cong\mathcal O_Y,}
$$

a [coherent sheaf](../../../ringed-space.md#coherent-sheaf). This is a concrete case of [codimension-two extension of regular functions on a normal variety](../../../ringed-space.md#codimension-two-extension-of-regular-functions-on-a-normal-variety).

## 4

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The intersection hypothesis says that $X$ is a [semi-separated scheme](../../../ringed-space.md#semi-separated-scheme). For an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V\subseteq X$, the intersection $V\cap U$ is affine. Restricting the given [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves) to it and applying the [affine module-sheaf equivalence](../../../ringed-space.md#affine-module-sheaf-equivalence) gives an [exact sequence](../../../homology.md#exact-sequence) of [global sections](../../../ringed-space.md#global-section):

$$
0\longrightarrow\Gamma(V\cap U,\mathcal M')
\longrightarrow\Gamma(V\cap U,\mathcal M)
\longrightarrow\Gamma(V\cap U,\mathcal M'')\longrightarrow0.
$$

These are exactly the sections on $V$ of the three [direct image sheaves](../../../ringed-space.md#direct-image-sheaf). Affine opens form a basis, and every section of the last sheaf on such a basis open lifts to the middle sheaf. This proves surjectivity as a [sheaf morphism](../../../algebraic-geometry.md#morphism-of-sheaves); left exactness of [direct image](../../../ringed-space.md#direct-image-sheaf) supplies the other positions. Hence **direct image preserves this short exact sequence**. The crucial ingredient is exactness of sections of [quasi-coherent sheaves](../../../ringed-space.md#quasi-coherent-sheaf) on an affine intersection; arbitrary [open immersions](../../../ringed-space.md#open-immersion) need not have this property.

For the cohomology comparison, every nonempty finite intersection

$$
U_{i_0\cdots i_p}=U_{i_0}\cap\cdots\cap U_{i_p}
$$

is affine. This follows by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction), intersecting the affine intersection already obtained with the next affine open. The restriction of $\mathcal F$ to it is quasi-coherent, so [vanishing of quasi-coherent cohomology on an affine scheme](../../../ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme) gives

$$
H^q(U_{i_0\cdots i_p},\mathcal F)=0\qquad(q>0).
$$

We now prove why this local vanishing gives the [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem), rather than identifying the two sorts of cohomology without a comparison.

Take a [flasque resolution](../../../ringed-space.md#flasque-resolution) $0\to\mathcal F\to\mathcal I^0\to\mathcal I^1\to\cdots$. Here a [flabby sheaf](../../../ringed-space.md#flasque-sheaf) has surjective restriction maps; its restrictions to open subsets are still flabby and have zero higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology). Form the [double complex](../../../homology.md#double-complex)

$$
C^{p,q}=\prod_{i_0<\cdots<i_p}
\Gamma(U_{i_0\cdots i_p},\mathcal I^q).
$$

The horizontal differential is the alternating restriction map $d_{\mathrm C}$; the vertical one $d_{\mathrm I}$ is induced by the resolution. They commute, so the total differential in bidegree $(p,q)$ is $d_{\mathrm C}+(-1)^p d_{\mathrm I}$ and has square zero. The [Čech resolution on a semi-separated scheme](../../../ringed-space.md#cech-resolution-on-a-semi-separated-scheme) uses precisely these intersections.

A [flabby sheaf](../../../ringed-space.md#flasque-sheaf) has zero positive [Čech cohomology](../../../ringed-space.md#cech-cohomology) for a finite [open cover](../../../topology.md#open-cover), and its degree-zero [Čech cohomology](../../../ringed-space.md#cech-cohomology) is its [global sections](../../../ringed-space.md#global-section). One way to establish this auxiliary fact is to use the exact augmented two-open complex

$$
0\to\Gamma(V\cup W,\mathcal I)
\to\Gamma(V,\mathcal I)\oplus\Gamma(W,\mathcal I)
\to\Gamma(V\cap W,\mathcal I)\to0.
$$

Exactness at the first two terms is the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom); the last map is onto because a section on the intersection extends to $V$. For the induction step, write $V$ for the union of all but the last open and $W$ for the last open. Separate Čech cochains according to whether their index list contains the last index. The resulting two-block complex compares the smaller cover of $V$ with its restricted cover of $V\cap W$, together with $\Gamma(W,\mathcal I)$ in degree zero. By induction those two smaller cover complexes have cohomology only in degree zero, where they give $\Gamma(V,\mathcal I)$ and $\Gamma(V\cap W,\mathcal I)$. The displayed two-open exact sequence then gives zero positive-degree cohomology for the full cover. This proves the auxiliary fact by induction on the number of opens. Thus horizontal cohomology of $C^{\bullet,q}$ consists only of $\Gamma(X,\mathcal I^q)$ in degree zero. Computing the cohomology of the total complex first horizontally therefore gives $H^n(X,\mathcal F)$, by the [resolution principle for sheaf cohomology](../../../ringed-space.md#resolution-principle-for-sheaf-cohomology).

On the other hand, vertical cohomology is

$$
H^q(C^{p,\bullet})
=\prod_{i_0<\cdots<i_p}H^q(U_{i_0\cdots i_p},\mathcal F),
$$

since the restricted [flasque resolutions](../../../ringed-space.md#flasque-resolution) compute cohomology on each intersection. The already established affine vanishing makes all rows with $q>0$ zero. The surviving row $q=0$ is exactly the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) $\check C^\bullet(\mathcal U,\mathcal F)$. Computing total cohomology first vertically therefore gives $\check H^n(\mathcal U,\mathcal F)$. These two computations are justified by the two filtrations of the first-quadrant [double complex](../../../homology.md#double-complex): in every total degree only finitely many terms occur, and the cover also bounds the horizontal degree. Their edge maps give the natural identification

$$
\boxed{\check H^p(\mathcal U,\mathcal F)\cong H^p(X,\mathcal F)\quad(p\geq0).}
$$

For negative degrees both groups are zero by convention. In particular, degree zero is the usual identification by the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom), not merely a comparison of dimensions.

## 5

↑ **Parent:** [Paper 13](paper-13.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For the [Sheaf of relative Kähler differentials](../../../ringed-space.md#sheaf-of-relative-kahler-differentials) on $X=\mathbb P^3_{\mathbb C}$, the cotangent form of the [Euler sequence](../../../algebraic-geometry.md#euler-sequence) is

$$
0\longrightarrow\Omega_{X/\mathbb C}
\longrightarrow\mathcal O_X(-1)^{\oplus4}
\xrightarrow{(t_0,t_1,t_2,t_3)}\mathcal O_X\longrightarrow0.
$$

The last arrow is onto because at least one homogeneous coordinate is invertible on each standard affine chart. Locally its kernel is the rank-three module generated by the differentials of the three affine coordinates, yielding the displayed [Sheaf of relative Kähler differentials](../../../ringed-space.md#sheaf-of-relative-kahler-differentials). The [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) gives $H^q(X,\mathcal O_X(-1))=0$ for every $q$, while $H^0(X,\mathcal O_X)=\mathbb C$ and its positive-degree groups vanish. The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) therefore gives the [cotangent-sheaf cohomology of projective space](../../../ringed-space.md#cotangent-sheaf-cohomology-of-projective-space) in this dimension:

$$
\boxed{H^q(X,\Omega_{X/W})\cong
\begin{cases}\mathbb C,&q=1,\\0,&q\ne1,\end{cases}
\qquad\chi(X,\Omega_{X/W})=-1.}
$$

The isomorphism for $q=1$ is the connecting map from the constant global sections of $\mathcal O_X$. The [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) is the alternating sum of dimensions, explaining the minus sign.

For the curve, put $S=\mathbb C[t_0,t_1,t_2,t_3]$. It is a [unique factorization domain](../../../algebra.md#unique-factorization-domain), so irreducibility of $F$ makes $(F)$ a [prime ideal](../../../commutative-algebra.md#prime-ideal). Also $F$ does not divide $G$: otherwise irreducibility of $G$ would make them associates, contrary to their distinct degrees. Thus the image of $G$ is a nonzero element of the [integral domain](../../../commutative-algebra.md#integral-domain) $S/(F)$. It follows that $(F,G)$ is a [regular sequence](../../../commutative-algebra.md#regular-sequence). Its [Koszul complex](../../../homology.md#koszul-complex) is an [exact sequence](../../../homology.md#exact-sequence), and graded sheafification gives

$$
0\longrightarrow\mathcal O_X(-12)
\xrightarrow{(-G,F)}\mathcal O_X(-5)\oplus\mathcal O_X(-7)
\xrightarrow{(F,G)}\mathcal O_X
\longrightarrow i_*\mathcal O_Z\longrightarrow0,
$$

where $i:Z\hookrightarrow X$ is the [closed immersion](../../../ringed-space.md#closed-immersion). The signs make the composite $F(-G)+GF=0$. The shifts come respectively from $5+7$, $5$, and $7$.

Let $\mathcal I_Z$ be the [ideal sheaf of a closed subscheme](../../../ringed-space.md#ideal-sheaf-of-a-closed-subscheme). Split this [Koszul resolution](../../../algebra.md#koszul-resolution) into

$$
0\to\mathcal O_X(-12)\to\mathcal O_X(-5)\oplus\mathcal O_X(-7)
\to\mathcal I_Z\to0,
\qquad
0\to\mathcal I_Z\to\mathcal O_X\to i_*\mathcal O_Z\to0.
$$

For all integers $d$, $H^1(X,\mathcal O_X(d))=H^2(X,\mathcal O_X(d))=0$. Also $H^1(X,\mathcal O_X)=H^2(X,\mathcal O_X)=0$. The two [long exact sequences in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology), together with [sheaf cohomology under a closed inclusion](../../../ringed-space.md#sheaf-cohomology-under-a-closed-inclusion), consequently identify

$$
H^1(Z,\mathcal O_Z)
\cong H^2(X,\mathcal I_Z)
\cong\ker\bigl(H^3(X,\mathcal O_X(-12))
\longrightarrow H^3(X,\mathcal O_X(-5))\oplus H^3(X,\mathcal O_X(-7))\bigr).
$$

By [Serre duality](../../../ringed-space.md#serre-duality), $H^3(X,\mathcal O_X(-m))\cong S_{m-4}^*$ for $m\geq4$. Counting degree-$d$ monomials in four variables gives $\dim S_d=\binom{d+3}{3}$. Thus the source has dimension $\binom{11}{3}=165$, and the two target spaces have dimensions $\binom{4}{3}=4$ and $\binom{6}{3}=20$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) proves the requested bound:

$$
\boxed{\dim_{\mathbb C}H^1(Z,\mathcal O_Z)\geq165-4-20=141.}
$$

In fact equality holds. Under the [Serre duality](../../../ringed-space.md#serre-duality) pairings, the dual of this map is

$$
S_1\oplus S_3\longrightarrow S_8,\qquad (a,b)\longmapsto-Ga+Fb.
$$

If $Ga=Fb$, primeness of $F$ and $F\nmid G$ imply $F\mid a$. But $a$ has degree one and $F$ has degree five, forcing $a=0$, and then $b=0$. The dual map is injective, so the original map is surjective and its kernel has dimension $141$. **Thus the lower bound is attained for every pair allowed in the question.** No smoothness assumption is needed. The [regular sequence](../../../commutative-algebra.md#regular-sequence) cuts out a [projective complete intersection](../../../ringed-space.md#projective-complete-intersection) of dimension one. Also $H^0(X,\mathcal I_Z)=H^1(X,\mathcal I_Z)=0$, by the negative twists and the intermediate cohomology vanishing in the first short exact sequence, so the second gives $H^0(Z,\mathcal O_Z)=\mathbb C$. This is the [genus of a complete-intersection space curve](../../../algebraic-geometry.md#genus-of-a-complete-intersection-space-curve): the first cohomology has dimension $141$, equal to its [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
