# Paper 125

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_125.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_125.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For points $P,Q$ on a smooth plane cubic, draw the line through them, using the tangent at $P$ when $P=Q$, and let its third intersection with the cubic be $R$. The [chord-and-tangent group law](../../../normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law) defines $P+Q$ as the reflection of $R$ in the $x$-axis; the point at infinity $O$ is the identity and $-(x,y)=(x,-y)$.

If $P,Q\in E(\mathbb Q)$, their chord or tangent has rational coefficients. Substitution into the cubic gives a polynomial with rational coefficients for which two intersection roots are rational, so the third is rational as well. The identity and inverse of every rational point are rational, and closure under addition follows. Assuming the elliptic-curve law is a group law, $E(\mathbb Q)$ is therefore a subgroup of $E(\overline{\mathbb Q})$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $E:y^2=x^3-9x+9$, the addition formulas use

$$
m=\frac{y_2-y_1}{x_2-x_1},
\qquad
x(P_1+P_2)=m^2-x_1-x_2,
\qquad
y(P_1+P_2)=m(x_1-x(P_1+P_2))-y_1,
$$

with $m=(3x_1^2-9)/(2y_1)$ for doubling. They give

$$
2P=\left(\frac94,\frac38\right),
\qquad
2Q=(3,-3)=-Q,
$$

and

$$
P+Q=(-3,-3),
\qquad
P-Q=(1,-1).
$$

Let $(x,y)\ne O$ be rational. If the [3-adic valuation](../../../number-theory.md#p-adic-valuation) satisfies $v_3(y)\geq2$, first $v_3(x)$ cannot be negative: otherwise $x^3$ is the unique term of least valuation in $x^3-9x+9$, giving $2v_3(y)=3v_3(x)<0$. If $v_3(x)=0$, the right side has valuation zero. If $v_3(x)\geq1$, its three terms have valuations at least $3$, at least $3$, and exactly $2$, so $2v_3(y)=2$. In every case $v_3(y)\leq1$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Lutz–Nagell theorem](../../../normalization-of-an-algebraic-curve.md#nagell-lutz-theorem) says that if

$$
E:y^2=x^3+ax+b,
\qquad a,b\in\mathbb Z,
$$

has nonzero discriminant and $P=(x,y)\in E(\mathbb Q)$ is a torsion point, then $x,y\in\mathbb Z$ and either $y=0$ or

$$
y^2\mid4a^3+27b^2.
$$

For integrality, fix a prime $p$. If a rational point has nonintegral coordinates, its primitive projective coordinates reduce to $O$, so it belongs to the kernel of reduction. The parameter $t=-x/y$ identifies this kernel with the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve) over $p\mathbb Z_p$. The formal logarithm, with the standard separate first-step argument at $p=2$, shows that this group has no nonzero rational torsion. A rational torsion point therefore has nonnegative $p$-adic valuations in both coordinates for every prime $p$, hence integral coordinates.

Suppose now that $y\ne0$. The point $2P$ is again a nonzero torsion point and hence integral. Its $x$-coordinate is $m^2-2x$, where

$$
m=\frac{3x^2+a}{2y}.
$$

Thus $m^2$ is an integer. A rational number whose square is integral is integral, so $2y\mid3x^2+a$ and in particular $y^2\mid(3x^2+a)^2$. The curve equation and the identity

$$
(3x^2+4a)(3x^2+a)^2-27(x^3+ax-b)(x^3+ax+b)=4a^3+27b^2
$$

then prove $y^2\mid4a^3+27b^2$. This is the [divisibility proof in the Nagell–Lutz theorem](../../../normalization-of-an-algebraic-curve.md#divisibility-proof-in-the-nagell-lutz-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Here

$$
4a^3+27b^2=4(-9)^3+27(9)^2=-729=-3^6.
$$

By the [Lutz–Nagell theorem](../../../normalization-of-an-algebraic-curve.md#nagell-lutz-theorem), a nonzero rational torsion point has integral coordinates and either $y=0$ or $y^2\mid3^6$. Part b gives $v_3(y)\leq1$, so $y\in\{0,\pm1,\pm3\}$. The cubic $x^3-9x+9$ has no integral zero. Substitution of $y=\pm1,\pm3$ gives exactly

$$
\pm P,\quad \pm Q,\quad \pm(P+Q),\quad \pm(P-Q).
$$

This proves the required inclusion.

Since $2Q=-Q$, the point $Q$ has order three. The point $P$ is not torsion because $2P=(9/4,3/8)$ is nonintegral, contradicting Nagell–Lutz. If $P+Q$ or $P-Q$ were torsion, adding the torsion point $\mp Q$ would make $P$ torsion; their negatives are excluded in the same way. Hence

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{O,Q,-Q\}\cong\mathbb Z/3\mathbb Z.}
$$

## 2

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny) $\phi:E\to E'$ is the degree of the induced finite extension of function fields. Saying that degree is a quadratic form on $\operatorname{End}(E)$ means

