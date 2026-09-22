# Paper 27

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper27.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper27.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

We take $d\in\mathbb Q^\times$, as required for this rational [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve). The tangent at $O=(1:-1:0)$ is $X+Y=0$. Its intersection with the curve has $dZ^3=0$, so it meets the curve three times at $O$: the identity is an [inflection point of a plane cubic](../../../normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic).

For $P,Q$, let their chord meet the [diagonal cubic elliptic curve](../../../normalization-of-an-algebraic-curve.md#diagonal-cubic-elliptic-curve) at the third point $R$, using the tangent if $P=Q$ and counting [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity). Then join $R$ to $O$ and take the third intersection $S$. Define $P+Q=S$. Equivalently, three collinear intersection points satisfy $P+Q+R=O$.

Here inversion has the particularly simple form

$$
\boxed{-(X:Y:Z)=(Y:X:Z).}
$$

Indeed $P$, its displayed inverse, and $O$ lie on the same line, since swapping $X,Y$ preserves both the curve and $X+Y$. Thus **addition is the chord or tangent operation followed by swapping the first two coordinates**. The rule includes limiting cases involving $O$ and repeated intersections. Its [associativity](../../../group.md#associative-property) follows from the [elliptic curve group law from Riemann-Roch](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch): the identification $P\mapsto[P-O]$ with the degree-zero [Picard group](../../../ringed-space.md#picard-group) turns the line-intersection [Weil divisor](../../../algebraic-geometry.md#weil-divisor) relation into addition of [divisor classes](../../../algebraic-geometry.md#divisor-class). Since a line cuts a [Weil divisor](../../../algebraic-geometry.md#weil-divisor) linearly equivalent to $3O$, that relation is exactly the chord rule just described.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [Hessian criterion for flexes of a plane cubic](../../../normalization-of-an-algebraic-curve.md#hessian-criterion-for-flexes-of-a-plane-cubic) applied to the defining [polynomial](../../../polynomial.md) gives

$$
\det\begin{pmatrix}6X&0&0\\0&6Y&0\\0&0&6dZ\end{pmatrix}=216dXYZ.
$$

Consequently the [inflection points of a plane cubic](../../../normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic) on this curve are exactly its intersections with the three coordinate lines. Choose $r\in\overline{\mathbb Q}$ with $r^3=d$, and a primitive cube [root of unity](../../../algebra.md#root-of-unity) $\zeta$. The nine distinct [flexes of a diagonal cubic](../../../normalization-of-an-algebraic-curve.md#flexes-of-a-diagonal-cubic) are

$$
\boxed{(1:-\zeta^j:0),\quad(0:-r\zeta^j:1),\quad(-r\zeta^j:0:1),\qquad j=0,1,2.}
$$

With the chosen flex as identity, these points are precisely $E_d[3]$. A tangent cutting the [Weil divisor](../../../algebraic-geometry.md#weil-divisor) $3P$ gives $3(P-O)=0$; conversely $3(P-O)=0$ makes the hyperplane [Weil divisor](../../../algebraic-geometry.md#weil-divisor) equivalent to $3P$, which supplies a tangent with triple contact. This is the [three-torsion points are flexes of a plane cubic](../../../normalization-of-an-algebraic-curve.md#three-torsion-points-are-flexes-of-a-plane-cubic) correspondence.

On $Z=0$ only $O$ is rational, since the other cube [roots of unity](../../../algebra.md#root-of-unity) are not rational. On each other coordinate line a [rational point](../../../algebraic-geometry.md#rational-point) exists exactly when $d$ is a rational cube, and then exactly one does. Therefore

$$
\boxed{E_d(\mathbb Q)[3]\cong\begin{cases}\mathbb Z/3\mathbb Z,&d\in(\mathbb Q^\times)^3,\\0,&\text{otherwise}.\end{cases}}
$$

In particular the rational [torsion subgroup](../../../group-theory.md#torsion-subgroup) cannot contain two independent points of order $3$.

One can also determine the whole [rational torsion of a diagonal cubic](../../../normalization-of-an-algebraic-curve.md#rational-torsion-of-a-diagonal-cubic). First it is killed by $6$. To see this, use the [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) from (iii). At [primes](../../../number-theory.md#prime-number) $\ell\equiv2\pmod3$ outside the finite set containing $2,3$ and the prime divisors of the numerator and denominator of $d$, the cube map permutes $\mathbb F_\ell$, so

$$
\#E_d(\mathbb F_\ell)=1+\sum_{x\in\mathbb F_\ell}\bigl(1+\chi(x^3-432d^2)\bigr)=\ell+1,
$$

where the quadratic character is extended by $\chi(0)=0$, and the character sum vanishes after substituting $t=x^3-432d^2$. [Reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) injects the prime-to-$\ell$ part of rational torsion into this [finite group](../../../group.md#finite-group). This injection follows because multiplication by an [integer](../../../number-theory.md#integer) [prime](../../../number-theory.md#prime-number) to $\ell$ is invertible on the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve), and hence its reduction kernel has no such torsion.

For any [prime](../../../number-theory.md#prime-number) $q>3$, choose a good $\ell\equiv2\pmod3$ with $\ell\equiv1\pmod q$; the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) and the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) supply such [primes](../../../number-theory.md#prime-number) outside the finite bad [set](../../../set.md). Then $q\nmid\ell+1$, excluding $q$-torsion. Similarly good $\ell\equiv5\pmod{12}$ exclude order $4$, and good $\ell\equiv11\pmod{18}$ exclude order $9$. Thus every rational torsion point has order dividing $6$.

The inversion formula in (i) shows that the only possible nonidentity [rational point](../../../algebraic-geometry.md#rational-point) of order $2$ has $X=Y$ and $Z\ne0$. It exists precisely when $(X/Z)^3=-d/2$, that is, when $d/2$ is a rational cube. There is at most one such point. This condition and $d$ being a cube cannot hold together, since $2$ is not a rational cube. Combining it with the three-torsion calculation gives the full answer:

$$
\boxed{E_d(\mathbb Q)_{\mathrm{tors}}\cong\begin{cases}
\mathbb Z/3\mathbb Z,&d\in(\mathbb Q^\times)^3,\\
\mathbb Z/2\mathbb Z,&d/2\in(\mathbb Q^\times)^3,\\
0,&\text{otherwise}.
\end{cases}}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the invertible linear [projective transformation](../../../projective-space.md#projective-linear-transformation)

$$
(\mathcal X:\mathcal Y:\mathcal Z)=(-12dZ:-36d(X-Y):X+Y).
$$

The identity

$$
(X+Y)^3+3(X+Y)(X-Y)^2=4(X^3+Y^3)=-4dZ^3
$$

gives

$$
\mathcal Y^2\mathcal Z=1296d^2(X-Y)^2(X+Y)=\mathcal X^3-432d^2\mathcal Z^3.
$$

The transformation is invertible because $d\ne0$, and it sends $O$ to $(0:1:0)$. Hence it is an [isomorphism](../../../algebra.md#isomorphism) of the pointed [smooth projective curves](../../../projective-space.md#smooth-projective-curve), giving the required [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve):

$$
\boxed{y^2=x^3-432d^2.}
$$

For affine points $u=X/Z,v=Y/Z$, the transformation and its inverse are

$$
x=-\frac{12d}{u+v},\qquad y=-\frac{36d(u-v)}{u+v},\qquad
u=\frac{y-36d}{6x},\qquad v=\frac{-y-36d}{6x}.
$$

These formulae are interpreted in their stated affine charts; the [projective transformation](../../../projective-space.md#projective-linear-transformation) handles the exceptional points without any ambiguity.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Set $d=-7$. The affine rational pair $(u,v)=(2,-1)$ gives $P=(84,756)$ on the [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) $y^2=x^3-21168$. It is a point of infinite order: in the [rational torsion of a diagonal cubic](../../../normalization-of-an-algebraic-curve.md#rational-torsion-of-a-diagonal-cubic) classification, neither $-7$ nor $-7/2$ is a rational cube, so this curve has trivial rational [torsion subgroup](../../../group-theory.md#torsion-subgroup).

There is also a short direct torsion check specific to this curve. The [primes](../../../number-theory.md#prime-number) $5$ and $11$ are good and have point counts $6$ and $12$, respectively, because cubing is bijective in their [finite fields](../../../algebra.md#finite-field). Reduction at these two [primes](../../../number-theory.md#prime-number) bounds the entire rational torsion by order dividing $6$, including its possible $5$- and $11$-primary parts by reduction at the other [prime](../../../number-theory.md#prime-number). The flex calculation excludes order $3$, and the inversion calculation excludes order $2$. Hence $P$ is indeed nontorsion.

Every nonzero multiple $nP$ is distinct, and its inverse projective image has $Z\ne0$: the only [rational point](../../../algebraic-geometry.md#rational-point) at infinity on the diagonal cubic is its identity. Thus each yields a distinct rational pair. More explicitly, if $nP=(x_n,y_n)$ on the [Weierstrass model](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), then

$$
\boxed{u_n=\frac{y_n+252}{6x_n},\qquad v_n=\frac{252-y_n}{6x_n},\qquad u_n^3+v_n^3=7\quad(n\ge1).}
$$

Here $x_n\ne0$, since $x_n=0$ would require a rational square equal to $-21168$. For example the [elliptic-curve addition formula](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula) gives $2P=(28,28)$, which produces $(u_2,v_2)=(5/3,4/3)$. This proves **there are infinitely many rational pairs of cubes summing to seven**.

## 2

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Work with the usual commutative unital [ring](../../../commutative-algebra.md#ring) convention. Write $f(T)=a_1T+a_2T^2+\cdots$, where $a_1=f'(0)$ is a [unit](../../../algebra.md#unit-in-a-ring), and seek $g(T)=\sum_{n\ge1}b_nT^n$. Since $g$ has zero constant term, every coefficient of the composition of these [formal power series](../../../commutative-algebra.md#formal-power-series) involves only finitely many terms.

The linear coefficient forces $b_1=a_1^{-1}$. Suppose $b_1,\ldots,b_{n-1}$ have been chosen. The coefficient of $T^n$ in $f(g(T))$ is

$$
a_1b_n+C_n(a_2,\ldots,a_n;b_1,\ldots,b_{n-1}).
$$

Indeed the term involving $b_n$ can only come from $a_1g$: in $g^j$ with $j\ge2$, using a degree-$n$ term forces total degree at least $n+j-1>n$. Choose $b_n=-a_1^{-1}C_n$. This [recursive construction of a compositional inverse](../../../commutative-algebra.md#recursive-construction-of-a-compositional-inverse) uniquely gives $f\circ g=T$.

To check the other composition rather than assume it, construct $h(T)=\sum_{n\ge1}c_nT^n$ satisfying $h\circ f=T$. At degree $n$, its new coefficient is $c_na_1^n$ plus terms already determined; $a_1^n$ is a [unit](../../../algebra.md#unit-in-a-ring), so the same recursion works. Composition is associative, as can be checked coefficientwise, or after truncation modulo $T^{N+1}$ for every $N$. Therefore

$$
h=h\circ(f\circ g)=(h\circ f)\circ g=g.
$$

Consequently the [compositional inverse of a formal power series](../../../commutative-algebra.md#compositional-inverse-of-a-formal-power-series) is unique and satisfies

$$
\boxed{f(g(T))=g(f(T))=T.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem) asserts that $E(K)/mE(K)$ is finite for an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) over a [number field](../../../algebraic-number-theory.md#number-field) $K$ and an [integer](../../../number-theory.md#integer) $m\ge2$. The role of (i) is to make division by $m$ possible in the local [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve) whenever the [residue characteristic](../../../commutative-algebra.md#residue-characteristic) does not divide $m$.

Let $v$ be a finite place with [good reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) and $v\nmid m$. The [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve) is parametrized by $t=-x/y$ in the [maximal ideal](../../../commutative-algebra.md#maximal-ideal) of the local [valuation ring](../../../commutative-algebra.md#valuation-ring). Multiplication by $m$ is represented by an integral [formal power series](../../../commutative-algebra.md#formal-power-series)

$$
[m](T)=mT+\text{terms of degree at least }2.
$$

Its linear coefficient is a local [unit](../../../algebra.md#unit-in-a-ring). Part (i) supplies an integral compositional inverse. Both series converge on the [maximal ideal](../../../commutative-algebra.md#maximal-ideal), so multiplication by $m$ is a [bijection](../../../function.md#bijection) on the reduction kernel, over the [local field](../../../arithmetic.md#local-field) and over every finite [unramified extension](../../../arithmetic.md#unramified-extension).

This implies [unramified division torsors at good primes](../../../normalization-of-an-algebraic-curve.md#unramified-division-torsors-at-good-primes). For $P\in E(K)$, first divide its reduction by $m$ over the algebraic closure of the [residue field](../../../commutative-algebra.md#residue-field). Multiplication by $m$ on the reduced curve is [surjective](../../../algebra.md#surjective-function) and separable, so the chosen division point is defined over some finite residue extension. Smooth lifting gives a point $Q_0$ over the corresponding unramified local extension with the required reduction. The difference $P-mQ_0$ lies in the reduction kernel; the inverse series supplies $Q_1$ with $mQ_1=P-mQ_0$. Thus $Q=Q_0+Q_1$ divides $P$ over an [unramified extension](../../../arithmetic.md#unramified-extension). Applying the same reasoning to all reduced $m$-torsion points lifts all of $E[m]$, so every point of $[m]^{-1}P$ lies in the maximal [unramified extension](../../../arithmetic.md#unramified-extension). This excludes ramification outside a fixed [finite set](../../../set.md#finite-set) $S$ consisting of [primes](../../../number-theory.md#prime-number) of bad reduction and [primes](../../../number-theory.md#prime-number) over $m$.

For completeness, the remaining global finiteness step in the [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#kummer-theoretic-proof-of-the-weak-mordell-weil-theorem) is as follows. Choose $Q\in E(\overline K)$ with $mQ=P$. The [cocycle](../../../algebra.md#cocycle) $\sigma\mapsto\sigma Q-Q$ defines the [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve)

$$
E(K)/mE(K)\hookrightarrow H^1(K,E[m]).
$$

Changing $Q$ by an $m$-torsion point changes the [cocycle](../../../algebra.md#cocycle) by a [coboundary](../../../algebra.md#coboundary). A zero class makes $Q$ rational after that change, so the map is injective.

Let $L=K(E[m])$, fixed independently of $P$. Since the torsion is rational over $L$, the [cocycle](../../../algebra.md#cocycle) restricted to its [Galois group](../../../galois-theory.md#galois-group) is a homomorphism into $E[m]$. Consequently $L(Q)/L$ is Galois of degree at most $m^2$, contains the entire division fibre, and is unramified outside $S$. Hence $[L(Q):K]\le m^2[L:K]$. There are only finitely many extensions of bounded degree unramified outside a fixed [finite set](../../../set.md#finite-set): local extensions of bounded degree have bounded [field discriminant](../../../algebraic-number-theory.md#field-discriminant) exponents, and the [Hermite–Minkowski theorem](../../../algebraic-number-theory.md#hermite-minkowski-theorem) then applies to the bounded global [field discriminants](../../../algebraic-number-theory.md#field-discriminant). Their finite Galois compositum $M$ contains every such division fibre; each $L(Q)$ is stable over $K$ because it contains $E[m]$ and the whole fibre above the rational point $P$. All the Kummer classes consequently factor through the fixed [finite group](../../../group.md#finite-group) $\operatorname{Gal}(M/K)$ with values in the fixed [finite group](../../../group.md#finite-group) $E[m]$. There are only finitely many such [cocycles](../../../algebra.md#cocycle), proving

$$
\boxed{E(K)/mE(K)\text{ is finite}.}
$$

Thus (i) provides the local division step that bounds ramification; the global arithmetic finiteness completes the argument.

## 3

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) $\phi:E_1\to E_2$ over a [field](../../../algebra.md#field) $K$ is a nonconstant morphism preserving the identity and addition. It is [surjective](../../../algebra.md#surjective-function) and finite: its image is a closed connected subgroup, and a nonconstant morphism of [smooth projective curves](../../../projective-space.md#smooth-projective-curve) is finite. The [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) is the degree of its induced extension of [function fields](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety). A [separable isogeny](../../../normalization-of-an-algebraic-curve.md#separable-isogeny) has degree equal to the number of geometric kernel points; in general the degree is the length of the finite kernel scheme, incorporating inseparability. The [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) multiplies under composition, and degree one means an [isomorphism](../../../algebra.md#isomorphism). In characteristic zero all [elliptic isogenies](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) are separable. In positive characteristic the [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) illustrates inseparability, while an [elliptic isogeny](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) of degree [prime](../../../number-theory.md#prime-number) to the characteristic is separable.

The [homomorphism group of elliptic curves](../../../normalization-of-an-algebraic-curve.md#homomorphism-group-of-elliptic-curves) includes the zero homomorphism, the constant identity map, and every nonzero member is an [elliptic isogeny](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves). The operations are pointwise addition and negation; for endomorphisms, composition also gives the [endomorphism ring of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve). We put $q(0)=0$ and $q(\phi)=\deg\phi$ otherwise. We now prove the [positive definiteness of degree on elliptic-curve homomorphisms](../../../normalization-of-an-algebraic-curve.md#positive-definiteness-of-degree-on-elliptic-curve-homomorphisms) in full.

Let $E=E_2$, and choose a [Weierstrass model](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve). Its coordinate $x$ has a double pole at $O$, and the generic fibre of $x$ consists of $P$ and $-P$. On $E\times E$ the rational function $x(P)-x(Q)$ therefore has [Weil divisor](../../../algebraic-geometry.md#weil-divisor)

$$
\Delta+\Delta_- -2V-2H,
$$

where $\Delta=\{P=Q\}$, $\Delta_-=\{P=-Q\}$, $V=\{O\}\times E$, and $H=E\times\{O\}$. The generic zeros on the two diagonals have multiplicity one, and the generic poles on $V,H$ have multiplicity two; their intersections have codimension two and add no [Weil divisor](../../../algebraic-geometry.md#weil-divisor) components. This argument also uses the general Weierstrass involution in characteristic $2$, where $-P$ need not mean changing just the sign of $y$.

For the sum and difference maps $a(P,Q)=P+Q$ and $s(P,Q)=P-Q$, the divisors $a^*(O)$ and $s^*(O)$ are $\Delta_-$ and $\Delta$. Consequently, for the degree-one [line bundle](../../../ringed-space.md#line-bundle) $L=\mathcal O_E(O)$,

$$
a^*L\otimes s^*L\cong\operatorname{pr}_1^*(L^{\otimes2})\otimes\operatorname{pr}_2^*(L^{\otimes2}).
$$

Pull back along $P\mapsto(\phi(P),\psi(P))$ and take degrees of [line bundles](../../../ringed-space.md#line-bundle) on $E_1$. A nonconstant map pulls back $L$ to degree equal to its degree, while a constant map pulls it back to a trivial bundle of degree zero. We obtain the [degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law)

$$
\boxed{q(\phi+\psi)+q(\phi-\psi)=2q(\phi)+2q(\psi).}
$$

Using the line-bundle identity is important: it still restricts correctly when $\phi=\psi$ or $\phi=-\psi$, when restriction of the displayed rational function would be identically zero.

Since $q(-\phi)=q(\phi)$, applying the identity to $n\phi$ and $\phi$ gives the second-difference recursion

$$
q((n+1)\phi)+q((n-1)\phi)=2q(n\phi)+2q(\phi).
$$

Starting from $q(0)=0$ and $q(\phi)$ yields $q(n\phi)=n^2q(\phi)$ for all [integers](../../../number-theory.md#integer) $n$. Define

$$
B(\phi,\psi)=\frac{q(\phi+\psi)-q(\phi-\psi)}4
=\frac{q(\phi+\psi)-q(\phi)-q(\psi)}2.
$$

It is symmetric and odd in each variable. Applying the parallelogram identity to the four terms in its first expression gives

$$
B(u+w,v)+B(u-w,v)=2B(u,v).
$$

Interchanging $u,w$ and using oddness also gives $B(u+w,v)-B(u-w,v)=2B(w,v)$. Adding proves $B(u+w,v)=B(u,v)+B(w,v)$; symmetry proves additivity in the other variable. Thus $q$ is a [quadratic form](../../../linear-algebra.md#quadratic-form) with associated rational [bilinear form](../../../linear-algebra.md#bilinear-form) $B$.

Every nonzero homomorphism has positive degree, so $q(\phi)>0$ for $\phi\ne0$. The scaling identity also shows that the homomorphism [group](../../../group.md) is a [torsion-free group](../../../group.md#torsion-free-group). Hence $q$ extends to its rational [vector space](../../../vector-space.md). On the span of any finitely many rationally independent homomorphisms, the matrix of $B$ is rational. Positivity on nonzero rational vectors implies nonnegativity on real vectors by density. If the real matrix had a nontrivial kernel, its rational linear equations would have a nonzero rational solution, contradicting positivity. Thus its real extension is a [positive-definite quadratic form](../../../linear-algebra.md#positive-definite-quadratic-form). This establishes the requested positivity as well as the quadratic identities.

An important companion to degree is the [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny). Under $E\cong\operatorname{Pic}^0(E)$ via $P\mapsto[P-O]$, the pullback $\phi^*:\operatorname{Pic}^0(E_2)\to\operatorname{Pic}^0(E_1)$ defines $\widehat\phi:E_2\to E_1$. Divisor pushforward corresponds to $\phi$, and pushforward after pullback multiplies [divisor classes](../../../algebraic-geometry.md#divisor-class) by $n=\deg\phi$. Therefore $\phi\widehat\phi=[n]$. Composing shows that $\widehat\phi\phi-[n]$ takes values in the finite kernel of $\phi$; a morphism from a connected smooth curve into this finite scheme must be constant, and its identity value is zero. Thus

$$
\boxed{\widehat\phi\phi=[n],\qquad\phi\widehat\phi=[n],\qquad\deg\widehat\phi=n.}
$$

The last equality follows from $\deg[n]=n^2$, already proved by applying $q(m\phi)=m^2q(\phi)$ to the identity map. The [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) is unique, since the difference of two choices composed with $\phi$ would vanish and $\phi$ is [surjective](../../../algebra.md#surjective-function). It follows that being isogenous is an equivalence relation: duality supplies symmetry, and composition supplies transitivity. For a finite subgroup of geometric points of order [prime](../../../number-theory.md#prime-number) to the characteristic, the quotient curve and its quotient map give an [elliptic isogeny](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) with that kernel; in general one uses finite subgroup schemes. This is the geometric source of explicit descent maps, including the [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) in Question 4.

Finally [elliptic isogenies](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) preserve the rational [rank of an abelian group](../../../group.md#rank-of-an-abelian-group) over a [number field](../../../algebraic-number-theory.md#number-field). Their dual compositions are multiplication by $n$, so after tensoring the [rational point](../../../algebraic-geometry.md#rational-point) [groups](../../../group.md) with $\mathbb Q$ the [elliptic isogeny](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) becomes invertible. For a single curve, its endomorphism algebra in characteristic zero is $\mathbb Q$ or an imaginary quadratic [field](../../../algebra.md#field), giving ordinary [integer](../../../number-theory.md#integer) multiplication or [complex multiplication](../../../algebraic-geometry.md#complex-multiplication). In positive characteristic a supersingular curve can instead have a quaternionic endomorphism algebra. The positive degree form controls the sizes of these homomorphisms, while duality makes their arithmetic and geometric properties accessible.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $K$ be a [number field](../../../algebraic-number-theory.md#number-field) and $E/K$ an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve). Heights measure the arithmetic size of points, and turn the finite quotient supplied by the [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem) into finite generation. For a [projective point](../../../projective-space.md#projective-point) $[X:Z]\in\mathbb P^1(K)$ define the [Absolute logarithmic Weil height](../../../algebraic-number-theory.md#absolute-logarithmic-weil-height)

$$
h([X:Z])=\frac1{[K:\mathbb Q]}\sum_v n_v\log\max(|X|_v,|Z|_v),
$$

using the usual normalized absolute values and local degrees $n_v=[K_v:\mathbb Q_v]$. The [product formula](../../../algebraic-number-theory.md#product-formula) makes this independent of scaling and of enlarging $K$. For a [Short Weierstrass form](../../../normalization-of-an-algebraic-curve.md#short-weierstrass-form) put $h_x(P)=h([x(P):1])$ and $h_x(O)=h([1:0])=0$. Over $\mathbb Q$, if $x=A/B$ in lowest terms, $h(x)=\log\max(|A|,|B|)$.

The finiteness property is [Northcott theorem](../../../algebraic-number-theory.md#northcott-theorem): for bounded height and bounded degree over $\mathbb Q$ there are only finitely many algebraic numbers. One sees the mechanism from the [height-Mahler measure formula](../../../algebraic-number-theory.md#height-mahler-measure-formula). If $\alpha$ has degree $d\le D$ and height at most $H$, its primitive integral [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) has [Mahler measure](../../../algebraic-number-theory.md#mahler-measure) $e^{dh(\alpha)}\le e^{DH}$. Expanding its product of linear factors bounds every coefficient by $2^De^{DH}$. Only finitely many integral [polynomials](../../../polynomial.md) satisfy this bound, and each has finitely many roots. Thus a height bound gives only finitely many $x$-coordinates in the fixed [number field](../../../algebraic-number-theory.md#number-field) $K$, and each gives at most two points of $E$, besides $O$.

To understand multiplication, the doubling formula gives

$$
x(2P)=\frac{x^4-2ax^2-8bx+a^2}{4(x^3+ax+b)}.
$$

Its homogeneous numerator and denominator have degree four. They have no common projective zero: at infinity the numerator is nonzero, and at a root of $f(t)=t^3+at+b$ the numerator equals $f'(t)^2$, since it is $f'(t)^2-8tf(t)$. Nonsingularity excludes a common root of $f,f'$. The coordinate doubling map is therefore a degree-four morphism of the [projective line](../../../finite-group-theory.md#projective-line).

The general [height growth under a morphism of the projective line](../../../normalization-of-an-algebraic-curve.md#height-growth-under-a-morphism-of-the-projective-line) is $h(\Phi(t))=d h(t)+O(1)$ for a fixed degree-$d$ morphism. Here is why the error is bounded independently of $t$. At a place $v$, normalize its homogeneous coordinates to have maximum norm $1$. The fixed homogeneous forms have uniformly bounded norm. They also have a positive lower bound: the normalized coordinate space is compact over $K_v$, and their common zero [set](../../../set.md) is empty. Outside finitely many places their coefficients are integral and their reduction has no common zero, making both bounds $1$. Homogeneity and summation over places then give the asserted height estimate. Consequently there is a fixed $C$ with

$$
|h_x(2P)-4h_x(P)|\le C\qquad(P\in E(K)).
$$

Define the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) by the conventional normalization

$$
\widehat h(P)=\frac12\lim_{n\to\infty}4^{-n}h_x(2^nP).
$$

The successive approximants differ by at most $C/(2\cdot4^{n+1})$, so the limit exists and

$$
\left|\widehat h(P)-\tfrac12h_x(P)\right|\le\frac C6,
\qquad \widehat h(2P)=4\widehat h(P),\qquad\widehat h(P)\ge0.
$$

Thus [canonical height](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) retains Northcott finiteness, while replacing the bounded-error doubling rule by an exact one.

We also need the [height parallelogram identity](../../../normalization-of-an-algebraic-curve.md#height-parallelogram-identity). It follows from the [symmetric-square proof of the naive height parallelogram estimate](../../../normalization-of-an-algebraic-curve.md#symmetric-square-proof-of-the-naive-height-parallelogram-estimate), which we give explicitly using the supplied addition formulae. For $x_i=X_i/Z_i$, the unordered pair $x(P+Q),x(P-Q)$ is represented by the binary quadratic $CT^2-BTS+AS^2$, where

$$
\begin{aligned}
A&=X_1^2X_2^2-2aX_1X_2Z_1Z_2-4b(X_1Z_1Z_2^2+X_2Z_2Z_1^2)+a^2Z_1^2Z_2^2,\\
B&=2(X_1X_2+aZ_1Z_2)(X_1Z_2+X_2Z_1)+4bZ_1^2Z_2^2,\\
C&=(X_1Z_2-X_2Z_1)^2.
\end{aligned}
$$

These forms define the [biquadratic morphism for elliptic sums and differences](../../../normalization-of-an-algebraic-curve.md#biquadratic-morphism-for-elliptic-sums-and-differences). They have no common zero. If $C=0$, the two projective coordinates agree. On the finite diagonal $x_1=x_2=t$, $B=4f(t)$ and $A=f'(t)^2-8tf(t)$, so simultaneous vanishing would violate nonsingularity. At $(\infty,\infty)$ the homogeneous $A$ is nonzero. This also handles $P=\pm Q$ and sums or differences equal to $O$, for which the affine fractions alone would be inappropriate.

The same local norm argument as above, now using bidegree $(2,2)$, gives

$$
h([A:B:C])=2h_x(P)+2h_x(Q)+O(1).
$$

On the other hand the binary quadratic is the product of two linear factors for $x(P+Q)$ and $x(P-Q)$. At nonarchimedean places coefficient maximum norms multiply exactly: scale each factor to norm $1$ and reduce; the product of the two nonzero residue [polynomials](../../../polynomial.md) remains nonzero. This is [multiplicativity of the nonarchimedean polynomial norm](../../../commutative-algebra.md#multiplicativity-of-the-nonarchimedean-polynomial-norm). At archimedean places the norms are comparable up to fixed constants, by the coefficient triangle inequality and [compactness](../../../topology.md#compact-space) of normalized linear factors. Therefore

$$
h([A:B:C])=h_x(P+Q)+h_x(P-Q)+O(1).
$$

Combining the estimates proves the naive-height parallelogram relation with a uniform error. Apply it to $2^nP,2^nQ$, divide by $2\cdot4^n$, and pass to the limit to obtain

$$
\boxed{\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).}
$$

As in the polarization argument of (a), this makes $\widehat h$ quadratic, with the [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing)

$$
\langle P,Q\rangle=\frac{\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)}2,
\qquad \widehat h(nP)=n^2\widehat h(P).
$$

A torsion point has [canonical height](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) zero because its multiples have bounded [naive height](../../../normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line). Conversely, if $\widehat h(P)=0$, then all $2^nP$ have bounded [naive height](../../../normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line). Northcott finiteness makes two equal, giving $(2^j-2^i)P=O$ for some $j>i$. Thus **[canonical height](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) vanishes exactly on torsion**. In particular the [torsion subgroup](../../../group-theory.md#torsion-subgroup) is finite, since the comparison with [naive height](../../../normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line) bounds the heights of all its points.

We can now prove the [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group). The [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem), as explained in Question 2(ii), makes $E(K)/2E(K)$ finite. Choose representatives $R_1,\ldots,R_s$ and put $M=\max_i\widehat h(R_i)$. Every $P$ can be written $P=2Q+R_i$. The parallelogram identity and nonnegativity give

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)\le\tfrac12\widehat h(P)+\tfrac12M.
$$

Iterating this [height descent](../../../normalization-of-an-algebraic-curve.md#height-descent-lemma) makes the height at step $n$ at most $M+2^{-n}\max(\widehat h(P)-M,0)$, so after finitely many steps it is at most $M+1$. There are only finitely many points of that height by Northcott and the naive-height comparison. Reversing $P=2Q+R_i$ shows that every point is an [integer](../../../number-theory.md#integer) combination of the finitely many representatives and this finite bounded-height [set](../../../set.md). Therefore

$$
\boxed{E(K)\text{ is finitely generated},\qquad E(K)\cong\mathbb Z^r\oplus E(K)_{\mathrm{tors}}.}
$$

On the resulting free part the [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing) is positive definite. Its nonnegativity extends from rational vectors to real vectors by density. If a nonzero real vector $v$ were in its kernel, in a basis of the free part round $nv$ to [integer](../../../number-theory.md#integer) vectors $z_n$. Their rounding errors are uniformly bounded, and $\widehat h(z_n)=\widehat h(z_n-nv)$ would be uniformly bounded. The vectors $z_n$ are unbounded and therefore include infinitely many distinct vectors, contradicting Northcott finiteness. Thus there is no real null vector. Heights consequently support quantitative point searches, tests of independence, and the [regulator of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#regulator-of-an-elliptic-curve), in addition to providing the descent that proves finite generation.

## 4

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [rational point](../../../algebraic-geometry.md#rational-point) of order $2$ can be moved to $(0,0)$, giving an integral model

$$
E:y^2=x(x^2+ax+b),\qquad b(a^2-4b)\ne0.
$$

Its [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent) partner and the [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) are

$$
E':Y^2=X(X^2-2aX+b'),\qquad b'=a^2-4b,
$$



$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),\qquad
\widehat\phi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right).
$$

The maps extend over the identity and $(0,0)$, have these two points as their respective kernels, and direct substitution and the doubling formula give $\widehat\phi\phi=[2]$ and $\phi\widehat\phi=[2]$.

Define the [two-torsion square-class homomorphisms](../../../normalization-of-an-algebraic-curve.md#two-torsion-square-class-homomorphism) by

$$
\alpha:E(\mathbb Q)\longrightarrow\mathbb Q^\times/(\mathbb Q^\times)^2,\qquad
\alpha(O)=1,\quad\alpha((0,0))=b,\quad\alpha((x,y))=x,
$$

and similarly $\alpha'$ for $E'$, using $b'$. To see the homomorphism property, intersect a line $y=mx+c$ with $E$. Its three $x$-coordinates have product $c^2$, since the resulting monic cubic has constant term $-c^2$. The third point is the negative of the sum of the first two, and negation preserves $x$, so the [square classes](../../../galois-theory.md#square-class) multiply as required. If the line passes through $(0,0)$, the other two coordinates have product $b$, giving exactly the prescribed exceptional value. Vertical lines and repeated intersections give the identity and tangent cases.

We also verify the kernel needed for descent:

$$
\ker\alpha=\widehat\phi E'(\mathbb Q),\qquad\ker\alpha'=\phi E(\mathbb Q).
$$

For a point on $E'$, the first coordinate of its image under $\widehat\phi$ is $Y^2/(4X^2)$, a square. Conversely, if $P=(s^2,y)$ has square $x$-coordinate, solving $x(\widehat\phi(X,Y))=s^2$ gives

$$
X^2-(2a+4s^2)X+b'=0.
$$

Its [discriminant](../../../polynomial.md#discriminant) is $16(s^4+as^2+b)=(4y/s)^2$, so it has rational nonzero roots $X=a+2s^2\pm2y/s$. Taking $Y=\pm2sX$ gives a point on $E'$; choose the signs so its image has second coordinate $y$. The exceptional point $(0,0)$ lies in the image exactly when $b$ is a square, as seen from the points with $Y=0$, $X=a\pm2\sqrt b$. This proves the first kernel formula. Applying the same argument to $E'$ and then rescaling the second partner by $(X,Y)\mapsto(X/4,Y/8)$ proves the second.

There are only finitely many candidate [square classes](../../../galois-theory.md#square-class). For a [rational point](../../../algebraic-geometry.md#rational-point) write $x=M/e^2$ and $y=N/e^3$, with $\gcd(M,e)=1$. These denominator forms follow because a negative [prime](../../../number-theory.md#prime-number) [valuation](../../../algebra.md#valuation) of $x$ makes the leading cubic term the unique lowest-valuation term, forcing that [valuation](../../../algebra.md#valuation) to be even. Then

$$
N^2=M(M^2+aMe^2+be^4).
$$

If a [prime](../../../number-theory.md#prime-number) divides $M$ but not $b$, the second factor is a [unit](../../../algebra.md#unit-in-a-ring) at that [prime](../../../number-theory.md#prime-number), so its [valuation](../../../algebra.md#valuation) in $M$ is even. Thus every class in $\alpha(E)$ has a signed squarefree representative $d\mid b$. This is the [prime-support bound in two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#prime-support-bound-in-two-isogeny-descent); the analogous candidates for $\alpha'(E')$ divide $b'$.

The class $d$ is realized by a nonexceptional [rational point](../../../algebraic-geometry.md#rational-point) precisely when its [quartic covering in a two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#quartic-covering-in-a-two-isogeny-descent)

$$
N^2=dU^4+aU^2V^2+(b/d)V^4
$$

has a [rational point](../../../algebraic-geometry.md#rational-point) with $UV\ne0$. Indeed substitution $x=d(U/V)^2$, $y=dUN/V^3$ gives the original equation, and conversely the square-class condition gives these parameters. Clearing denominators permits $U,V,N$ integral with $\gcd(U,V)=1$. The zero-coordinate cases account for the already known identity and two-torsion classes.

For clarity, the [two-isogeny rank formula](../../../normalization-of-an-algebraic-curve.md#square-class-index-formula-for-two-isogeny-descent) contains a factor $4$, even when $E$ has full rational two-torsion. Put $t=\#E(\mathbb Q)[2]$, which is $2$ or $4$, and let $r$ be the rank. From the two kernel formulas and $2E=\widehat\phi\phi E$,

$$
[E:2E]=\frac{\#\alpha(E)\,\#\alpha'(E')}{\delta},\qquad
\delta=[\ker\widehat\phi:\ker\widehat\phi\cap\phi E].
$$

Indeed the kernel of the induced map $E'/\phi E\to\widehat\phi E'/2E$ is $\ker\widehat\phi/(\ker\widehat\phi\cap\phi E)$. The intersection is $\phi(E[2])$, of size $t/2$, so $\delta=4/t$. The [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group) gives $[E:2E]=2^rt$. Therefore

$$
\boxed{2^r=\frac{\#\alpha(E)\,\#\alpha'(E')}4.}
$$

This gives a practical rank procedure. Enumerate the finitely many signed squarefree divisors of $b,b'$, and test their quartics over the reals and [local fields](../../../arithmetic.md#local-field) at $2$ and [primes](../../../number-theory.md#prime-number) dividing the relevant coefficients or [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant). These necessary local conditions give finite [Selmer group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#n-selmer-group) upper bounds. Search the remaining coverings for [rational points](../../../algebraic-geometry.md#rational-point), or search the curves directly, to realize [square classes](../../../galois-theory.md#square-class) and obtain lower bounds. One can also exhibit independent points and check independence by the [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing). When the upper and lower bounds agree, the rank is determined. Local solubility alone does not guarantee a [rational point](../../../algebraic-geometry.md#rational-point), so a persistent gap can reflect a nontrivial [Tate–Shafarevich group](../../../normalization-of-an-algebraic-curve.md#tate-shafarevich-group) rather than a missing congruence test.

Now take $a=0$, $b=-p^2$ for an odd [prime](../../../number-theory.md#prime-number) $p$. The curve has four rational two-torsion points $O,(0,0),(p,0),(-p,0)$. Their images under $\alpha$ are $1,-1,p,-p$. The prime-support bound allows no other classes, so

$$
\alpha(E_p)=\{1,-1,p,-p\},\qquad\#\alpha(E_p)=4.
$$

Its partner is $E'_p:Y^2=X^3+4p^2X$. Any nonidentity [rational point](../../../algebraic-geometry.md#rational-point) with $X\ne0$ has $X>0$, because $X^2+4p^2>0$. Also the exceptional point has [square class](../../../galois-theory.md#square-class) $4p^2=1$. Thus its image is contained in the four positive candidate classes $\{1,2,p,2p\}$. The [rank bound for a prime congruent-number elliptic curve](../../../normalization-of-an-algebraic-curve.md#rank-bound-for-a-prime-congruent-number-elliptic-curve) follows:

$$
\boxed{2^{\operatorname{rank}E_p(\mathbb Q)}=\#\alpha'(E'_p)\le4,\qquad\operatorname{rank}E_p(\mathbb Q)\le2.}
$$

For an exact rank-one example, take $p=5$. The point $(X,Y)=(5,25)$ on $E'_5:Y^2=X^3+100X$ realizes the class $5$. The [five-adic obstructions for the congruent-number isogeny covers](../../../normalization-of-an-algebraic-curve.md#five-adic-obstructions-for-the-congruent-number-isogeny-covers) exclude the other two possible nontrivial classes. For $d=2$, the quartic is

$$
N^2=2U^4+50V^4,\qquad\gcd(U,V)=1.
$$

Modulo $5$, if $5\nmid U$ the right side is $2$, a nonsquare. Hence $U=5U_1$ and $N=5N_1$; primitivity gives $5\nmid V$. Dividing by $25$ then gives $N_1^2=50U_1^4+2V^4\equiv2\pmod5$, again impossible. For $d=10$, the quartic is $N^2=10(U^4+V^4)$. At least one of $U,V$ is nonzero modulo $5$, and their fourth powers are $0$ or $1$, so their sum is $1$ or $2$ modulo $5$. The right side has five-adic [valuation](../../../algebra.md#valuation) $1$, impossible for a square. Thus $\alpha'(E'_5)=\{1,5\}$ exactly, and

$$
\boxed{p=5,\qquad\operatorname{rank}E_5(\mathbb Q)=1.}
$$

The [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) maps $(5,25)$ to $(25/4,-75/8)$ on $E_5$, giving an explicit [rational point](../../../algebraic-geometry.md#rational-point) associated with this rank-one computation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
