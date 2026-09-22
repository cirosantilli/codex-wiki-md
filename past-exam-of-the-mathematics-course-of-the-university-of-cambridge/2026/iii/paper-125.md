# Paper 125

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20125.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20125.pdf)

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
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A one-dimensional commutative [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) over $R$ is a power series $F(X,Y)\in R[[X,Y]]$ satisfying

$$
F(X,0)=X,qquad F(X,Y)=F(Y,X),qquad
F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

A homomorphism $\theta:\mathcal F\to\mathcal G$ is a series $\theta(T)\in TR[[T]]$ such that

$$
\theta(F(X,Y))=G(\theta(X),\theta(Y)).
$$

Write $\theta(T)=uT+O(T^2)$. If $u=\theta'(0)$ is a unit, recursive comparison of coefficients constructs a unique compositional inverse $\psi(T)\in TR[[T]]$ with $\psi(\theta(T))=T=\theta(\psi(T))$. Apply $\psi$ to the homomorphism identity and substitute $X=\psi(U)$, $Y=\psi(V)$ to obtain

$$
F(\psi(U),\psi(V))=\psi(G(U,V)).
$$

**Thus $\psi$ is a homomorphism from $\mathcal G$ to $\mathcal F$, so $\theta$ is an isomorphism.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [Minimal Weierstrass equation](../../../normalization-of-an-algebraic-curve.md#minimal-weierstrass-equation) for $E/\mathbb Q_p$ is a [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) with coefficients in $\mathbb Z_p$ whose discriminant has minimum $p$-adic valuation among all integral equations for $E$ related by admissible changes of variables.

Let $P\in E(\mathbb Q_p)$ and choose projective coordinates $[X:Y:Z]$ with $X,Y,Z\in\mathbb Z_p$ and at least one coordinate a unit. Reducing the coordinates modulo $p$ gives

$$
\operatorname{red}(P)=[\bar X:\bar Y:\bar Z]\in\bar E(\mathbb F_p).
$$

Multiplying the primitive coordinates by a unit does not alter this point, so this defines the [reduction map](../../../normalization-of-an-algebraic-curve.md#reduction-of-an-elliptic-curve) $E(\mathbb Q_p)\to\bar E(\mathbb F_p)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For the [filtration of elliptic-curve points over a local field](../../../normalization-of-an-algebraic-curve.md#filtration-of-elliptic-curve-points-over-a-local-field), define

$$
E_0(\mathbb Q_p)=\{P:\operatorname{red}(P)\in\bar E_{\mathrm{ns}}(\mathbb F_p)\},
$$

and

$$
E_1(\mathbb Q_p)=\ker\left(E_0(\mathbb Q_p)\to\bar E_{\mathrm{ns}}(\mathbb F_p)\right).
$$

For $r\geq1$, use the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve) with parameter $z=-x/y$ and put

$$
E_r(\mathbb Q_p)=\{P\in E_1(\mathbb Q_p):v_p(z(P))\geq r\}.
$$

Reduction induces

$$
E_0(\mathbb Q_p)/E_1(\mathbb Q_p)
\cong\bar E_{\mathrm{ns}}(\mathbb F_p),
$$

while the coefficient of $p^r$ in the formal parameter gives

$$
\boxed{E_r(\mathbb Q_p)/E_{r+1}(\mathbb Q_p)
\cong(\mathbb F_p,+)qquad(r\geq1).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a locally compact group $G$ on which multiplication by $n$ has finite kernel and cokernel, compare a [Haar measure](../../../measure-theory.md#haar-measure) with its pushforward under $[n]$. On the one-dimensional $p$-adic Lie group $E(\mathbb Q_p)$, the derivative of $[n]$ at the identity is $n$, hence

$$
\frac{\#E(\mathbb Q_p)/nE(\mathbb Q_p)}{\#E(\mathbb Q_p)[n]}
=|n|_p^{-1}=p^{v_p(n)}.
$$

This can also be read directly from the successive quotients in the [filtration of elliptic-curve points over a local field](../../../normalization-of-an-algebraic-curve.md#filtration-of-elliptic-curve-points-over-a-local-field); factors prime to $p$ act invertibly on a sufficiently small formal-group neighbourhood.

The real Lie group $E(\mathbb R)$ has one or two circle components. On its identity component, $[n]$ has degree $n$; the component-group kernel and cokernel have the same order. Therefore

$$
\frac{\#E(\mathbb R)/nE(\mathbb R)}{\#E(\mathbb R)[n]}=\frac1n.
$$

Only primes dividing $n$ contribute to the finite-place product, and unique factorization gives

$$
\boxed{\frac1n\prod_p p^{v_p(n)}=1.}
$$

## 2

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an endomorphism $\phi$ of an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), define its [trace of an elliptic-curve endomorphism](../../../normalization-of-an-algebraic-curve.md#trace-of-an-elliptic-curve-endomorphism) by

$$
\operatorname{tr}(\phi)=1+\deg\phi-\deg(1-\phi).
$$

Polarizing the quadratic form $\deg$ shows that this is the integer for which

$$
\phi+\widehat\phi=[\operatorname{tr}(\phi)],
\qquad
\widehat\phi\phi=[\deg\phi],
$$

where $\widehat\phi$ is the [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny). Consequently

$$
\phi^2-[\operatorname{tr}(\phi)]\phi+[\deg\phi]
=\phi^2-(\phi+\widehat\phi)\phi+\widehat\phi\phi=0.
$$

Also

$$
\phi^2+\widehat\phi^{,2}
=(\phi+\widehat\phi)^2-2\phi\widehat\phi
=[\operatorname{tr}(\phi)^2-2\deg\phi].
$$

The left side is $[\operatorname{tr}(\phi^2)]$, so

$$
\boxed{\operatorname{tr}(\phi^2)=\operatorname{tr}(\phi)^2-2\deg\phi.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) and put

$$
a=p+1-\#E(\mathbb F_p).
$$

Part (a) gives

$$
\pi^2-[a]\pi+[p]=0.
$$

Let $\alpha,\beta$ be the two roots of $T^2-aT+p$. The points over $\mathbb F_{p^r}$ are exactly $\ker(1-\pi^r)$. Since the differential of $1-\pi^r$ is the identity, this isogeny is separable, and therefore

$$
\#E(\mathbb F_{p^r})=\deg(1-\pi^r).
$$

Using $\deg\psi=(1-\psi)(1-\widehat\psi)$ in the endomorphism algebra gives the [elliptic-curve point count over a finite field](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-point-count-over-a-finite-field)

$$
\#E(\mathbb F_{p^r})
=p^r+1-\alpha^r-\beta^r.
$$

Equivalently, if $a_r=\alpha^r+\beta^r$, then

$$
a_0=2,qquad a_1=a,qquad a_r=aa_{r-1}-pa_{r-2},
$$

and $\#E(\mathbb F_{p^r})=p^r+1-a_r$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Suppose that $uP+v\alpha(P)=O$ with $u,v\in\mathbb F_\ell$. If $v=0$, then $u=0$ because $P$ has order $\ell$. If $v\ne0$, then

$$
\alpha(P)=\lambda P,qquad \lambda=-u/v\in\mathbb F_\ell.
$$

Applying $\alpha$ again and using $\alpha^2=[-1]$ yields $\lambda^2=-1$ in $\mathbb F_\ell$. This is impossible when $\ell\equiv3\pmod4$, because $-1$ is then not a quadratic residue. Hence $P$ and $\alpha(P)$ are linearly independent in the two-dimensional vector space $E[\ell]$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

For $E:y^2=x^3-x$ over $\mathbb F_3$, each of $x=0,1,2$ gives the single affine point with $y=0$. Including $O$ gives $\#E(\mathbb F_3)=4$, so the Frobenius trace is $a=3+1-4=0$. Therefore the [Frobenius isogeny of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) $\pi$ satisfies

$$
\pi^2+[3]=0.
$$

On the [$11$-torsion](../../../normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve), this reads $\pi^2=[-3]=[8]$. The element $8\in\mathbb F_{11}^{\times}$ has order ten and $8^5=-1$. Hence

$$
\pi^{10}=-1,qquad \pi^{20}=1,
$$

and no smaller positive power of $\pi$ is the identity on $E[11]$. A [division field of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#division-field-of-an-elliptic-curve) over a finite field has degree equal to the order of Frobenius on the torsion module, so

$$
\boxed{[\mathbb F_3(E[11]):\mathbb F_3]=20.}
$$

## 3

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $P=[x:y]\in\mathbb P^1(\mathbb Q)$ represented by coprime integers, its [naive height on the projective line](../../../normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line) is

$$
H(P)=\max\{|x|,|y|\}.
$$

Write the degree-$d$ morphism as $\Phi=[F:G]$, where $F,G\in\mathbb Z[X,Y]$ are homogeneous of degree $d$ with no common projective zero. Bounding their coefficients gives

$$
H(\Phi(P))\leq c_2H(P)^d.
$$

For the reverse inequality, the nonvanishing of the [resultant](../../../polynomial.md#resultant) of $F$ and $G$ gives homogeneous Bézout identities expressing fixed nonzero integer multiples of powers of $X$ and $Y$ as polynomial combinations of $F$ and $G$. Evaluating at $(x,y)$, removing the common divisor of $F(x,y)$ and $G(x,y)$, and taking the larger of $|x|,|y|$ gives

$$
H(P)^d\leq C H(\Phi(P)).
$$

**Thus $c_1H(P)^d\leq H(\Phi(P))\leq c_2H(P)^d$ for constants depending only on $\Phi$.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $h=\log H$ and set $h_x(P)=h(x(P))$ for $P\ne O$, with $h_x(O)=0$. The given degree-four morphism and part (a) imply that a constant $C$ exists with

$$
|h_x(2P)-4h_x(P)|\leq C
$$

for every $P\in E(\mathbb Q)$. Define

$$
\widehat h(P)=\frac12\lim_{r\to\infty}4^{-r}h_x(2^rP).
$$

To check the limit, put $a_r=4^{-r}h_x(2^rP)$. Then

$$
|a_{r+1}-a_r|\leq C4^{-r-1}.
$$

The geometric series converges, so $(a_r)$ is Cauchy and the limit exists. This is the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve); shifting the sequence by one index immediately gives $\widehat h(2P)=4\widehat h(P)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Because the [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) is a quadratic form, polarization makes

$$
B(P,Q)=\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)
$$

a symmetric bilinear form on the free part of the [Mordell-Weil group](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group). If $P'_i=\sum_jU_{ij}P_j$ is another integral basis, then $U\in\operatorname{GL}_r(\mathbb Z)$ and the Gram matrices satisfy

$$
M'=UMU^T.
$$

Since $\det U=\pm1$, their determinants agree. Thus the [regulator of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#regulator-of-an-elliptic-curve) is independent of the chosen basis.

Now let $Q_1,\ldots,Q_r$ be a basis for the free part of $E'(\mathbb Q)$. The images $\phi(P_i)$ span a finite-index sublattice, so modulo torsion

$$
\phi(P_i)=\sum_jA_{ij}Q_j
$$

for an integral matrix $A$ with nonzero determinant. The height identity gives

$$
B'(\phi P_i,\phi P_j)=\deg(\phi)B(P_i,P_j).
$$

Taking determinants in the two descriptions of this Gram matrix yields

$$
(\det A)^2\operatorname{Reg}(E'/\mathbb Q)
=\deg(\phi)^r\operatorname{Reg}(E/\mathbb Q).
$$

**Therefore the required formula holds with $d=(\det A)^{-1}\in\mathbb Q^\times$.**

## 4

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve) gives an injection

$$
\delta:E(K)/nE(K)\hookrightarrow H^1(K,E[n]).
$$

Because $E[n]\subseteq E(K)$, the Galois action on $E[n]$ is trivial, so a cocycle in the image is a continuous homomorphism $G_K\to E[n]$. For $P\in E(K)$ and $Q$ with $nQ=P$, its kernel fixes the Kummer extension $K(Q)/K$, which is Galois of degree at most $n^2$ and exponent dividing $n$.

The local theory of [reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-an-elliptic-curve) shows that these extensions are unramified outside the finite set consisting of primes dividing $n$, primes of bad reduction, and archimedean places. Local fields have only finitely many extensions of any bounded degree. Together with the Hermite-Minkowski finiteness theorem, this implies that only finitely many global extensions of degree at most $n^2$ with these ramification restrictions occur. Each has only finitely many homomorphisms to the finite group $E[n]$. Hence the image of $\delta$, and therefore $E(K)/nE(K)$, is finite.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For

$$
E:y^2=x^3+x^2+7x,
$$

use [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent) through

$$
E':y^2=x^3-2x^2-27x.
$$

The square-class maps send a nonexceptional point to the class of its $x$-coordinate. On $E$, possible classes are $\pm1,\pm7$; the defining quartics and positivity exclude the negative classes, while $(1,3)$ and $(7,21)$ realize $1$ and $7$. Thus the image has order two. On $E'$, the possible classes are $\pm1,\pm3$; the classes $1$ and $-3$ occur, while the quartics for $-1$ and $3$ have no primitive solution modulo $16$. Hence this image also has order two. The two-isogeny descent formula

$$
2^{r+2}=|\operatorname{im}\alpha|\,|\operatorname{im}\alpha'|
$$

therefore gives $r=0$.

The displayed curve has good reduction at $5$ and $11$, where direct counting gives

$$
\#E(\mathbb F_5)=6,
\qquad
\#E(\mathbb F_{11})=18.
$$

Reduction injects rational torsion of order prime to these characteristics, so its order divides $\gcd(6,18)=6$. We already have the six distinct points

$$
O,quad(0,0),quad(1,\pm3),quad(7,\pm21).
$$

Since the rank is zero, these are all the rational points and $E(\mathbb Q)\cong\mathbb Z/6\mathbb Z$.

## 5

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

In characteristic zero, the [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) $\phi:E\to E'$ is finite and separable, so

$$
[K(E):K(E')]=\deg\phi=\#E[\phi].
$$

For every $T\in E[\phi]$, translation $\tau_T(P)=P+T$ satisfies $\phi\tau_T=\phi$. It therefore induces a $K(E')$-automorphism of $K(E)$. These translations are distinct, giving $\#E[\phi]$ automorphisms of an extension of the same degree. The extension is consequently Galois, and

$$
E[\phi]\longrightarrow\operatorname{Gal}(K(E)/K(E')),
\qquad T\longmapsto\tau_T^*,
$$

is an isomorphism.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $Q\in E'[\widehat\phi]$. The compatibility of divisor classes with pullback identifies the class of

$$
\phi^*((Q)-(O))
$$

with $\widehat\phi(Q)=O$, so choose $g_Q\in K(E)^\times$ with

$$
\operatorname{div}(g_Q)=\phi^*((Q)-(O)).
$$

Since $[n]Q=\phi\widehat\phi(Q)=O$, choose $f_Q\in K(E')^\times$ with

$$
\operatorname{div}(f_Q)=n((Q)-(O)).
$$

The functions $f_Q\circ\phi$ and $g_Q^n$ have the same divisor. Their quotient is constant, and because $K$ is algebraically closed we may rescale $g_Q$ so that

$$
f_Q\circ\phi=g_Q^n.
$$

Thus define

$$
E'[\widehat\phi]\longrightarrow
\frac{K(E')^\times\cap K(E)^{\times n}}{K(E')^{\times n}},
\qquad Q\longmapsto[f_Q].
$$

Changing either function changes $f_Q$ only by an $n$th power of a constant. The divisor relation for $Q+R$ differs from the sum of those for $Q$ and $R$ by $n$ times a principal divisor, so the map is a homomorphism. If $[f_Q]$ is trivial, then $f_Q=h^n$ for $h\in K(E')^\times$, whence $\operatorname{div}(h)=(Q)-(O)$; the divisor-class isomorphism forces $Q=O$. The map is therefore well-defined and injective.

For $P\in E[\phi]$, translation by $P$ fixes $g_Q^n=f_Q\circ\phi$. Hence

$$
e_\phi(P,Q)=\frac{g_Q(X+P)}{g_Q(X)}\in\mu_n
$$

is independent of the auxiliary point $X$. This is the [Weil pairing](../../../normalization-of-an-algebraic-curve.md#weil-pairing) associated with $\phi$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $D_Q=(Q)-(O)$ on $E'$. Compatibility of the divisor-class maps with pullback gives a function $h\in K(E)^\times$ such that

$$
D_{\widehat\phi(Q)}=\phi^*D_Q+\operatorname{div}(h).
$$

If $f_Q$ has divisor $mD_Q$, then

$$
\operatorname{div}((f_Q\circ\phi)h^m)=mD_{\widehat\phi(Q)}.
$$

Use these functions in the divisor-evaluation formula for the [Weil pairing](../../../normalization-of-an-algebraic-curve.md#weil-pairing). Pullback and pushforward satisfy

$$
(f_Q\circ\phi)(D_P)=f_Q(\phi_*D_P),
$$

while the factor $h^m$ contributes an $m$th power and cancels from the pairing. The two evaluations are therefore identical, giving

$$
e_m(P,\widehat\phi(Q))=e_m(\phi(P),Q)
$$

for every $P\in E[m]$ and $Q\in E'[m]$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