$$
\deg(n\phi)=n^2\deg\phi
$$

and that

$$
\langle\phi,\psi\rangle=\frac12\bigl(\deg(\phi+\psi)-\deg\phi-\deg\psi\bigr)
$$

is bilinear, equivalently

$$
\deg(\phi+\psi)+\deg(\phi-\psi)=2\deg\phi+2\deg\psi.
$$

The [trace of an elliptic-curve endomorphism](../../../normalization-of-an-algebraic-curve.md#trace-of-an-elliptic-curve-endomorphism) is

$$
\operatorname{tr}(\phi)=1+\deg\phi-\deg(1-\phi).
$$

The relation $\phi^2-[\operatorname{tr}\phi]\phi+[\deg\phi]=0$ implies

$$
\operatorname{tr}(\phi^2)=\operatorname{tr}(\phi)^2-2\deg\phi,
$$

the [trace of the square of an elliptic-curve endomorphism](../../../normalization-of-an-algebraic-curve.md#trace-of-the-square-of-an-elliptic-curve-endomorphism).

The [Hasse theorem for elliptic curves](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves) states that for $E/\mathbb F_q$,

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve), put $a=\operatorname{tr}(\pi)$, and note that $\deg\pi=q$ and

$$
\#E(\mathbb F_q)=\deg(1-\pi)=q+1-a.
$$

For integers $m,n$, quadraticity gives

$$
0\leq\deg(m+n\pi)=m^2+amn+qn^2.
$$

This binary quadratic form cannot have positive discriminant, since rational numbers $m/n$ are dense, so $a^2-4q\leq0$. Substitution proves the bound. This is the [degree-form proof of the Hasse bound](../../../normalization-of-an-algebraic-curve.md#degree-form-proof-of-the-hasse-bound).

Both endpoints occur. The curve $E:y^2=x^3-x$ over $\mathbb F_3$ is supersingular with trace zero. Over $\mathbb F_9$, its Frobenius is $[-3]$, so

$$
\#E(\mathbb F_9)=9+1-(-6)=16=9+1+2\sqrt9.
$$

Its nontrivial [quadratic twist](../../../normalization-of-an-algebraic-curve.md#quadratic-twist-of-an-elliptic-curve) over $\mathbb F_9$ has the opposite trace and therefore has

$$
9+1-6=4=9+1-2\sqrt9
$$

points.

## 3

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a short Weierstrass equation $E:y^2=x^3+ax+b$ in characteristic different from two, the [invariant differential on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#invariant-differential-on-an-elliptic-curve)

$$
\omega=\frac{dx}{2y}
$$

is nonzero and regular, including at $O$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $X=x\circ\phi$. Since $X(-P)=X(P)$, it is an even rational function and therefore belongs to $k(x)$; write $X=p(x)/q(x)$ with coprime polynomials $p,q$. The pullback of a nonzero invariant differential is invariant, so for some $c\in k^\times$,

$$
\phi^*\left(\frac{dX}{2Y}\right)=c\frac{dx}{2y}.
$$

Since

$$
dX=\frac{p'q-pq'}{q^2},dx,
$$

we obtain

$$
Y=\frac{p'q-pq'}{cq^2},y.
$$

Thus

$$
\boxed{\phi(x,y)=\left(\frac{p(x)}{q(x)},\frac{p'(x)q(x)-p(x)q'(x)}{c q(x)^2}y\right).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Take $(x,y)\in E_r(K)\setminus\{O\}$. Because $v(x)<0$ and $p,q$ have degrees $d,d-1$, their leading terms dominate, giving

$$
v\left(\frac{p(x)}{q(x)}\right)=v(x)\leq-2r.
$$

The polynomial $p'q-pq'$ has degree $2d-2$ with nonzero leading coefficient, the same degree as $q^2$. Their quotient consequently has valuation zero at $x$, so

$$
v\left(\frac{p'q-pq'}{cq^2}y\right)=v(y)\leq-3r.
$$

The isogeny sends $O$ to $O$, hence $\phi(E_r(K))\subseteq E'_r(K)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the alternative affine coordinates

$$
t=-\frac{x}{y},\qquad w=-\frac1y,
$$

so that $x=t/w$ and $y=-1/w$. The equation becomes

$$
w=t^3+atw^2+bw^3.
$$

Recursive coefficient comparison gives a unique series $w(t)\in t^3k[[t]]$. Since $v(w(t))=3v(t)$ and hence $v(x)=-2v(t)$, $v(y)=-3v(t)$, this gives the [formal coordinates on a short Weierstrass curve](../../../normalization-of-an-algebraic-curve.md#formal-coordinates-on-a-short-weierstrass-curve) identification

$$
\boxed{E_1(K)=\{(t,w(t)):v(t)\geq1\}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

A one-dimensional commutative [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) over a ring $R$ is a power series $F(X,Y)\in R[[X,Y]]$ satisfying $F(X,0)=X$, commutativity, and associativity. A morphism $f:F\to G$ is a series $f(T)\in TR[[T]]$ satisfying

$$
f(F(X,Y))=G(f(X),f(Y)).
$$

Express the isogeny of part b in the formal coordinates of part d and set

$$
f(t)=-\frac{X(t,w(t))}{Y(t,w(t))}.
$$

Part c shows that points approaching $O$ map to points approaching $O'$, so $f(t)\in tk[[t]]$. Since $\phi$ is a group homomorphism, applying the parameter $t'$ to $\phi(P+Q)=\phi(P)+\phi(Q)$ gives

$$
f(F_E(t_1,t_2))=F_{E'}(f(t_1),f(t_2)).
$$

**Thus $f$ is the [formal-group morphism induced by an isogeny](../../../normalization-of-an-algebraic-curve.md#formal-group-morphism-induced-by-an-isogeny) $\widehat E\to\widehat{E'}$.**

## 4

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $G=\operatorname{Gal}(L/K)$. If $a\in K^\times$ becomes an $n$th power in $L$, choose $\alpha\in L$ with $\alpha^n=a$. Then

$$
\sigma\longmapsto\frac{\sigma(\alpha)}{\alpha}
$$

is a cocycle with values in the finite group $\mu_n(L)$. Changing $\alpha$ changes it by a coboundary, and its class is trivial exactly when $a$ was already an $n$th power in $K$. Thus the kernel injects into the finite group $H^1(G,\mu_n(L))$ and is finite. This is the multiplicative case of the [finite-extension kernel of a Kummer map](../../../normalization-of-an-algebraic-curve.md#finite-extension-kernel-of-a-kummer-map).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Assume $\mu_n\subset K$ and put $\alpha=\sqrt[n]{a}$. All roots of $X^n-a$ are $\zeta\alpha$ with $\zeta\in\mu_n\subset K$, so $K(\alpha)$ is its splitting field and is a [Finite Galois extension](../../../galois-theory.md#finite-galois-extension). The map

$$
\operatorname{Gal}(K(\alpha)/K)\longrightarrow\mu_n,
\qquad
\sigma\longmapsto\frac{\sigma(\alpha)}{\alpha}
$$

is an injective group homomorphism.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For a finite Galois extension $L/K$, the kernel of

$$
E(K)/nE(K)\longrightarrow E(L)/nE(L)
$$

is finite. Indeed, if $P=nQ$ for $Q\in E(L)$, then $\sigma\mapsto\sigma Q-Q$ is a cocycle in the finite $G$-module $E[n](L)$, and the resulting map from the kernel to $H^1(G,E[n](L))$ is injective.

The analogue of part b assumes $E[n]\subset E(K)$. Given $P\in E(K)$ and $Q\in E(\overline K)$ with $nQ=P$, every conjugate of $Q$ is $Q+T$ for some $T\in E[n]$. Hence $K(Q)/K$ is Galois and

$$
\operatorname{Gal}(K(Q)/K)\longrightarrow E[n],
\qquad
\sigma\longmapsto\sigma Q-Q
$$

is an injective homomorphism. These are the two elliptic forms of the [Kummer pairing](../../../normalization-of-an-algebraic-curve.md#kummer-pairing).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Pass to the finite extension $L=K(E[n])$. Part c shows that the kernel of $E(K)/nE(K)\to E(L)/nE(L)$ is finite, so it is enough to control the image after $n$-torsion becomes rational. The [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve)

$$
E(L)/nE(L)\hookrightarrow H^1(L,E[n])
$$

associates to $P$ the finite extension generated by one $n$-division point of $P$.

Let $S$ contain the places over $n$, all archimedean places, and all places of bad reduction. The local theory of elliptic curves shows that these Kummer classes are unramified outside $S$. Because $E[n]$ is finite and constant over $L$, such classes are controlled by finitely many $S$-unramified power classes. Finiteness of the class group and finite generation of the unit group make that power-class group finite. The Kummer image is therefore finite, proving the [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem) that $E(K)/nE(K)$ is finite; this is the [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#kummer-theoretic-proof-of-the-weak-mordell-weil-theorem).

## 5

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let a rational right triangle have legs $A,B$, hypotenuse $C$, and area $AB/2=D$. After interchanging the legs if necessary, set

$$
x=\frac{A+C}{B},
\qquad
y=\frac{2x}{B}.
$$

Using $C^2=A^2+B^2$ and $AB=2D$ gives

$$
x^2-1=\frac{2A(A+C)}{B^2}=\frac{4Dx}{B^2}=\frac{Dy^2}{x},
$$

so $P=(x,y)$ lies on the [congruent number elliptic curve](../../../normalization-of-an-algebraic-curve.md#congruent-number-elliptic-curve) $E_D:Dy^2=x^3-x$. The triangle is nondegenerate, so $y\ne0$ and $2P\ne O$.

Conversely the three displayed lengths in the question satisfy

$$
\left(\frac{x^2-1}{y}\right)^2+\left(\frac{2x}{y}\right)^2
=\left(\frac{x^2+1}{y}\right)^2,
$$

and their area is

$$
\left|\frac{x(x^2-1)}{y^2}\right|=D.
$$

**Thus every such triangle is $\Delta_P$.**

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The change of variables $X=5x$, $Y=25y$ identifies $E_5$ with

$$
Y^2=X^3-25X=X(X-5)(X+5).
$$

A full [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent), equivalently the standard full 2-descent for a cubic with three rational roots, gives

$$
E_5(\mathbb Q)/2E_5(\mathbb Q)
=\langle(0,0),(1,0),(-4/5,6/25)\rangle_{\mathbb F_2}.
$$

The local conditions at $2$, $5$, and infinity leave exactly these eight square-class combinations; primes outside $\{2,5\}$ have even valuations and contribute none. Hence the quotient has dimension three. Since the rational 2-torsion has dimension two, the rank is one.

The [Lutz–Nagell theorem](../../../normalization-of-an-algebraic-curve.md#nagell-lutz-theorem) on the integral model, or reduction at two good primes, excludes odd torsion and torsion of order greater than two. Therefore

$$
E_5(\mathbb Q)_{\mathrm{tors}}=\{O,(0,0),(1,0),(-1,0)\}\cong(\mathbb Z/2\mathbb Z)^2,
$$

and $(-4/5,6/25)$ generates the free part. This is the [Mordell-Weil group of the congruent number curve for five](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group-of-the-congruent-number-curve-for-five).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For $x(P)=A/B^2$ in lowest terms, take the logarithmic naive height $h(P)=\log\max\{|A|,B^2\}$. Its required properties are

$$
h(2P)=4h(P)+O(1)
$$

and

$$
h(P+Q)+h(P-Q)=2h(P)+2h(Q)+O(1),
$$

with constants depending only on the curve. Define the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) by

$$
\widehat h(P)=\lim_{r\to\infty}4^{-r}h(2^rP).
$$

The first bounded-error relation makes this a convergent telescoping correction to $h(P)$. Apply the second relation to $2^rP,2^rQ$, divide by $4^r$, and let $r\to\infty$ to obtain

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Also $\widehat h(2P)=4\widehat h(P)$, and the parallelogram identity then gives $\widehat h(nP)=n^2\widehat h(P)$ for every integer $n$. Thus $\widehat h$ is a quadratic form.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

By part b, write

$$
E_5(\mathbb Q)=\mathbb ZG\oplus E_5[2].
$$

The [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) vanishes on torsion and satisfies $\widehat h(mG+T)=m^2\widehat h(G)$. If $\widehat h(P)=\widehat h(Q)\ne0$, their nonzero integer coefficients therefore have equal squares, so

$$
Q=\pm P+T
$$

for some $T\in E_5[2]$.

Negation leaves the $x$-coordinate unchanged. Addition by the four 2-torsion points changes $x$ among

$$
x,qquad-\frac1x,qquad\frac{x+1}{x-1},
\qquad-\frac{x-1}{x+1}.
$$

Substitution in the three side formulas for $\Delta_P$, using $5y^2=x^3-x$, only changes signs and permutes the three values. Hence $\Delta_Q$ and $\Delta_P$ are the same right triangle up to reordering their sides.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
