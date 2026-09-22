# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_22.pdf)

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
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
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

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For the first [algebraic curve](../../../algebraic-geometry.md#algebraic-curve), a [hyperbola](../../../geometry-and-topology.md#hyperbola), use the line $y=1+tx$ through $(0,1)$. Substitution and cancellation of the known intersection give $x((1-t^2)x-2t)=0$. Thus a [rational parametrization of an algebraic curve](../../../algebraic-geometry.md#rational-parametrization-of-an-algebraic-curve) is

$$
\boxed{x=\frac{2t}{1-t^2},\qquad y=\frac{1+t^2}{1-t^2}.}
$$

The identity $y^2-x^2=1$ follows immediately. Away from $(0,1)$ its inverse is $t=(y-1)/x$; the exceptional point is recovered at $t=0$. The other point with $x=0$, namely $(0,-1)$, corresponds to $t=\infty$, while $t=\pm1$ gives the points at infinity on the projective closure. This explains the exceptional parameters rather than discarding them.

For the second [algebraic curve](../../../algebraic-geometry.md#algebraic-curve), the [rational parametrization of an algebraic curve](../../../algebraic-geometry.md#rational-parametrization-of-an-algebraic-curve)

$$
\boxed{x=t^2,\qquad y=t^3}
$$

has inverse $t=y/x$ where $x\ne0$, and $t=0$ gives the [cusp](../../../algebraic-geometry.md#cusp-algebraic-geometry). Indeed, if $x\ne0$ and $y^2=x^3$, then $(y/x)^2=x$ and $(y/x)^3=y$. **Both curves admit rational parametrizations**, although the second has a singular point.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Here is an elementary [polynomial pencil with four square members](../../../polynomial.md#polynomial-pencil-with-four-square-members) argument. Suppose first that $u,v$ are linearly dependent. Their [coprimality of polynomials](../../../polynomial.md#coprime-polynomials) then forces both to be constant. Otherwise write the four distinct members as $L_j=\alpha_j u+\beta_jv=s_j^2$. They are nonzero and pairwise [coprime polynomials](../../../polynomial.md#coprime-polynomials): a common nonconstant factor of two members would divide both $u$ and $v$.

Put $d=\max(\deg u,\deg v)>0$. At most one member of the pencil has [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) smaller than $d$, since cancellation of its leading coefficient determines a unique projective pair. Choose a member $L_k$ of minimal degree $e$ and any independent member $L_l$ of degree $d$. The [polynomial](../../../polynomial.md)

$$
W=L_k^{\prime}L_l-L_kL_l^{\prime}
$$

is nonzero: otherwise the [rational function](../../../isolated-singularity.md#rational-function) $L_k/L_l$ would have zero [derivative](../../../calculus.md#derivative), hence would be constant in characteristic zero. Its degree is at most $d+e-1$; if both members have degree zero the original $d>0$ assumption has already failed.

Replacing this pair by any other independent pair changes $W$ only by a nonzero scalar. Since $L_j=s_j^2$, each $s_j$ divides $W$. The pairwise [coprimality of polynomials](../../../polynomial.md#coprime-polynomials) therefore gives $\prod_j s_j\mid W$. But three members have degree $d$, so

$$
\deg W\ \geq\sum_{j=1}^4\deg s_j
\ \geq\frac{3d+e}{2}
\ >d+e-1,
$$

a contradiction. **Consequently $u$ and $v$ are constant.** The possibility that a member is zero was already covered by linear dependence.

To apply this to an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), complete the square in its [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) and work over $\mathbb C$. Nonsingularity gives three distinct roots $e_1,e_2,e_3$, so the equation becomes $y^2=\prod_{j=1}^3(x-e_j)$. A nonconstant [rational parametrization of an algebraic curve](../../../algebraic-geometry.md#rational-parametrization-of-an-algebraic-curve) would have $x=u/v$ with [coprime polynomials](../../../polynomial.md#coprime-polynomials). Clearing denominators gives

$$
(yv^2)^2=v(u-e_1v)(u-e_2v)(u-e_3v).
$$

The four factors are pairwise [coprime polynomials](../../../polynomial.md#coprime-polynomials). A [rational function](../../../isolated-singularity.md#rational-function) whose square is a [polynomial](../../../polynomial.md) is itself a [polynomial](../../../polynomial.md), by comparing numerator and denominator in lowest terms. [Unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain), and the fact that every nonzero complex constant has a square root, make each of these four factors a square in $\mathbb C[t]$. They correspond to four distinct projective pairs. The result just proved forces $u,v$ to be constant, and the equation then forces $y$ to be constant as well. **This proves the [nonparametrizability of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#nonparametrizability-of-an-elliptic-curve).**

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Let $C$ be the projective cubic of a [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), allowing its [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) to vanish, and let $O=[0:1:0]$. Use only the [smooth locus of a variety](../../../algebraic-geometry.md#smooth-locus-of-a-variety) $C_{\mathrm{sm}}(K)$: the singular point, if present, is excluded. For $P,Q$, intersect their chord with $C$, using the tangent if $P=Q$ and counting [intersection multiplicity](../../../algebraic-geometry.md#intersection-multiplicity). If the third intersection is $R$, define $P+Q=-R$, where

$$
-(x,y)=(x,-y-a_1x-a_3)
$$

in general [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) coordinates. The line through $R$ and $O$ gives this reflection. A vertical chord gives $P+(-P)=O$, and the tangent at $O$ meets $C$ three times at $O$, so $O$ is the identity. The construction is symmetric in $P,Q$. It stays in the nonsingular locus: a line through a singular point has intersection multiplicity at least two there, and therefore cannot also contain two smooth intersections counted with multiplicity.

For the nonsingular case, prove [associativity](../../../group.md#associative-property) by transporting a known [abelian group](../../../group.md#abelian-group) law. The [Abel-Jacobi map of a genus-one curve](../../../normalization-of-an-algebraic-curve.md#abel-jacobi-map-of-a-genus-one-curve)

$$
\iota:C\longrightarrow\operatorname{Pic}^0(C),\qquad P\longmapsto[P-O]
$$

is bijective over an [algebraic closure](../../../algebra.md#algebraic-closure). Indeed, the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) in [genus one](../../../normalization-of-an-algebraic-curve.md#genus-one-curve) says that every [divisor class](../../../algebraic-geometry.md#divisor-class) of degree one has a unique effective representative consisting of one point: existence follows from $\ell(D)=1$, and uniqueness follows because two distinct representatives would produce a degree-one map to the [projective line](../../../finite-group-theory.md#projective-line), impossible for a [genus one curve](../../../normalization-of-an-algebraic-curve.md#genus-one-curve). Subtracting $O$ gives the claimed bijection.

Any line section represents the same [divisor class](../../../algebraic-geometry.md#divisor-class) as $3O$, including tangencies. Thus $P+Q+R\sim3O$ as [divisors on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve), while the vertical line gives $R+(-R)+O\sim3O$. Hence

$$
\iota(P+Q)=\iota(P)+\iota(Q).
$$

Addition in the [Picard group](../../../ringed-space.md#picard-group) is associative, so

$$
\boxed{(P+Q)+S=P+(Q+S).}
$$

The [chord-and-tangent group law](../../../normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law) is defined over $K$, so the [group operation](../../../group.md#group-operation) restricts to the $K$-[rational points](../../../algebraic-geometry.md#rational-point).

For completeness, a singular [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) produces the [smooth-locus group of a singular Weierstrass cubic](../../../normalization-of-an-algebraic-curve.md#smooth-locus-group-of-a-singular-weierstrass-cubic), not an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve). Over an [algebraic closure](../../../algebra.md#algebraic-closure), its [normalization of an algebraic curve](../../../normalization-of-an-algebraic-curve.md) is the [projective line](../../../finite-group-theory.md#projective-line); deleting the two preimages of a [nodal crossing](../../../complex-analysis.md#nodal-crossing) gives the [multiplicative algebraic group](../../../algebraic-geometry.md#multiplicative-algebraic-group), while deleting the single preimage of a [cusp](../../../algebraic-geometry.md#cusp-algebraic-geometry) gives the [additive group](../../../group.md#additive-group). For example, on $y^2=x^3$, the coordinate $u=x/y$, with $u(O)=0$, makes the smooth-locus law addition. On $y^2=x^2(x+1)$ in characteristic different from two, put $t=y/x$ and $z=(t+1)/(t-1)$, with $z(O)=1$; the chord relation gives $z(P)z(Q)z(R)=1$, so the group law is multiplication of $z$. A nonsplit node gives the corresponding form of the [multiplicative algebraic group](../../../algebraic-geometry.md#multiplicative-algebraic-group) over $K$. These descriptions also establish the singular-case group laws.

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\pi$ denote the [Frobenius isogeny of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) and write $N=\#E(\mathbb F_q)$. Its [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) is $q$. The [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) $1-\pi$ has differential equal to the identity because $d\pi=0$, so it is a [separable isogeny](../../../normalization-of-an-algebraic-curve.md#separable-isogeny). Its kernel consists precisely of the [rational points](../../../algebraic-geometry.md#rational-point) fixed by $\pi$, giving

$$
\deg(1-\pi)=N.
$$

We use the [degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law) for [isogenies of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves), with degree zero assigned to the zero map:

$$
\deg(f+g)+\deg(f-g)=2\deg f+2\deg g,\qquad \deg[n]=n^2.
$$

One explanation of the first identity is the [divisor proof of the degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law): on $E\times E$, the zero [divisor](../../../number-theory.md#divisor) of $x(P)-x(Q)$ is the sum of the diagonal and the graph of negation, while its pole [divisor](../../../number-theory.md#divisor) is twice each coordinate copy of $O$. Pulling the associated [line bundle](../../../ringed-space.md#line-bundle) identity back by $(f,g)$ and taking degrees gives the identity, including exceptional cases by the line-bundle formulation. This works for a general [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), including characteristic two; $x$ is the quotient coordinate for negation. Polarization therefore makes degree a [quadratic form](../../../linear-algebra.md#quadratic-form) on the [endomorphism ring of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve).

Set $a=q+1-N$, the [Trace of Frobenius](../../../normalization-of-an-algebraic-curve.md#trace-of-frobenius). The cross term is determined by $\deg(1-\pi)=1+q-a$, giving, for all integers $m,n$,

$$
\deg([m]-[n]\pi)=m^2-amn+qn^2\geq0.
$$

If $a^2>4q$, the real degree-two [polynomial](../../../polynomial.md) $X^2-aX+q$ is negative on a nonempty open interval. That interval contains a rational $m/n$, contradicting the displayed nonnegativity after multiplication by $n^2$. Thus $a^2\leq4q$. **Hasse's bounds are**

$$
\boxed{q+1-2\sqrt q\ \leq\#E(\mathbb F_q)\ \leq q+1+2\sqrt q.}
$$

The argument proves the [Hasse theorem for elliptic curves](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves) without assuming its bound in advance.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The squares in the [finite field](../../../algebra.md#finite-field) $\mathbb F_7$ are $0,1,2,4$. For $x=0,1,\ldots,6$, the values of $x^3-x+1$ and the numbers of possible $y$ are respectively

$$
\begin{array}{c|rrrrrrr}
x&0&1&2&3&4&5&6\\\hline
x^3-x+1&1&1&0&4&5&2&1\\
\#y&2&2&1&2&0&2&2
\end{array}
$$

Adding $O$ yields **$\#E(\mathbb F_7)=12$**. The [Trace of Frobenius](../../../normalization-of-an-algebraic-curve.md#trace-of-frobenius) is $a=8-12=-4$. The [trace of the square of an elliptic-curve endomorphism](../../../normalization-of-an-algebraic-curve.md#trace-of-the-square-of-an-elliptic-curve-endomorphism) is $a^2-2q=16-14=2$, so the [elliptic-curve point count over a finite field](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-point-count-over-a-finite-field) gives

$$
\boxed{\#E(\mathbb F_{49})=49+1-2=48.}
$$

For example, this trace identity follows from $\pi^2-[a]\pi+[q]=0$ and $\operatorname{tr}[q]=2q$.

One suitable second [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) is

$$
\boxed{E^{\prime}:y^2=x^3+3x+6\quad\text{over }\mathbb F_7.}
$$

Here $4\cdot3^3+27\cdot6^2\equiv2\pmod7$, so its [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) is nonzero. Its complete list of [rational points](../../../algebraic-geometry.md#rational-point) is $O,(3,0),(6,3),(6,4)$, obtained by checking the seven $x$-values. For $P=(6,3)$ the tangent slope is $1$ in $\mathbb F_7$, and the [elliptic-curve addition formula](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula) gives $2P=(3,0)$. Consequently $P$ has order four and **$E^{\prime}(\mathbb F_7)\cong\mathbb Z/4\mathbb Z$**.

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In this one-dimensional setting, a commutative [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) over a commutative [ring](../../../commutative-algebra.md#ring) $R$ is a [formal power series](../../../commutative-algebra.md#formal-power-series) $F(X,Y)\in R[[X,Y]]$ with

$$
F(X,0)=X,\quad F(0,Y)=Y,\quad F(X,Y)=F(Y,X),\quad
F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

In particular $F(X,Y)=X+Y+$ terms of total degree at least two. There is a unique [formal inverse](../../../normalization-of-an-algebraic-curve.md#formal-inverse) $i_F(T)=-T+O(T^2)$; coefficient recursion solves $F(T,i_F(T))=0$.

A morphism from [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) $F$ to $G$ is $f(T)\in TR[[T]]$ satisfying

$$
f(F(X,Y))=G(f(X),f(Y)).
$$

The [invertible morphism criterion for formal group laws](../../../normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws) is

$$
\boxed{f\text{ is an isomorphism}\quad\Longleftrightarrow\quad f^{\prime}(0)\in R^{\times}.}
$$

Necessity follows by differentiating $g\circ f=T$ at zero for an inverse $g$. Conversely, write $f(T)=a_1T+a_2T^2+\cdots$ with $a_1$ a [unit](../../../algebra.md#unit-in-a-ring). In constructing $g(T)=b_1T+b_2T^2+\cdots$, the coefficient of $T$ fixes $b_1=a_1^{-1}$; at degree $n$, the equation $f(g(T))=T$ has the form $a_1b_n+$ an already known expression $=0$. This determines every $b_n$ over $R$. The same construction gives an inverse on the other side, and uniqueness makes the two inverses agree. Finally apply $g$ to the morphism identity with $X=g(U),Y=g(V)$ to obtain

$$
g(G(U,V))=F(g(U),g(V)).
$$

Thus the inverse is itself a morphism of [formal group laws](../../../normalization-of-an-algebraic-curve.md#formal-group-law), not merely an inverse [formal power series](../../../commutative-algebra.md#formal-power-series). Over a general [ring](../../../commutative-algebra.md#ring), nonzero derivative is insufficient: it must be a [unit](../../../algebra.md#unit-in-a-ring).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

We use two precise facts about the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve). At a [prime](../../../number-theory.md#prime-number) $p$ of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve), its [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve) is identified by the [uniformizer](../../../commutative-algebra.md#uniformizer) $t=-x/y$ with the group $\widehat E(p\mathbb Z_p)$. For odd $p$ this group is torsion-free. To see the second fact, the integral [invariant differential of a formal group law](../../../normalization-of-an-algebraic-curve.md#invariant-differential-of-a-formal-group-law) has the form $(1+\sum_{j\geq1}c_jT^j)dT$, with $c_j\in\mathbb Z_p$. Integrating constructs the [formal logarithm](../../../normalization-of-an-algebraic-curve.md#formal-logarithm)

$$
\log_F(T)=T+\sum_{j\geq2}d_jT^j/j,\qquad d_j\in\mathbb Z_p.
$$

It is a [group homomorphism](../../../group-theory.md#group-homomorphism) to the [additive group](../../../group.md#additive-group). For $0\ne t\in p\mathbb Z_p$ and $j\geq2$,

$$
v_p(d_jt^j/j)\geq jv_p(t)-v_p(j)>v_p(t)
$$

when $p$ is odd. Hence the series converges and $v_p(\log_F(t))=v_p(t)$, so it is injective. The target has no nonzero torsion. Therefore reduction is injective on the entire rational [torsion subgroup](../../../group-theory.md#torsion-subgroup) at an odd [prime](../../../number-theory.md#prime-number) of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve), including its $p$-primary part.

For the present [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), $\Delta=64D^6$, so every odd $p\nmid D$ is a [prime](../../../number-theory.md#prime-number) of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve). If $p\equiv3\pmod4$, the [Legendre symbol](../../../number-theory.md#legendre-symbol) of $-1$ is $-1$. The values $x$ and $-x$ cancel in the sum of the [Legendre symbols](../../../number-theory.md#legendre-symbol) of $x^3-D^2x$, yielding

$$
\#E(\mathbb F_p)=p+1.
$$

The rational [torsion subgroup](../../../group-theory.md#torsion-subgroup) injects into each of these groups, so it is finite and its order $M$ divides every such $p+1$.

For any odd [prime](../../../number-theory.md#prime-number) $\ell$, the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) supplies infinitely many $p$ with $p\equiv3\pmod4$ and $p\equiv1\pmod\ell$. Discard the finitely many dividing $D$. Since $\ell\nmid p+1$, it cannot divide $M$. Similarly choose $p\equiv3\pmod8$, again avoiding $D$; then $v_2(p+1)=2$, so $M\mid4$.

There are already four rational [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion) points,

$$
O,\quad(0,0),\quad(D,0),\quad(-D,0),
$$

which are distinct because a squarefree integer $D$ is nonzero. Thus

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=E(\mathbb Q)[2]\cong(\mathbb Z/2\mathbb Z)^2.}
$$

**Its order is four.** In fact the argument works for every nonzero integer $D$; squarefreeness is not needed for this torsion conclusion.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use the [congruent number elliptic curve](../../../normalization-of-an-algebraic-curve.md#congruent-number-elliptic-curve) in the equivalent coordinates

$$
E_{15}:y^2=x^3-225x.
$$

The [rational point](../../../algebraic-geometry.md#rational-point) $P=(25,100)$ lies on it, since $25^3-225\cdot25=10000$. By the preceding [rational torsion of a congruent number curve](../../../normalization-of-an-algebraic-curve.md#rational-torsion-of-a-congruent-number-curve) result, every rational [torsion point of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve) has $y=0$ or is $O$. Thus $P$ is not a [torsion point of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve), and its positive multiples give infinitely many distinct [rational points](../../../algebraic-geometry.md#rational-point) with nonzero $y$.

For any such point $(x,y)$, put

$$
\boxed{a=\left|\frac{x^2-225}{y}\right|,\quad
b=\left|\frac{30x}{y}\right|,\quad
c=\left|\frac{x^2+225}{y}\right|.}
$$

The identity $(x^2-225)^2+(30x)^2=(x^2+225)^2$ proves that these positive rational numbers are the sides of a [right triangle](../../../geometry-and-topology.md#right-triangle). Their area is

$$
\frac{ab}{2}=15\left|\frac{x(x^2-225)}{y^2}\right|=15.
$$

All three sides are nonzero because a point with $y\ne0$ has $x\notin\{0,15,-15\}$. For $P$ the construction gives $(a,b,c)=(4,15/2,17/2)$.

It remains to ensure that infinitely many points do not describe only finitely many triangles. Given the ordered positive pair $b,c$, set $r=c/b$. Then $X=|x|$ satisfies

$$
X^2-30rX+225=0.
$$

There are at most two possible $X$, then at most two signs of $x$ and two signs of $y$. Thus each ordered triangle has at most eight preimages; allowing interchange of its legs still gives a finite number. **There are infinitely many distinct rational right triangles of area $15$.** This is the [infinitely many rational right triangles from a nontorsion point](../../../normalization-of-an-algebraic-curve.md#infinitely-many-rational-right-triangles-from-a-nontorsion-point) principle.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [height function](../../../algebraic-number-theory.md#height-function) measures arithmetic size, which is what makes an otherwise infinite descent terminate. For a [number field](../../../algebraic-number-theory.md#number-field) $K$, normalize absolute values to extend the standard real and $p$-adic ones, and write $n_v=[K_v:\mathbb Q_v]$. The logarithmic [projective height](../../../algebraic-number-theory.md#projective-height) is

$$
h([a_0:\cdots:a_s])=\frac1{[K:\mathbb Q]}\sum_v n_v\log\max_j|a_j|_v.
$$

The [product formula](../../../algebraic-number-theory.md#product-formula) makes it independent of the chosen homogeneous coordinates, and the local-degree normalization makes it independent of the [number field](../../../algebraic-number-theory.md#number-field) containing them. Over $\mathbb Q$, $h([a:b])=\log\max(|a|,|b|)$ for [coprime](../../../number-theory.md#coprime-integers) integer coordinates. Set $h_x(P)=h(x(P))$ on an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), with $h_x(O)=0$.

Two features are essential. First, the [Northcott theorem](../../../algebraic-number-theory.md#northcott-theorem) says that points of bounded [projective height](../../../algebraic-number-theory.md#projective-height) and bounded field degree form a finite set. For points on a fixed [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) over $K$, each $x$-coordinate has at most two preimages, so bounded $h_x$ gives finitely many points. Second, a degree-$d$ morphism of the [projective line](../../../finite-group-theory.md#projective-line) satisfies $h(f(z))=dh(z)+O(1)$, uniformly in $z$. The upper bound comes from evaluating its homogeneous [polynomials](../../../polynomial.md); for the lower bound, their lack of a common zero gives a resultant identity bounding the input coordinates by the output coordinates at each place. Summing the local bounds gives the asserted uniform constant.

The duplication map on the $x$-line has degree four. Nonsingularity ensures that its numerator and denominator have no common projective zero. Therefore

$$
h_x(2P)=4h_x(P)+O(1).
$$

Telescoping defines the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve)

$$
\widehat h(P)=\frac12\lim_{j\to\infty}4^{-j}h_x(2^jP),\qquad
\widehat h(P)=\tfrac12h_x(P)+O(1).
$$

The error in successive terms is bounded by a geometric series, proving convergence and the uniform bounded difference. It also gives $\widehat h(2P)=4\widehat h(P)$ and nonnegativity. The usual addition formula gives the approximate [height parallelogram identity](../../../normalization-of-an-algebraic-curve.md#height-parallelogram-identity) for $h_x$; equivalently, the unordered pair of sum and difference on the $x$-line has bidegree $(2,2)$. Applying that identity to $2^jP,2^jQ$ and passing to the limit gives

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

In particular $\widehat h(nP)=n^2\widehat h(P)$. Its polarization is the [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing), a positive semidefinite bilinear form even before finite generation has been proved. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for this pairing gives

$$
\widehat h(P-Q)\leq2\widehat h(P)+2\widehat h(Q).
$$

Also $\widehat h(P)=0$ precisely for [torsion points of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve): one direction follows from periodic multiples, and in the other direction all multiples have bounded $h_x$, so the [Northcott theorem](../../../algebraic-number-theory.md#northcott-theorem) makes two multiples equal. Bounded [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) likewise gives a finite set of $K$-[rational points](../../../algebraic-geometry.md#rational-point).

Now the [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem) gives finitely many representatives $R_1,\ldots,R_s$ for $E(K)/2E(K)$. Put $H=\max_i\widehat h(R_i)$. Write any point as $P=2Q+R_i$. Then

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)
\leq\tfrac12\widehat h(P)+\tfrac12H.
$$

Repeatedly applying this [height descent lemma](../../../normalization-of-an-algebraic-curve.md#height-descent-lemma) eventually reaches height at most $H+1$: after $j$ steps the height is at most $H+2^{-j}(\widehat h(P)-H)$. The set of points with height at most $H+1$ is finite. Reading the relations $P=2Q+R_i$ backwards shows that this finite set together with the $R_i$ generates $E(K)$. Consequently

$$
\boxed{E(K)\cong E(K)_{\mathrm{tors}}\oplus\mathbb Z^r,\qquad r<\infty.}
$$

**Heights turn weak Mordell-Weil finiteness into the Mordell-Weil theorem.** The [canonical height pairing](../../../normalization-of-an-algebraic-curve.md#canonical-height-pairing) subsequently equips the free part with a positive definite [quadratic form](../../../linear-algebra.md#quadratic-form), useful for bounding searches and measuring independent generators; this interpretation is a consequence of the proof, not an assumption used in the descent.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Classical [Kummer theory](../../../galois-theory.md#kummer-theory) relates extraction of $n$th roots to [Galois cohomology](../../../galois-theory.md#galois-cohomology). In characteristic zero the exact sequence

$$
1\longrightarrow\mu_n\longrightarrow\overline K^{\times}
\xrightarrow{z\mapsto z^n}\overline K^{\times}\longrightarrow1
$$

and [Hilbert theorem 90](../../../galois-theory.md#hilbert-s-theorem-90) identify $H^1(K,\mu_n)$ with $K^{\times}/K^{\times n}$. For an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), the corresponding [Kummer exact sequence of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-exact-sequence-of-an-elliptic-curve) is

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0.
$$

Multiplication by $n$ is surjective over the [algebraic closure](../../../algebra.md#algebraic-closure). If $nQ=P\in E(K)$, the cocycle $\sigma\mapsto\sigma Q-Q$ takes values in $E[n]$. Changing the choice of $Q$ changes it by a coboundary, and changing $P$ by an element of $nE(K)$ does not change its class. Conversely, a trivial cocycle class allows $Q$ to be adjusted by an $n$-torsion point to become $K$-rational. Thus the [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve) is an injection

$$
\delta:E(K)/nE(K)\hookrightarrow H^1(K,E[n]).
$$

This is the elliptic form of [Kummer theory](../../../galois-theory.md#kummer-theory). The full cohomology group need not be finite; the arithmetic restriction on these classes is essential.

Choose a finite set $S$ of places containing the archimedean places, the [primes](../../../number-theory.md#prime-number) over $n$, and all [primes](../../../number-theory.md#prime-number) of [bad reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#bad-reduction-of-an-elliptic-curve). At a finite place outside $S$, $E$ has [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) and $n$ is a [unit](../../../algebra.md#unit-in-a-ring). A division point of the reduction of $P$ exists over the algebraic closure of the [residue field](../../../commutative-algebra.md#residue-field). Smooth lifting gives a point over a finite [unramified extension](../../../arithmetic.md#unramified-extension) whose multiple differs from $P$ by an element of the [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve). In the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve), $[n](T)=nT+O(T^2)$ is an isomorphism by the [invertible morphism criterion for formal group laws](../../../normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws), and its integral inverse converges on the maximal ideal. Correcting that difference produces a division point in the maximal [unramified extension](../../../arithmetic.md#unramified-extension). Hence the [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve) class is unramified outside $S$.

To prove finiteness explicitly, choose a finite [Galois extension](../../../galois-theory.md#finite-galois-extension) $L/K$ containing all $E[n]$ and all $n$th roots of unity, and enlarge $S$ to include its ramified places. A basis of $E[n]\cong(\mathbb Z/n\mathbb Z)^2$ identifies it over $L$ with $\mu_n^2$. Classical [Kummer theory](../../../galois-theory.md#kummer-theory) then identifies

$$
H^1(L,E[n])\cong(L^{\times}/L^{\times n})^2.
$$

The restriction of every class in the image of $\delta$ belongs to $L(S_L,n)^2$, where the [S-unramified power class group](../../../normalization-of-an-algebraic-curve.md#s-unramified-power-class-group) is

$$
L(S_L,n)=\{[a]:v_{\mathfrak p}(a)\equiv0\pmod n\text{ for all }\mathfrak p\notin S_L\}.
$$

Indeed an unramified local [Kummer extension](../../../galois-theory.md#kummer-extension) at residue characteristic prime to $n$ has valuation divisible by $n$: in an unramified field containing a root, $n v(a^{1/n})=v(a)$ with integral valuations.

The [finiteness of S-unramified Kummer classes](../../../normalization-of-an-algebraic-curve.md#finiteness-of-s-unramified-kummer-classes) follows from the exact sequence

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/(\mathcal O_{L,S_L}^{\times})^n
\longrightarrow L(S_L,n)
\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[n]
\longrightarrow0.
$$

To see the final map, write the ideal of $a$ away from $S_L$ as $\mathfrak a^n$ and take the [ideal class](../../../algebraic-number-theory.md#ideal-class) of $\mathfrak a$. Its kernel is represented by an [S-unit](../../../algebra.md#s-unit), after division by an $n$th power; conversely an $n$-torsion [ideal class](../../../algebraic-number-theory.md#ideal-class) yields such an $a$. The [S-unit group](../../../algebra.md#s-unit-group) is finitely generated by the [Dirichlet unit theorem](../../../algebraic-number-theory.md#dirichlet-s-unit-theorem) together with the finitely many inverted [primes](../../../number-theory.md#prime-number). The [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) of the localized ring is a quotient of the finite ordinary [ideal class group](../../../algebraic-number-theory.md#ideal-class-group). Both outer groups are therefore finite.

Finally restriction has finite kernel: inflation-restriction puts it in the finite group $H^1(\operatorname{Gal}(L/K),E[n])$. Thus the image of $\delta$ has finite restriction image and finite kernel, and

$$
\boxed{\#(E(K)/nE(K))<\infty\qquad(n\geq2).}
$$

**This proves the weak Mordell-Weil theorem.** Combining it with the [height descent lemma](../../../normalization-of-an-algebraic-curve.md#height-descent-lemma) proves the full [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group). Local restrictions at every place refine the finite group used here to the [Selmer group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#n-selmer-group), which is useful for explicit descent calculations.

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Work in characteristic different from two, as in the number-field application below. Nonsingularity is equivalent to $b(a^2-4b)\ne0$. The chord through $P=(x,y)$ and $T=(0,0)$ has slope $y/x$. Using $y^2/x^2=x+a+b/x$ in the [elliptic-curve addition formula](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula) gives

$$
\boxed{x^{\prime}=\frac b x,\qquad y^{\prime}=-\frac{by}{x^2}.}
$$

These formulas hold for $P\ne O,T$; addition interchanges $O$ and $T$.

It follows that $\xi=x+a+b/x=y^2/x^2$ and $\eta=y(1-b/x^2)$. The relation is

$$
\boxed{\eta^2=\xi\bigl(\xi^2-2a\xi+a^2-4b\bigr).}
$$

For a direct verification, observe that

$$
(\xi-a)^2-4b=(x-b/x)^2,
\qquad
\eta^2=\frac{y^2}{x^2}(x-b/x)^2.
$$

Therefore the [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) is

$$
\boxed{\begin{aligned}
E^{\prime}&:Y^2=X(X^2-2aX+a^2-4b),\\
\phi(x,y)&=\left(x+a+\frac b x,\ y\left(1-\frac b{x^2}\right)\right),\\
\phi(O)&=\phi(T)=O.
\end{aligned}}
$$

The target [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) is nonsingular because its corresponding coefficient product is $16b(a^2-4b)\ne0$. The [rational map of projective varieties](../../../algebraic-geometry.md#rational-map-of-projective-varieties) extends over the exceptional points to a morphism of smooth projective [algebraic curves](../../../algebraic-geometry.md#algebraic-curve); at both $O$ and $T$ its affine coordinates tend to infinity, giving the displayed values. A nonconstant morphism between [elliptic curves](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) sending $O$ to $O$ is a [group homomorphism](../../../group-theory.md#group-homomorphism), so this is an [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves).

One can also see the quotient directly: translation by $T$ leaves $\xi,\eta$ invariant. The equation $x^2+(a-\xi)x+b=0$ makes the source [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) a degree-two extension of the target [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety); its nontrivial automorphism is translation by $T$. Equivalently, the [degree of an isogeny from its x-coordinate map](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny-from-its-x-coordinate-map) is two. The [kernel of an isogeny](../../../normalization-of-an-algebraic-curve.md#kernel-of-an-isogeny) is precisely $\{O,T\}$. **Thus $\phi$ is a separable isogeny of degree two.**

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

First compute the [Mordell-Weil group](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group) rank by [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent). Here

$$
E:y^2=x(x^2+i),\qquad E^{\prime}:Y^2=X(X^2-4i).
$$

The [two-isogeny formula](../../../normalization-of-an-algebraic-curve.md#two-isogeny-formula) gives $\phi:E\to E^{\prime}$. If $u=1+i$, then $u^4=-4$, and

$$
\theta:E\longrightarrow E^{\prime},\qquad(x,y)\longmapsto(u^2x,u^3y)
$$

is an isomorphism over $K$. Its $x$-coordinate multiplier $u^2$ is a square in $K$.

Use the [two-torsion square-class homomorphism](../../../normalization-of-an-algebraic-curve.md#two-torsion-square-class-homomorphism)

$$
\alpha:E(K)\longrightarrow K^{\times}/K^{\times2},\qquad
\alpha(P)=[x(P)],\quad\alpha(O)=1,\quad\alpha(T)=[i].
$$

For any [prime ideal](../../../commutative-algebra.md#prime-ideal) of the [Gaussian integers](../../../commutative-algebra.md#gaussian-integer), if $v(x)>0$, then $x^2+i$ is a [unit](../../../algebra.md#unit-in-a-ring) and $2v(y)=v(x)$; if $v(x)<0$, the term $x^3$ has strictly smallest valuation and $2v(y)=3v(x)$. Hence every valuation of $x$ is even. Since the [Gaussian integers](../../../commutative-algebra.md#gaussian-integer) form a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), dividing by a square leaves a [unit](../../../algebra.md#unit-in-a-ring). Their units are $\{1,-1,i,-i\}$, whose [square classes](../../../galois-theory.md#square-class) are $\{1,i\}$ because $-1=i^2$ and $i$ is not a square in $K$. For the latter assertion, $(a+bi)^2=i$ with $a,b\in\mathbb Q$ would imply $a^2=b^2$ and $2ab=1$, hence $a^2=1/2$, impossible for rational $a$. Thus

$$
\alpha(E(K))=\{1,[i]\}.
$$

Both classes occur, at $O$ and $T$. This is the [unit square-class bound for two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#unit-square-class-bound-for-two-isogeny-descent).

Define $\alpha^{\prime}$ on $E^{\prime}$ similarly, with $\alpha^{\prime}((0,0))=[-4i]=[i]$. Since $\theta$ multiplies nonexceptional $x$-coordinates by a square, and preserves the exceptional classes as well, its image is also $\{1,[i]\}$. The standard kernel identities in [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent) are

$$
\ker\alpha=\widehat\phi E^{\prime}(K),\qquad
\ker\alpha^{\prime}=\phi E(K).
$$

Here $\widehat\phi$ is the [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) and $\widehat\phi\phi=[2]$. These identities can be checked directly from the formulas: $x(\widehat\phi(X,Y))=(Y/(2X))^2$, and conversely a square $x$-coordinate lets the quadratic equation for a preimage be solved using the curve equation. For example, if $x=r^2\ne0$, the equation for $X$ is $X^2-(4x+2a)X+(a^2-4b)=0$, whose discriminant is $16(x^2+ax+b)=16(y/r)^2$; the $Y$-coordinate then follows from the dual formula. The exceptional points satisfy the same completed square-class criterion.

The [two-isogeny index formula over a number field](../../../normalization-of-an-algebraic-curve.md#two-isogeny-index-formula-over-a-number-field) keeps track of a small kernel factor:

$$
[E(K):2E(K)]
=\frac{\#\alpha(E(K))\,\#\alpha^{\prime}(E^{\prime}(K))}{\delta},
\qquad
\delta=[\ker\widehat\phi:\ker\widehat\phi\cap\phi E(K)].
$$

In this case $\ker\widehat\phi=\{O,T^{\prime}\}$, where $T^{\prime}=(0,0)$, and $T^{\prime}\notin\phi E(K)$ because $\alpha^{\prime}(T^{\prime})=[i]\ne1$. Thus $\delta=2$, and the index is $2\cdot2/2=2$. There is only one nonzero rational [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion) point on $E$: the other two would require $x^2=-i$, and $-i$ has the same nonsquare class as $i$. The [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group) now gives

$$
2^{r+1}=[E(K):2E(K)]=2,
$$

so **$r=0$**.

It remains to identify all torsion, rather than merely the rank. The [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) is $-64i^3$, so the [primes](../../../number-theory.md#prime-number) $(3)$ and $(2-i)$ have [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve), with residue characteristics three and five. By the supplied point-count information their reduction groups have orders that are powers of two. The [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) is injective on prime-to-residue-characteristic torsion. Every odd-primary torsion subgroup therefore injects into a group of two-power order at at least one of these two [primes](../../../number-theory.md#prime-number), and must be zero. All torsion is two-primary.

Finally, if a point had order four, its double would be $T$. The [elliptic-curve addition formula](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula) gives

$$
x(2P)=\frac{(x^2-i)^2}{4x(x^2+i)}.
$$

For $2P=T$ the denominator is nonzero, so $x^2=i$, impossible in $K$. A point of higher two-power order would have a multiple of order four, so it too is excluded. Thus the only torsion points are $O,T$. Together with rank zero,

$$
\boxed{E(\mathbb Q(i))=\{O,(0,0)\}\cong\mathbb Z/2\mathbb Z.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
