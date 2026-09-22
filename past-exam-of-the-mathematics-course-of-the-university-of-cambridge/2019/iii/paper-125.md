# Paper 125

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_125.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_125.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Hasse theorem for elliptic curves](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves) states that every [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) $E/\mathbb F_q$ satisfies

$$
\boxed{\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.}
$$

Let $\pi$ be the [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) and put $a=\operatorname{tr}(\pi)$. Its fixed points are exactly $E(\mathbb F_q)$, so separability of $1-\pi$ gives

$$
\#E(\mathbb F_q)=\deg(1-\pi)=1+q-a.
$$

The [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) is a nonnegative [quadratic form](../../../linear-algebra.md#quadratic-form) on the endomorphism ring, and for all integers $m,n$,

$$
\deg([m]+[n]\pi)=m^2+amn+qn^2\geq0.
$$

If $a^2>4q$, this quadratic polynomial has two real roots and takes a negative value at some rational $m/n$ between them, hence after clearing denominators at some integer pair $(m,n)$. Therefore $a^2\leq4q$, and substituting $a=q+1-\#E(\mathbb F_q)$ proves the bound. This is the [degree-form proof of the Hasse bound](../../../normalization-of-an-algebraic-curve.md#degree-form-proof-of-the-hasse-bound).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $x=0,1,2$, the value of $x^3-x-1$ is the nonsquare $2$ in $\mathbb F_3$. Thus the point at infinity is the only rational point and

$$
\#E(\mathbb F_3)=1,
\qquad a_3=3+1-1=3.
$$

The eigenvalues of the [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) are the roots

$$
\alpha,\beta=\frac{3\pm i\sqrt3}{2}=\sqrt3e^{\pm i\pi/6}
$$

of $T^2-3T+3$. The [elliptic-curve point count over a finite field](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-point-count-over-a-finite-field) gives

$$
\#E(\mathbb F_{3^r})=3^r+1-\alpha^r-\beta^r
=3^r+1-2\cdot3^{r/2}\cos(r\pi/6).
$$

The last term vanishes exactly when $r\pi/6\equiv\pi/2\pmod\pi$. Hence

$$
\boxed{\#E(\mathbb F_{3^r})=3^r+1\quad\Longleftrightarrow\quad r\equiv3\pmod6.}
$$

## 2

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

If $p\mid D$, square-freeness gives the cuspidal reduction $y^2=x^3$. Its nonsingular group is isomorphic to the [additive group](../../../group.md#additive-group) $\mathbb F_p$, so it is cyclic of order $p$.

Suppose $p\nmid D$. The reduction is an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve). Since $p\equiv3\pmod4$, $-1$ is a [quadratic nonresidue](../../../number-theory.md#quadratic-nonresidue). Pairing $x$ with $-x$ in the quadratic-character sum and using

$$
(-x)^3-D^2(-x)=-(x^3-D^2x)
$$

shows that the two contributions cancel. Therefore $\#\widetilde E(\mathbb F_p)=p+1$. The three roots $0,D,-D$ are distinct, so the full [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion) is rational. A cyclic group has at most two elements killed by $2$, hence $\widetilde E(\mathbb F_p)$ is noncyclic. Thus

$$
\boxed{\widetilde E_{\mathrm{ns}}(\mathbb F_p)\text{ is cyclic of order }p\text{ if }p\mid D,\text{ and noncyclic of order }p+1\text{ otherwise}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A one-dimensional commutative [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) over a ring $R$ is a series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,
\qquad F(X,Y)=F(Y,X),
\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

An isomorphism $u:F\to G$ is a series $u(T)\in TR[[T]]$ with a compositional inverse and

$$
u(F(X,Y))=G(u(X),u(Y)).
$$

The multiplication series is defined recursively by $[0]_F=0$, $[1]_F=T$ and $[n+1]_F=F([n]_F,T)$, with the [formal inverse](../../../normalization-of-an-algebraic-curve.md#formal-inverse) handling negative $n$. Its linear term is

$$
[n]_F(T)=nT+O(T^2).
$$

By the [invertible morphism criterion for formal group laws](../../../normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws), it is an isomorphism exactly when its linear coefficient $n$ is a unit of $R$. Indeed, when $n\in R^\times$, recursive coefficient comparison constructs a unique compositional inverse; applying the morphism identity for $[n]_F$ shows that the inverse also respects $F$. Conversely, an invertible series must have a unit linear coefficient. Therefore

$$
\boxed{[n]_F\text{ is an isomorphism}\quad\Longleftrightarrow\quad n\in R^\times.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A positive integer $D$ is a [congruent number](../../../normalization-of-an-algebraic-curve.md#congruent-number) when it is the area of a right triangle with positive rational side lengths. For a point $P=(x,y)$ with $y\ne0$ on

$$
E_D:y^2=x^3-D^2x,
$$

the formulas

$$
a=\frac{x^2-D^2}{y},
\qquad b=\frac{2Dx}{y},
\qquad c=\frac{x^2+D^2}{y}
$$

give $a^2+b^2=c^2$ and $ab/2=D$, after changing signs if necessary. Conversely, a rational right triangle of area $D$ gives

$$
x=\frac{D(a+c)}b,
\qquad y=\frac{2D^2(a+c)}{b^2},
$$

so these constructions are inverse up to the usual sign choices.

It remains to distinguish torsion. If an odd prime $\ell$ divided the order of a rational torsion point, choose by the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) a good prime $p\equiv3\pmod4$ for which $p\not\equiv-1\pmod\ell$. Part (a) gives $\#E_D(\mathbb F_p)=p+1$, while part (b), applied to the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve), makes reduction injective on $\ell$-power torsion because $\ell$ is a unit in $\mathbb Z_p$. This is impossible. Similarly, a good prime $p\equiv3\pmod8$ shows that the rational $2$-primary torsion has order at most four. Since

$$
O,(0,0),(D,0),(-D,0)
$$

already form the full rational [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion),

$$
E_D(\mathbb Q)_{\mathrm{tors}}\cong(\mathbb Z/2\mathbb Z)^2.
$$

The triangle construction uses exactly the points with $y\ne0$, which are therefore nontorsion. By the [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group), such a point exists exactly when the free part has positive rank. Hence

$$
\boxed{D\text{ is congruent}\quad\Longleftrightarrow\quad\operatorname{rank}E_D(\mathbb Q)\geq1.}
$$

## 3

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

On $y^2=x^3+5x^2+4x$, the slope through $P_1=(-1,0)$ and $P_2=(-2,2)$ is $-2$. The [elliptic-curve addition formula](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula) gives

$$
x(P_1+P_2)=(-2)^2-5-(-1)-(-2)=2,
\qquad y(P_1+P_2)=(-2)(-1-2)=6.
$$

For doubling $P_2$, the tangent slope is

$$
\lambda=\frac{3x^2+10x+4}{2y}\bigg|_{(-2,2)}=-1,
$$

and hence

$$
\boxed{P_1+P_2=(2,6),\qquad 2P_2=(0,0).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [elliptic-curve discriminant](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant) is supported at $2$ and $3$, so $5$ and $7$ are primes of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve). Direct point counts give

$$
\#\widetilde E(\mathbb F_5)=8,
\qquad
\#\widetilde E(\mathbb F_7)=8.
$$

For example, summing $1+\chi_p(x(x+1)(x+4))$ over $x\in\mathbb F_p$ and adding the point at infinity gives these values.

The [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) at the two primes shows that $|E(\mathbb Q)_{\mathrm{tors}}|$ divides eight. Part (a) shows that $P_2$ has order four, and $P_1$ is an independent point of order two because it does not lie in $\langle P_2\rangle$. They already generate eight points, so

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\langle P_2\rangle\oplus\langle P_1\rangle
\cong\mathbb Z/4\mathbb Z\oplus\mathbb Z/2\mathbb Z.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [two-descent on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#two-descent-on-an-elliptic-curve) map associated with the three rational roots $0,-1,-4$,

$$
\delta:E(\mathbb Q)/2E(\mathbb Q)longrightarrow
(\mathbb Q^\times/\mathbb Q^{\times2})^2,
\qquad
(x,y)\longmapsto(x,x+1),
$$

with the standard limiting values at the [2-torsion](../../../normalization-of-an-algebraic-curve.md#2-torsion). Only the square classes of $-1$, $2$ and $3$ can occur, because all other numerator and denominator valuations in the three factors $x,x+1,x+4$ are even. Checking solubility over $\mathbb R$, $\mathbb Q_2$ and $\mathbb Q_3$ leaves exactly

$$
\operatorname{im}\delta
=\{(1,1),(-1,-3),(-2,-1),(2,3)\}.
$$

These four classes are represented respectively by $O$, $P_1$, $P_2$ and $P_1+P_2$. Thus $|E(\mathbb Q)/2E(\mathbb Q)|=4$. Since part (b) gives

$$
E(\mathbb Q)\cong\mathbb Z^r\oplus\mathbb Z/4\mathbb Z\oplus\mathbb Z/2\mathbb Z,
$$

the quotient by doubling has order $2^{r+2}$. Therefore

$$
\boxed{\operatorname{rank}E(\mathbb Q)=0.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let the common difference of $r^2,s^2,1,t^2$ be $d$. Then

$$
r^2=2s^2-1,
\qquad t^2=2-s^2.
$$

For $x=-2s^2$ and $y=2rst$,

$$
x(x+1)(x+4)
=(-2s^2)(-r^2)(2t^2)
=4r^2s^2t^2=y^2,
$$

so $(-2s^2,2rst)\in E(\mathbb Q)$.

Part (c) says every rational point is one of the eight torsion points from part (b). Among their $x$-coordinates, the only negative value of the form $-2s^2$ with $s\ne0$ is $-2$, arising from $P_2$ or $-P_2$. Thus $s^2=1$, and the four-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression) has common difference zero. Consequently

$$
\boxed{\text{there is no nonconstant four-term arithmetic progression of rational squares.}}
$$

Clearing denominators gives Euler's corresponding result for integer squares.

## 4

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

[Kummer theory](../../../galois-theory.md#kummer-theory) begins with the exact sequence

$$
1\longrightarrow\mu_n\longrightarrow\overline K^\times
\xrightarrow{(cdot)^n}\overline K^\times\longrightarrow1.
$$

[Galois cohomology](../../../galois-theory.md#galois-cohomology) and Hilbert theorem 90 identify

$$
H^1(K,\mu_n)\cong K^\times/K^{\times n},
$$

so cyclic extensions of exponent dividing $n$ are described by adjoining $n$th roots when $K$ contains $\mu_n$.

For an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) $E/K$, multiplication by $n$ gives the [Kummer exact sequence of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-exact-sequence-of-an-elliptic-curve)

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0.
$$

Its connecting homomorphism is the injective [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve)

$$
E(K)/nE(K)\hookrightarrow H^1(K,E[n]),
\qquad
P\longmapsto(\sigma\mapsto\sigma Q-Q),
$$

where $nQ=P$. Passing to the finite [division field of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#division-field-of-an-elliptic-curve) $K(E[n])$ makes $E[n]$ constant. Rational functions whose divisors are $n(T)-n(O)$ then express the classes through finitely many elements of $K(E[n])^\times/K(E[n])^{\times n}$.

Let $S$ contain the primes above $n$, the primes of [bad reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#bad-reduction-of-an-elliptic-curve) and the finitely many primes introduced by these functions. The local theory of good reduction shows that every Kummer class coming from $E(K)$ is unramified outside $S$, so it lies in an [S-unramified power class group](../../../normalization-of-an-algebraic-curve.md#s-unramified-power-class-group). Such a group is finite: valuations outside $S$ vanish modulo $n$, the [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) is finite, and the [Dirichlet unit theorem](../../../algebraic-number-theory.md#dirichlet-s-unit-theorem) makes the group of $S$-units modulo $n$th powers finite. The kernel created by passing to $K(E[n])$ is finite by finite-group [Galois cohomology](../../../galois-theory.md#galois-cohomology). Hence

$$
\boxed{E(K)/nE(K)\text{ is finite}.}
$$

This is the [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#kummer-theoretic-proof-of-the-weak-mordell-weil-theorem). Combining it with the [height descent lemma](../../../normalization-of-an-algebraic-curve.md#height-descent-lemma) proves the [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group): $E(K)$ is a finitely generated abelian group.

## 5

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $P=[x_0:\cdots:x_N]\in\mathbb P^N(\mathbb Q)$, choose coprime integer coordinates and define the [projective height](../../../algebraic-number-theory.md#projective-height)

$$
H(P)=\max_i|x_i|.
$$

Write the morphism $F:\mathbb P^1\to\mathbb P^1$ as $F=[F_0:F_1]$, where $F_0,F_1\in\mathbb Z[X,Y]$ are homogeneous of degree $d$ with no common zero. Bounding each polynomial by the sum of the absolute values of its coefficients gives

$$
H(F(P))\leq c_2H(P)^d.
$$

Because $F_0$ and $F_1$ have no common projective zero, the [Projective Nullstellensatz](../../../algebraic-geometry.md#projective-nullstellensatz) gives an integer $m\geq d$ and homogeneous polynomials $A_{ij}$ such that suitable nonzero integer multiples of $X^m$ and $Y^m$ lie in the ideal $(F_0,F_1)$. Evaluating at primitive coordinates and using the same coefficient bound gives

$$
H(P)^m\leq C H(P)^{m-d}H(F(P)),
$$

after absorbing the bounded common divisor of $F_0(x,y)$ and $F_1(x,y)$ into $C$. Therefore

$$
\boxed{c_1H(P)^d\leq H(F(P))\leq c_2H(P)^d.}
$$

This is [height growth under a morphism of the projective line](../../../normalization-of-an-algebraic-curve.md#height-growth-under-a-morphism-of-the-projective-line).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $x:E\to\mathbb P^1$ be the $x$-coordinate map and define the naive logarithmic height by

$$
h(O)=0,
\qquad h(P)=\frac12\log H(x(P)).
$$

The duplication formula induces a degree-four morphism on the $x$-line, so part (a) gives

$$
h(2P)=4h(P)+O(1)
$$

uniformly in $P$. The telescoping sequence $4^{-n}h(2^nP)$ is therefore Cauchy. Define the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) by

$$
\widehat h(P)=\lim_{n\to\infty}4^{-n}h(2^nP).
$$

Summing the geometric error series proves that $|h(P)-\widehat h(P)|$ is bounded. If another function has this bounded-difference property and scales by four under doubling, evaluating the bounded difference at $2^nP$ and dividing by $4^n$ proves uniqueness.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

The addition law and part (a) give the approximate parallelogram identity

$$
h(P+Q)+h(P-Q)=2h(P)+2h(Q)+O(1).
$$

Replace $P,Q$ by $2^nP,2^nQ$, divide by $4^n$, and let $n\to\infty$. The error disappears, leaving the exact [parallelogram law](../../../linear-algebra.md#parallelogram-law)

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Together with $\widehat h(2P)=4\widehat h(P)$, induction on $|m|$ yields

$$
\boxed{\widehat h(mP)=m^2\widehat h(P)}
$$

for every integer $m$.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

Let $T$ have order $m>0$. Property (ii) gives $\widehat h(T)=0$, since

$$
m^2\widehat h(T)=\widehat h(mT)=\widehat h(O)=0.
$$

It also gives

$$
m^2\widehat h(P+T)=\widehat h(mP+mT)=\widehat h(mP)=m^2\widehat h(P).
$$

Therefore

$$
\boxed{\widehat h(P+T)=\widehat h(P)}
$$

for every rational [torsion point of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve). The construction in part (i), quadraticity in part (ii), and this identity establish existence; the bounded-difference and doubling argument in part (i) establishes uniqueness.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Since $\widehat h-h$ is bounded, a bound on $\widehat h(P)$ bounds the [projective height](../../../algebraic-number-theory.md#projective-height) of $x(P)$. The [Northcott theorem](../../../algebraic-number-theory.md#northcott-theorem) gives only finitely many possible rational $x$-coordinates, and each has at most two points above it. Hence

$$
\boxed{N(B)<\infty.}
$$

By the [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group), $E(\mathbb Q)\cong\mathbb Z^r\oplus E(\mathbb Q)_{\mathrm{tors}}$. The canonical height is a positive-definite [quadratic form](../../../linear-algebra.md#quadratic-form) on the lattice $\mathbb Z^r$, so [canonical-height lattice-point growth](../../../normalization-of-an-algebraic-curve.md#canonical-height-lattice-point-growth) gives

$$
N(B)=O(B^{r/2}).
$$

If $r=0$, this count is bounded; if $r=1$, it is $O(\sqrt B)$. Consequently

$$
\boxed{\frac{N(B)}{\sqrt B}\longrightarrow\infty\quad\Longrightarrow\quad\operatorname{rank}E(\mathbb Q)\geq2.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
