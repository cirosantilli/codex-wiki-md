# Paper 21

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper21.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper21.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group) gives $E(\mathbb Q)\cong E(\mathbb Q)_{\rm tors}\oplus\mathbb Z^r$. Move the rational point of order two to $(0,0)$ and clear denominators to obtain an integral [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve)

$$
E:y^2=x(x^2+ax+b),\qquad b(a^2-4b)\ne0.
$$

The [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) gives $E':Y^2=X(X^2-2aX+a^2-4b)$ and [dual isogenies](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) $\phi:E\to E'$, $\widehat\phi:E'\to E$ with $\widehat\phi\phi=[2]$. Compute the [torsion subgroup](../../../group-theory.md#torsion-subgroup) using [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) at several good primes, followed by [division polynomials of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#division-polynomials) to identify the possible points.

For the free part, use [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent). The [two-torsion square-class homomorphism](../../../normalization-of-an-algebraic-curve.md#two-torsion-square-class-homomorphism) is

$$
\alpha(O)=1,\qquad \alpha((0,0))=[b],\qquad \alpha((x,y))=[x]
$$

in $\mathbb Q^*/\mathbb Q^{*2}$, with [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $\widehat\phi E'(\mathbb Q)$; define $\alpha'$ on $E'$ similarly. The [prime-support bound in two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#prime-support-bound-in-two-isogeny-descent) restricts the first image to signed square-free divisors of $b$ and the second to those of $a^2-4b$. For each candidate $d$, solve its [two-isogeny descent quartic](../../../normalization-of-an-algebraic-curve.md#quartic-covering-in-a-two-isogeny-descent)

$$
N^2=dU^4+aU^2V^2+\frac bd V^4.
$$

Test [local solubility](../../../number-theory.md#local-solubility) at the real place and the relevant [p-adic fields](../../../arithmetic.md#p-adic-field), discard impossible classes, and search the surviving coverings for [rational points](../../../algebraic-geometry.md#rational-point). A point with $UV\ne0$ gives $x=d(U/V)^2$, $y=dUN/V^3$. Include the identity and rational [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion) cases separately. Once both rational images are determined, the [two-isogeny rank formula](../../../normalization-of-an-algebraic-curve.md#square-class-index-formula-for-two-isogeny-descent) gives

$$
2^r=\frac{\#\alpha(E(\mathbb Q))\,\#\alpha'(E'(\mathbb Q))}{4}.
$$

The point searches give explicit candidates for a basis. Their [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing) can certify independence; [Mordell-Weil saturation](../../../normalization-of-an-algebraic-curve.md#mordell-weil-saturation) and effective height bounds then certify that they generate the full free part. Rank alone does not certify generators of the whole [Mordell-Weil group](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group). If the rational images are not fully determined, the procedure instead supplies lower and upper bounds on the [rank of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#rank-of-an-elliptic-curve).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The obstruction is the [local-to-global gap in isogeny descent](../../../normalization-of-an-algebraic-curve.md#local-to-global-gap-in-isogeny-descent). A [two-isogeny descent quartic](../../../normalization-of-an-algebraic-curve.md#quartic-covering-in-a-two-isogeny-descent) can have points over $\mathbb R$ and every [p-adic field](../../../arithmetic.md#p-adic-field) without a [rational point](../../../algebraic-geometry.md#rational-point). Local tests compute an [isogeny Selmer group](../../../normalization-of-an-algebraic-curve.md#isogeny-selmer-group), which can strictly contain the rational-point quotient. For an [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) $\phi:E\to E'$, the comparison is

$$
0\longrightarrow E'(\mathbb Q)/\phi E(\mathbb Q)
\longrightarrow\operatorname{Sel}^{\phi}(E/\mathbb Q)
\longrightarrow\operatorname{Sha}(E/\mathbb Q)[\phi]
\longrightarrow0.
$$

The last group is the kernel of $\phi:\operatorname{Sha}(E/\mathbb Q)\to\operatorname{Sha}(E'/\mathbb Q)$, so it records elements of the [Tate–Shafarevich group](../../../normalization-of-an-algebraic-curve.md#tate-shafarevich-group) invisible to all local tests. Searching a locally soluble covering which has no [rational points](../../../algebraic-geometry.md#rational-point) never succeeds. Thus a [Selmer group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#n-selmer-group) gives an upper bound and found independent points give a lower bound, and these need not coincide. Higher descent can improve the bounds, but this particular procedure has no unconditional guarantee of closing every gap.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $E:y^2=x^3-17x$, the [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) gives $E':Y^2=X^3+68X$. By the [prime-support bound in two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#prime-support-bound-in-two-isogeny-descent), the image of the [two-torsion square-class homomorphism](../../../normalization-of-an-algebraic-curve.md#two-torsion-square-class-homomorphism) on $E$ lies in $\{1,-1,17,-17\}$. The identity gives $1$, $T=(0,0)$ gives $-17$, and $P=(-1,4)$ gives $-1$, since $(-1)^3-17(-1)=16$. The image is a [subgroup](../../../group.md#subgroup) of the [square-class group](../../../galois-theory.md#square-class-group-of-a-field), so their product $17$ occurs as well; explicitly $P+T=(17,68)$. Hence

$$
\alpha(E(\mathbb Q))=\{1,-1,17,-17\}.
$$

On $E'$, a nonzero affine point has $X>0$, because $Y^2=X(X^2+68)$. The only candidate [square classes](../../../galois-theory.md#square-class) are therefore $1,2,17,34$. The identity gives $1$, $T'=(0,0)$ gives $[68]=17$, and $(2,12)$ gives $2$, since $2^3+68\cdot2=144$. Their product $34$ occurs; adding $T'$ gives $(34,-204)$. Thus

$$
\alpha'(E'(\mathbb Q))=\{1,2,17,34\}.
$$

Both images have order four. The [two-isogeny rank formula](../../../normalization-of-an-algebraic-curve.md#square-class-index-formula-for-two-isogeny-descent) proves

$$
\boxed{2^r=\frac{4\cdot4}{4}=4,\qquad \operatorname{rank}E(\mathbb Q)=2.}
$$

This is the [rank-two elliptic curve with cubic x cubed minus seventeen x](../../../normalization-of-an-algebraic-curve.md#rank-two-elliptic-curve-with-cubic-x-cubed-minus-seventeen-x); all candidate classes are represented, so no unresolved [local-to-global gap in isogeny descent](../../../normalization-of-an-algebraic-curve.md#local-to-global-gap-in-isogeny-descent) remains in this computation.

## 2

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For each $x\in\mathbb F_p$, count the roots of $y^2=x^3+x^2+x+1$, and add the identity at infinity. A nonzero [quadratic residue](../../../number-theory.md#quadratic-residue) gives two roots, zero gives one, and a nonsquare gives none. Equivalently, with the [Legendre symbol](../../../number-theory.md#legendre-symbol) extended by $\chi_p(0)=0$,

$$
\#\widetilde E_p(\mathbb F_p)=p+1+\sum_{x\in\mathbb F_p}\chi_p(x^3+x^2+x+1).
$$

The numbers of affine $y$ values, in increasing $x$ order starting at zero, are

$$
\begin{array}{c|l|c}
p&\text{root counts for }x=0,\ldots,p-1&\#\widetilde E_p(\mathbb F_p)\\\hline
3&(2,2,1)&6\\
5&(2,2,1,1,1)&8\\
7&(2,2,2,0,2,2,1)&12\\
11&(2,2,2,0,0,0,0,2,0,0,1)&10
\end{array}
$$

so the answer is

$$
\boxed{(\#\widetilde E_3,\#\widetilde E_5,\#\widetilde E_7,\#\widetilde E_{11})=(6,8,12,10).}
$$

All four reductions are [smooth algebraic curves](../../../algebraic-geometry.md#smooth-algebraic-curve): the original PDF gives the [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) $-2^8$, so these odd primes are primes of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the [two-prime bound on rational elliptic torsion](../../../normalization-of-an-algebraic-curve.md#two-prime-bound-on-rational-elliptic-torsion) with the counts six at three and eight at five from [solution](#2/a/solution). For a [prime](../../../number-theory.md#prime-number) $\ell\ne3,5$, the $\ell$-primary [torsion subgroup](../../../group-theory.md#torsion-subgroup) injects into both reduced groups by [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve). Its order therefore divides the corresponding primary part of $\gcd(6,8)=2$. The three-primary subgroup injects into the group of order eight at five and is trivial; the five-primary subgroup injects into the group of order six at three and is trivial. Hence the entire rational [torsion subgroup](../../../group-theory.md#torsion-subgroup) has order at most two.

The factorization $x^3+x^2+x+1=(x+1)(x^2+1)$ supplies $T=(-1,0)$, a nonidentity point of order two under the [elliptic curve group law](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch). Therefore

$$
\boxed{E(\mathbb Q)_{\rm tors}=\{O,(-1,0)\}\cong\mathbb Z/2\mathbb Z.}
$$

The primary-component argument avoids assuming injectivity on residue-characteristic torsion.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [rational point](../../../algebraic-geometry.md#rational-point) $P=(0,1)$ lies on $E$ and is neither the identity nor $(-1,0)$. By [solution](#2/b/solution) these are all the rational [torsion points of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve). Hence **$P$ has infinite order and $E(\mathbb Q)$ is infinite**: its multiples $nP$ are distinct. No assertion about its being a generator or about the exact [rank of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#rank-of-an-elliptic-curve) is needed here.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**Only the prime two can ramify.** More precisely, every field $\mathbb Q(P_n)$ is [unramified](../../../arithmetic.md#unramified-extension) at every odd [prime](../../../number-theory.md#prime-number); actual ramification at two depends on $P$ and the chosen division point. Use $[2^n]P_n=P$, as printed in the original PDF.

Fix an odd prime $p$ and put $N=2^n$. The [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) $-2^8$ gives [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at $p$, and $N$ is a unit in $\mathbb Z_p$. The [unramified division torsors at good primes](../../../normalization-of-an-algebraic-curve.md#unramified-division-torsors-at-good-primes) imply that all [division points of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#division-point-of-an-elliptic-curve) above $P$ are defined over finite [unramified extensions](../../../arithmetic.md#unramified-extension) of $\mathbb Q_p$. Here is a direct lifting proof, which does not require $P$ to have integral affine coordinates.

Properness gives a reduction $\widetilde P$. Choose a point $\overline Q$ with $[N]\overline Q=\widetilde P$ over the algebraic closure of the [residue field](../../../commutative-algebra.md#residue-field), and a finite residue extension containing it. Pass to the corresponding finite [unramified extension](../../../arithmetic.md#unramified-extension) $K/\mathbb Q_p$. The [surjectivity of good reduction over a local field](../../../normalization-of-an-algebraic-curve.md#surjectivity-of-good-reduction-over-a-local-field) lifts $\overline Q$ to $Q_0\in E(K)$. Its error $[N]Q_0-P$ lies in the [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve). The [prime-to-residue-characteristic multiplication on a formal group](../../../normalization-of-an-algebraic-curve.md#prime-to-residue-characteristic-multiplication-on-a-formal-group) makes $[N]$ bijective on that kernel. Choose the unique kernel point $R$ with $[N]R=[N]Q_0-P$; then $Q=Q_0-R$ satisfies $[N]Q=P$ and has reduction $\overline Q$.

Every algebraic division point has some such reduction and is the unique lift in its division fibre: the difference of two lifts lies in the reduction kernel, which has no $N$-torsion. Thus every chosen $P_n$ lies in an unramified local extension. For every prime of its possibly non-Galois coordinate field above $p$, the [ramification index](../../../arithmetic.md#ramification-index) is one. Globally,

$$
\boxed{\mathbb Q(P_n)/\mathbb Q\text{ is unramified outside }\{2\}.}
$$

One cannot universally assert that two actually ramifies: $P=O$ and $P_n=O$ give the field $\mathbb Q$. It can ramify. For example, a half of $T=(-1,0)$ is

$$
Q=\left(-1+\sqrt2,\ 2\sqrt{\sqrt2-1}\right),\qquad [2]Q=T.
$$

The [elliptic curve group law](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch) verifies this by doubling. Its coordinate field contains $\mathbb Q(\sqrt2)$, which has [ramification in the quadratic extension generated by the square root of two](../../../arithmetic.md#ramification-in-the-quadratic-extension-generated-by-the-square-root-of-two), so the only possible bad prime does occur for this choice.

## 3

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) over $\mathbb Q$ has [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at $p$ if it admits an integral [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) over $\mathbb Z_p$ whose reduced projective cubic is a [smooth algebraic curve](../../../algebraic-geometry.md#smooth-algebraic-curve) over $\mathbb F_p$. Equivalently, its [Minimal Weierstrass equation](../../../normalization-of-an-algebraic-curve.md#minimal-weierstrass-equation) has a unit [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant), or its smooth proper model is an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) over the [valuation ring](../../../commutative-algebra.md#valuation-ring). The existence of an appropriate integral model matters: a nonminimal equation can have discriminant divisible by $p$ even when the curve has [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve). Equivalently,

$$
\boxed{E\text{ has good reduction at }p\iff v_p(\Delta_{\min})=0.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The supplied integral equation has [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) $\Delta=-11$. It therefore has [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at every $p\ne11$. At eleven its discriminant has [valuation](../../../algebra.md#valuation) one. Under a change of [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), discriminant valuations differ by a multiple of twelve. A good integral model would have valuation zero, which is impossible. This is the [discriminant valuation obstruction to good reduction](../../../normalization-of-an-algebraic-curve.md#discriminant-valuation-obstruction-to-good-reduction); it also shows the displayed model is minimal at eleven. Hence

$$
\boxed{\text{The good primes are precisely all primes except }11.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose an integral [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) with unit [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant). For $P\in E(\mathbb Q_p)$, choose homogeneous coordinates $[X:Y:Z]$ in $\mathbb Z_p$ with at least one unit by multiplying all three coordinates by a common power of $p$. Define

$$
\operatorname{red}(P)=[\overline X:\overline Y:\overline Z]\in\widetilde E_p(\mathbb F_p).
$$

Two primitive integral representatives differ by a unit, so this is well-defined. Every point of the reduced cubic is a [nonsingular point of an algebraic curve](../../../algebraic-geometry.md#nonsingular-point-of-an-algebraic-curve), and the identity reduces to $[0:1:0]$. This definition includes points whose affine coordinates are nonintegral.

To prove the [good-reduction map respects elliptic addition](../../../normalization-of-an-algebraic-curve.md#good-reduction-map-respects-elliptic-addition), use the smooth proper integral model. The [elliptic curve group law](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch) is a morphism on this model, constructed by addition of degree-zero [divisor classes](../../../algebraic-geometry.md#divisor-class); it is defined even where an affine chord formula has a vanishing denominator. Passing to the [residue field](../../../commutative-algebra.md#residue-field) commutes with this morphism. Hence

$$
\operatorname{red}(P+Q)=\operatorname{red}(P)+\operatorname{red}(Q),
$$

so reduction is a [homomorphism of abelian groups](../../../group-theory.md#homomorphism-of-abelian-groups).

For surjectivity, the simple-root [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) says that if $g\in\mathbb Z_p[t]$, $g(t_0)\equiv0\pmod p$ and $g'(t_0)\not\equiv0\pmod p$, then there is a unique $t\in\mathbb Z_p$ with $t\equiv t_0\pmod p$ and $g(t)=0$. The point at infinity lifts to $O$. At an affine point $(\overline x,\overline y)$ of the reduced equation $F(x,y)=0$, being a [nonsingular point of an algebraic curve](../../../algebraic-geometry.md#nonsingular-point-of-an-algebraic-curve) means at least one [partial derivative](../../../calculus.md#partial-derivative) $F_x,F_y$ is nonzero. If $F_y\ne0$, fix any integral lift $x_0$ of $\overline x$ and apply the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) to $g(t)=F(x_0,t)$ to lift $\overline y$. If $F_x\ne0$, fix $y_0$ and lift $\overline x$ instead. This proves the [surjectivity of good reduction over a local field](../../../normalization-of-an-algebraic-curve.md#surjectivity-of-good-reduction-over-a-local-field) and gives

$$
\boxed{E(\mathbb Q_p)\twoheadrightarrow\widetilde E_p(\mathbb F_p)\text{ as abelian groups}.}
$$

## 4

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) over $k$ is a nonconstant morphism $\phi:E_1\to E_2$ defined over $k$ and preserving the identity. Such a morphism is a [group homomorphism](../../../group-theory.md#group-homomorphism): apply the [Mumford rigidity lemma](../../../abelian-variety.md#mumford-rigidity-lemma) to $\phi(P+Q)-\phi(P)-\phi(Q)$, whose restriction to either coordinate axis is zero. A nonconstant morphism of [smooth projective curves](../../../projective-space.md#smooth-projective-curve) is finite and surjective, so its [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) is the positive integer

$$
\deg\phi=[k(E_1):\phi^*k(E_2)].
$$

Degrees multiply under composition. A [separable isogeny](../../../normalization-of-an-algebraic-curve.md#separable-isogeny) has degree equal to the number of geometric points in its [kernel of an isogeny](../../../normalization-of-an-algebraic-curve.md#kernel-of-an-isogeny). In positive [characteristic of a field](../../../algebra.md#characteristic-of-a-field), inseparable isogenies also occur, for example the [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve); their total degree includes inseparable multiplicity, so counting geometric kernel points alone is insufficient. Every isogeny of degree $d$ has a [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) $\widehat\phi$ satisfying $\widehat\phi\phi=[d]$ and $\phi\widehat\phi=[d]$.

Pointwise addition and negation make the [homomorphism group of elliptic curves](../../../normalization-of-an-algebraic-curve.md#homomorphism-group-of-elliptic-curves) $H=\operatorname{Hom}_k(E_1,E_2)$ an [abelian group](../../../group.md#abelian-group). Its zero is the constant identity map; every other element is an isogeny, because its nonconstant image is the whole target curve. Define $q(0)=0$ and $q(\phi)=\deg\phi$ otherwise. We prove the [positive definiteness of degree on elliptic-curve homomorphisms](../../../normalization-of-an-algebraic-curve.md#positive-definiteness-of-degree-on-elliptic-curve-homomorphisms), including arbitrary characteristic.

Let $L=\mathcal O_{E_2}(O)$, a [line bundle associated to a divisor](../../../cartier-divisor.md#line-bundle-associated-to-a-divisor) of degree one. On $E_2\times E_2$ write $m(P,Q)=P+Q$, $d(P,Q)=P-Q$ and let $\pi_i$ be the projections. The [divisor proof of the degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law) gives

$$
m^*L\otimes d^*L\cong\pi_1^*L^{\otimes2}\otimes\pi_2^*L^{\otimes2}.
$$

Here is a direct justification. The degree-two Weierstrass coordinate $x$ has a double pole at $O$, and $x(P)=x(Q)$ precisely when $Q=P$ or $Q=-P$. Consequently

$$
\operatorname{div}(x(P)-x(Q))=D_++D_--2(\{O\}\times E_2)-2(E_2\times\{O\}),
$$

where $D_+$ is the diagonal and $D_-$ the graph of negation. Since $D_+=d^{-1}(O)$ and $D_-=m^{-1}(O)$, this [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) gives the displayed [line bundle](../../../ringed-space.md#line-bundle) identity. This remains valid in characteristic two: the general [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) of a [smooth algebraic curve](../../../algebraic-geometry.md#smooth-algebraic-curve) has a nontrivial generic involution $(x,y)\mapsto(x,-y-a_1x-a_3)$, so the two graphs still occur. This identity is also the symmetric-line-bundle form of the [Theorem of the square](../../../abelian-variety.md#theorem-of-the-square).

Pull back the bundle identity along $(\phi,\psi):E_1\to E_2\times E_2$ and take degrees of [line bundles](../../../ringed-space.md#line-bundle). For a nonzero map, $\deg(\phi^*L)=q(\phi)$; for a zero map its pullback is trivial and has degree zero. Thus the [degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law) is

$$
q(\phi+\psi)+q(\phi-\psi)=2q(\phi)+2q(\psi).
$$

Using bundles rather than pulling back the rational function itself is essential when $\phi=\pm\psi$, where that function can vanish identically. Negation preserves degree, so $q(-\phi)=q(\phi)$. Applying the parallelogram identity to $n\phi$ and $\phi$ gives the [quadratic degree recursion for elliptic multiplication](../../../normalization-of-an-algebraic-curve.md#quadratic-degree-recursion-for-elliptic-multiplication), and induction from $q(0)=0$ yields $q(n\phi)=n^2q(\phi)$ for every integer $n$.

Define the [bilinear degree pairing for elliptic-curve homomorphisms](../../../normalization-of-an-algebraic-curve.md#bilinear-degree-pairing-for-elliptic-curve-homomorphisms) by

$$
B(\phi,\psi)=\frac{q(\phi+\psi)-q(\phi-\psi)}4
=\frac{q(\phi+\psi)-q(\phi)-q(\psi)}2.
$$

It is symmetric and odd in each argument. Two applications of the [parallelogram law](../../../linear-algebra.md#parallelogram-law) give

$$
\begin{aligned}
B(x+z,y)+B(x-z,y)&=2B(x,y),\\
B(x+z,y)-B(x-z,y)&=2B(z,y).
\end{aligned}
$$

Adding proves $B(x+z,y)=B(x,y)+B(z,y)$, and symmetry proves additivity in the other argument. Also $B(\phi,\phi)=q(\phi)$. Therefore $q$ is an integer-valued [quadratic form](../../../linear-algebra.md#quadratic-form). The integral polarization is $2B(\phi,\psi)=q(\phi+\psi)-q(\phi)-q(\psi)$; $B$ itself may be half-integral.

Finally $q(\phi)>0$ for every nonzero $\phi$, since an isogeny has positive finite degree. If $n\phi=0$ with $n\ne0$, the identity $q(n\phi)=n^2q(\phi)$ forces $\phi=0$, so $H$ is a [torsion-free abelian group](../../../group.md#torsion-free-abelian-group). On any finite-dimensional rational span in $H\otimes\mathbb Q$, the pairing has a rational matrix and is positive on every nonzero rational vector. By density it is nonnegative on real vectors; if that rational matrix were singular, its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) would contain a nonzero rational vector, contradicting strict positivity. Thus its real extension is a [positive-definite quadratic form](../../../linear-algebra.md#positive-definite-quadratic-form). This establishes the required positivity as well as the quadratic identity. For example, on the subgroup of multiplication maps $[n]$, $q([n])=n^2$; on the [endomorphism ring of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve) with [complex multiplication](../../../algebraic-geometry.md#complex-multiplication) it is the imaginary-quadratic field norm, explaining the lattice geometry behind isogeny degrees.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
