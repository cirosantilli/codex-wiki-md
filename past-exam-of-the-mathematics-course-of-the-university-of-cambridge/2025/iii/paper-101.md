# Paper 101

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20101.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20101.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [a](#1/iv/a)
      - [Solution](#1/iv/a/solution)
    - [b](#1/iv/b)
      - [Solution](#1/iv/b/solution)
  - [v](#1/v)
    - [a](#1/v/a)
      - [Solution](#1/v/a/solution)
    - [b](#1/v/b)
      - [Solution](#1/v/b/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [a](#2/iii/a)
      - [Solution](#2/iii/a/solution)
    - [b](#2/iii/b)
      - [Solution](#2/iii/b/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [a](#4/ii/a)
      - [Solution](#4/ii/a/solution)
    - [b](#4/ii/b)
      - [Solution](#4/ii/b/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [a](#5/iii/a)
      - [Solution](#5/iii/a/solution)
    - [b](#5/iii/b)
      - [Solution](#5/iii/b/solution)

## 1

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $R$-modules $M,N$, the [tensor product of modules](../../../module-theory.md#tensor-product-of-modules) is an $R$-module $M\otimes_RN$ together with the balanced map

$$
\tau:M\times N\longrightarrow M\otimes_RN,
\qquad
(m,n)\longmapsto m\otimes n,
$$

such that every [balanced map](../../../module-theory.md#balanced-map) $b:M\times N\to P$ factors through one unique $R$-linear map $\widetilde b$:

$$
b=\widetilde b\circ\tau.
$$

Equivalently,

$$
\operatorname{Hom}_R(M\otimes_RN,P)
\cong\{\text{balanced maps }M\times N\to P\}
$$

naturally in $P$. This is the [universal property of the tensor product of modules](../../../module-theory.md#universal-property-of-the-tensor-product-of-modules).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

**Yes.** The integers form a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), and over a principal ideal domain a module is flat exactly when it is torsion-free. Thus the [torsion-free modules](../../../module-theory.md#torsion-free-module) $A$ and $B$ are [flat modules](../../../module-theory.md#flat-module). The functor

$$
(A\otimes_{\mathbb Z}B)\otimes_{\mathbb Z}-
\cong A\otimes_{\mathbb Z}(B\otimes_{\mathbb Z}-)
$$

is a composite of two exact tensor functors, so $A\otimes_{\mathbb Z}B$ is flat. Applying the converse direction of the same characterization shows that it is torsion-free. This is the [torsion-free module over a principal ideal domain is flat](../../../module-theory.md#torsion-free-module-over-a-principal-ideal-domain-is-flat) criterion.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

**No.** Take $R=\mathbb Z$, $M=\mathbb Q$, and

$$
N_i=\mathbb Z/i\mathbb Z\qquad(i\geq2).
$$

Every $N_i$ is a torsion group, so localization at the nonzero integers gives

$$
\mathbb Q\otimes_{\mathbb Z}N_i=0
$$

and hence $\prod_i(\mathbb Q\otimes_{\mathbb Z}N_i)=0$.

By contrast, the element $x=(1\bmod i)_{i\geq2}$ of $\prod_iN_i$ has infinite order: no positive integer is divisible by every $i$. The canonical description

$$
\mathbb Q\otimes_{\mathbb Z}\prod_iN_i
\cong(\mathbb Z\setminus\{0\})^{-1}\left(\prod_iN_i\right)
$$

shows that $1\otimes x$ is nonzero, because an element dies in this localization only if one nonzero integer annihilates it. Thus the left module is nonzero while the right module is zero, giving the [tensor product and infinite direct product](../../../module-theory.md#tensor-product-and-infinite-direct-product) counterexample.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/a">a</h4>

↑ **Parent:** [Iv](#1/iv)

<h5 id="1/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#1/iv/a)

Assume tensor products of two nonzero modules never vanish. If $\mathfrak m\ne\mathfrak n$ were distinct [maximal ideals](../../../commutative-algebra.md#maximal-ideal), then $\mathfrak m+\mathfrak n=R$ and

$$
(R/\mathfrak m)\otimes_R(R/\mathfrak n)
\cong R/(\mathfrak m+\mathfrak n)=0,
$$

although both residue fields are nonzero. Hence $R$ has one maximal ideal $\mathfrak m$ and is a [local ring](../../../commutative-algebra.md#local-ring).

For every module $M$,

$$
(R/\mathfrak m)\otimes_RM\cong M/\mathfrak mM.
$$

If $\mathfrak mM=M$, this tensor product vanishes. Since $R/\mathfrak m\ne0$, the assumed property forces $M=0$. Thus condition (a) implies condition (b).

<h4 id="1/iv/b">b</h4>

↑ **Parent:** [Iv](#1/iv)

<h5 id="1/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#1/iv/b)

Conversely, assume condition (b), and let $M,N$ be nonzero. The stated property gives

$$
M/\mathfrak mM\ne0,
\qquad
N/\mathfrak mN\ne0.
$$

These are nonzero [vector spaces](../../../vector-space.md) over the [residue field](../../../commutative-algebra.md#residue-field) $k=R/\mathfrak m$, so their tensor product over $k$ is nonzero. Associativity and base change give

$$
\begin{aligned}
(M\otimes_RN)\otimes_Rk
&\cong(M\otimes_Rk)\otimes_k(N\otimes_Rk)\\
&\cong(M/\mathfrak mM)\otimes_k(N/\mathfrak mN)\ne0.
\end{aligned}
$$

**Therefore $M\otimes_RN\ne0$. This proves the reverse implication and the [local tensor nonvanishing criterion](../../../module-theory.md#local-tensor-nonvanishing-criterion).**

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/a">a</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/a/solution">Solution</h5>

↑ **Parent:** [A](#1/v/a)

There is an exact sequence of $R$-modules

$$
0\longrightarrow I\cap J
\xrightarrow{x\mapsto(x,x)}
I\oplus J
\xrightarrow{(x,y)\mapsto x-y}
I+J\longrightarrow0.
$$

If $A$ is a [flat module](../../../module-theory.md#flat-module) over $R$, tensoring this sequence with $A$ preserves its left exactness. The image of each tensor product inside $A$ is the corresponding [extension of an ideal](../../../commutative-algebra.md#extension-of-an-ideal), so

$$
\boxed{I^e\cap J^e=(I\cap J)^e}.
$$

Both displayed inclusions therefore hold. This is the [flat extension preserves finite ideal intersections](../../../module-theory.md#flat-extension-preserves-finite-ideal-intersections) property.

<h4 id="1/v/b">b</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/b/solution">Solution</h5>

↑ **Parent:** [B](#1/v/b)

The inclusion

$$
(I\cap J)^e\subseteq I^e\cap J^e
$$

always holds: each generator coming from $I\cap J$ lies in both extended ideals.

The reverse inclusion can fail. Let

$$
R=k[x,y],\qquad A=R/(x-y),\qquad I=(x),\qquad J=(y)
$$

for a field $k$. Under $A\cong k[x]$,

$$
I^e=J^e=(x),
\qquad
I^e\cap J^e=(x),
$$

whereas $I\cap J=(xy)$ in $R$, so

$$
(I\cap J)^e=(x^2)\subsetneq(x).
$$

**Thus statement (2) is true in general and statement (1) is false in general.**

## 2

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [multiplicative subset](../../../commutative-algebra.md#multiplicatively-closed-set) $S\subseteq R$ contains $1$ and satisfies $s,t\in S\Rightarrow st\in S$. The [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) consists of fractions $r/s$ modulo the relation

$$
\frac r s=\frac{r'}{s'}
\quad\Longleftrightarrow\quad
\text{some }u\in S\text{ satisfies }u(rs'-r's)=0.
$$

Its structure map $\iota:R\to S^{-1}R$ makes every $s\in S$ invertible. The [universal property of localization](../../../commutative-algebra.md#universal-property-of-localization) says that if $f:R\to T$ is any ring homomorphism for which every $f(s)$ is a unit, there is one unique homomorphism $\widetilde f:S^{-1}R\to T$ satisfying $\widetilde f\iota=f$, namely

$$
\boxed{\widetilde f(r/s)=f(r)f(s)^{-1}.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The local criterion states that an $R$-module $M$ is flat if and only if $M_{\mathfrak p}$ is flat over $R_{\mathfrak p}$ for every prime ideal $\mathfrak p$. It is enough equivalently to test maximal ideals.

If $M$ is flat, localization of an exact sequence and the natural isomorphism

$$
(M\otimes_RN)_{\mathfrak p}
\cong M_{\mathfrak p}\otimes_{R_{\mathfrak p}}N_{\mathfrak p}
$$

show immediately that every $M_{\mathfrak p}$ is flat.

Conversely, let $N'\to N$ be injective and let $K$ be the kernel of

$$
M\otimes_RN'\longrightarrow M\otimes_RN.
$$

After localization at any prime $\mathfrak p$, flatness of $M_{\mathfrak p}$ gives $K_{\mathfrak p}=0$. A module whose localization at every maximal ideal is zero must itself be zero: if $0\ne x\in K$, its annihilator is contained in a maximal ideal $\mathfrak m$, and then $x/1\ne0$ in $K_{\mathfrak m}$. Hence $K=0$, tensoring by $M$ preserves every injection, and $M$ is flat. This proves that [flatness is local](../../../module-theory.md#flatness-is-local).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/a">a</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/iii/a)

Put $S=A\setminus\mathfrak p$ and define

$$
B_{\mathfrak p}=S^{-1}B,
$$

where $A$ acts on $B$ through the given inclusion. By the [prime ideal correspondence for localization](../../../commutative-algebra.md#prime-ideal-correspondence-for-localization), primes of $B_{\mathfrak p}$ correspond to primes $\mathfrak q$ of $B$ satisfying $\mathfrak q\cap S=\varnothing$, equivalently $\mathfrak q\cap A\subseteq\mathfrak p$.

The localized extension $A_{\mathfrak p}\subseteq B_{\mathfrak p}$ remains integral. If $\mathfrak q\cap A=\mathfrak p$, then

$$
B_{\mathfrak p}/S^{-1}\mathfrak q
$$

is an integral domain integral over the field $A_{\mathfrak p}/\mathfrak pA_{\mathfrak p}$. An integral domain integral over a field is a field, so $S^{-1}\mathfrak q$ is maximal.

Conversely, if $\mathfrak n$ is maximal in $B_{\mathfrak p}$, the [contraction of a maximal ideal under an integral extension](../../../commutative-algebra.md#contraction-of-a-maximal-ideal-under-an-integral-extension) is maximal in the local ring $A_{\mathfrak p}$, hence equals $\mathfrak pA_{\mathfrak p}$. Contracting once more to $A$ gives $\mathfrak p$. Extension and contraction are inverse under localization, proving the required [fiber primes of an integral extension](../../../commutative-algebra.md#fiber-primes-of-an-integral-extension) bijection.

<h4 id="2/iii/b">b</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/iii/b)

Take

$$
A=\mathbb Z\subseteq B=\mathbb Q,
\qquad
\mathfrak p=(2).
$$

This extension is not integral. Since every nonzero integer is already invertible in $\mathbb Q$,

$$
B_{\mathfrak p}=\mathbb Q
$$

has the maximal ideal $(0)$. On the other hand, the only prime ideal of $B$ is $(0)$, whose contraction to $\mathbb Z$ is $(0)$ rather than $(2)$. The set of primes of $B$ lying over $\mathfrak p$ is therefore empty while $\operatorname{MaxSpec}B_{\mathfrak p}$ is not.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $\mathfrak m$ be maximal in $R/I$ and let $\mathfrak n\subseteq R$ be its contraction. The ideal $\mathfrak n$ is maximal and contains $I$. It is disjoint from $S=1+I$: if $1+i\in\mathfrak n$ with $i\in I\subseteq\mathfrak n$, then $1\in\mathfrak n$. The [prime ideal correspondence for localization](../../../commutative-algebra.md#prime-ideal-correspondence-for-localization) therefore defines the proper ideal $S^{-1}\mathfrak n$, and

$$
S^{-1}R/S^{-1}\mathfrak n\cong R/\mathfrak n
$$

is a field. Thus $f(\mathfrak m)=S^{-1}\mathfrak n$ is maximal.

Conversely, let $\mathfrak q$ be the contraction to $R$ of a maximal ideal of $S^{-1}R$. Then $\mathfrak q$ is maximal among ideals disjoint from $S$. Since $\mathfrak q+I$ is disjoint from $S$—otherwise an equation $q+i=1+j$ would put $1+(j-i)\in\mathfrak q\cap S$—maximality gives $I\subseteq\mathfrak q$. If a proper ideal strictly contained $\mathfrak q$ in a maximal ideal $\mathfrak n$ of $R$, then $\mathfrak n$ would also contain $I$ and hence remain disjoint from $S$, a contradiction. Thus $\mathfrak q$ is maximal and contains $I$.

The two standard extension-contraction bijections, first for $R\to R/I$ and then for $R\to S^{-1}R$, now give inverse maps

$$
\boxed{\operatorname{MaxSpec}(R/I)\cong\operatorname{MaxSpec}(S^{-1}R)}.
$$

## 3

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For an ideal $I\subseteq k[T_1,\ldots,T_n]$, define

$$
V(I)=\{a\in k^n:f(a)=0\text{ for every }f\in I\}.
$$

For $X\subseteq k^n$, define

$$
I(X)=\{f:f(a)=0\text{ for every }a\in X\},
$$

and recall that $\sqrt I=\{f:f^r\in I\text{ for some }r\geq1\}$ is the [radical of an ideal](../../../commutative-algebra.md#radical-of-an-ideal).

For an [algebraically closed field](../../../algebra.md#algebraically-closed-field) $k$, the [Weak Hilbert Nullstellensatz](../../../algebraic-geometry.md#weak-hilbert-nullstellensatz) says that every maximal ideal of $k[T_1,\ldots,T_n]$ is

$$
(T_1-a_1,\ldots,T_n-a_n)
$$

for a unique $a\in k^n$, equivalently every proper ideal has a common zero. The [Strong Hilbert Nullstellensatz](../../../algebraic-geometry.md#strong-hilbert-nullstellensatz) says

$$
\boxed{I(V(I))=\sqrt I}.
$$

To prove the weak form, let $\mathfrak m$ be maximal. The residue field

$$
K=k[T_1,\ldots,T_n]/\mathfrak m
$$

is a field finitely generated as a $k$-algebra. By the [Zariski lemma](../../../algebraic-geometry.md#zariski-s-lemma), $K/k$ is finite algebraic; algebraic closedness gives $K=k$. If $a_i$ is the image of $T_i$, the quotient map is evaluation at $a=(a_1,\ldots,a_n)$ and its kernel is $(T_1-a_1,\ldots,T_n-a_n)$. This proves the assertion.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $\mathfrak m$ be maximal in $\mathbb Q[T_1,\ldots,T_n]$ and put

$$
K=\mathbb Q[T_1,\ldots,T_n]/\mathfrak m.
$$

The [Zariski lemma](../../../algebraic-geometry.md#zariski-s-lemma) makes $K$ a finite extension of $\mathbb Q$. Base change gives

$$
\mathbb C[T_1,\ldots,T_n]/\mathfrak m\mathbb C[T_1,\ldots,T_n]
\cong\mathbb C\otimes_{\mathbb Q}K.
$$

This ring is nonzero because the field extension makes $\mathbb C$ a [faithfully flat module](../../../module-theory.md#faithfully-flat-module) over $\mathbb Q$. Choose a maximal ideal $\mathfrak n$ of the quotient, or equivalently a maximal ideal of $\mathbb C[T_1,\ldots,T_n]$ containing $\mathfrak m\mathbb C[T_1,\ldots,T_n]$. Its contraction to the rational polynomial ring contains $\mathfrak m$ and is proper, so maximality of $\mathfrak m$ forces

$$
\boxed{\mathfrak n\cap\mathbb Q[T_1,\ldots,T_n]=\mathfrak m.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Let

$$
\mathfrak a=(XY^3,X^2(Y-3)).
$$

Certainly $\mathfrak a\subseteq(X)$, so $\sqrt{\mathfrak a}\subseteq(X)$. Conversely, cubing the second generator shows that $\mathfrak a$ contains $X^6(Y-3)^3$, while multiplying the first generator by $X^5$ shows that it contains $X^6Y^3$. The ideals generated by $Y^3$ and $(Y-3)^3$ are [comaximal ideals](../../../commutative-algebra.md#comaximal-ideals), so a polynomial combination of the two polynomials is $1$. Multiplication by $X^6$ gives $X^6\in\mathfrak a$, hence $X\in\sqrt{\mathfrak a}$. Therefore

$$
\boxed{\sqrt{\mathfrak a}=(X)},
$$

generated by the single polynomial $X$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Write the [finitely generated algebra](../../../algebra.md#finitely-generated-algebra) as

$$
A\cong\mathbb C[T_1,\ldots,T_n]/I.
$$

By the [Weak Hilbert Nullstellensatz](../../../algebraic-geometry.md#weak-hilbert-nullstellensatz), $\mathbb C$-algebra homomorphisms $A\to\mathbb C$ correspond exactly to the points of the [affine algebraic set](../../../algebraic-geometry.md#affine-algebraic-set) $V(I)$.

If $V(I)$ is finite, its cardinality is finite. If it is infinite, the [complex affine algebraic set cardinality dichotomy](../../../algebraic-geometry.md#complex-affine-algebraic-set-cardinality-dichotomy) gives

$$
|V(I)|=|\mathbb C|,
$$

which is uncountable. This also covers the zero algebra, whose homomorphism set is empty. Therefore

$$
\boxed{|\operatorname{Hom}_{\mathbb C}(A,\mathbb C)|\ne\aleph_0}.
$$

## 4

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For a prime ideal $\mathfrak p$, its height is the supremum of lengths $r$ of strict chains

$$
\mathfrak p_0\subsetneq\mathfrak p_1\subsetneq\cdots\subsetneq\mathfrak p_r=\mathfrak p.
$$

The [height of an ideal](../../../commutative-algebra.md#height-of-an-ideal) $I$, without assuming $I$ prime, is

$$
\boxed{\operatorname{ht}(I)=
\inf_{\mathfrak p\supseteq I}\operatorname{ht}(\mathfrak p)}.
$$

The [Krull dimension](../../../commutative-algebra.md#krull-dimension) of a ring $R$ is

$$
\boxed{\dim R=\sup\{r:\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_r
\text{ are prime ideals of }R\}}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/a">a</h4>

↑ **Parent:** [Ii](#4/ii)

<h5 id="4/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#4/ii/a)

For the maximal ideal $\mathfrak m$ of $(A,\mathfrak m)$, the [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) is

$$
G_{\mathfrak m}(A)
=\operatorname{gr}_{\mathfrak m}(A)
=\bigoplus_{n\geq0}\mathfrak m^n/\mathfrak m^{n+1}.
$$

If $x+\mathfrak m^{r+1}$ and $y+\mathfrak m^{s+1}$ are homogeneous classes, their product is

$$
xy+\mathfrak m^{r+s+1}.
$$

It is a graded algebra over the residue field $k=A/\mathfrak m$.

The [Hilbert series](../../../commutative-algebra.md#hilbert-series) is

$$
H_{G_{\mathfrak m}(A)}(t)
=\sum_{n\geq0}
\dim_k(\mathfrak m^n/\mathfrak m^{n+1})t^n.
$$

The Hilbert-Serre theorem makes this rational. The number $d(G_{\mathfrak m}(A))$ is the order of its pole at $t=1$, as recorded by the [pole dimension of an associated graded ring](../../../commutative-algebra.md#pole-dimension-of-an-associated-graded-ring).

The [Dimension theorem for Noetherian local rings](../../../commutative-algebra.md#dimension-theorem-for-noetherian-local-rings) states

$$
\boxed{\dim A
=\dim G_{\mathfrak m}(A)
=d(G_{\mathfrak m}(A))}.
$$

<h4 id="4/ii/b">b</h4>

↑ **Parent:** [Ii](#4/ii)

<h5 id="4/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#4/ii/b)

Put $\overline A=A/(x)$ and $\overline{\mathfrak m}=\mathfrak m/(x)$. Applying the dimension theorem to $A$ and $\overline A$ gives

$$
d(G_{\overline{\mathfrak m}}(\overline A))
=\dim\overline A,
\qquad
d(G_{\mathfrak m}(A))=\dim A.
$$

Since $x$ is a non-zero-divisor, it belongs to no minimal prime of the Noetherian ring $A$. Any chain of primes in $A/(x)$ lifts to a chain

$$
\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_r
$$

of primes of $A$ containing $x$. A minimal prime $\mathfrak q\subseteq\mathfrak p_0$ cannot contain $x$, so the inclusion is strict. Prepending $\mathfrak q$ gives a chain of length $r+1$ in $A$. Thus the [dimension drop by a non-zero-divisor](../../../commutative-algebra.md#dimension-drop-by-a-non-zero-divisor) gives

$$
\dim(A/(x))\leq\dim A-1.
$$

Combining these equalities proves

$$
\boxed{d(G_{\mathfrak m/(x)}(A/(x)))
\leq d(G_{\mathfrak m}(A))-1}.
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The polynomial ring $\mathbb C[X,Y]$ is a two-dimensional [unique factorization domain](../../../algebra.md#unique-factorization-domain). Let $\mathfrak p$ be a prime ideal containing $(f,g)$. Since $f\ne0$, the prime $\mathfrak p$ is nonzero. If it were not maximal, it would have height one, so the [height-one prime in a unique factorization domain](../../../algebra.md#height-one-prime-in-a-unique-factorization-domain) would give $\mathfrak p=(h)$ for an irreducible polynomial $h$. Then $h$ would divide both $f$ and $g$, contrary to the hypothesis. Every prime of

$$
R=\mathbb C[X,Y]/(f,g)
$$

is therefore maximal.

The [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem) makes $R$ Noetherian, and it has Krull dimension zero by the preceding paragraph. The [Noetherian dimension-zero criterion for an Artinian ring](../../../algebra.md#noetherian-dimension-zero-criterion-for-an-artinian-ring) now shows that

$$
\boxed{R\text{ is Artinian}}.
$$

## 5

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

A [discrete valuation](../../../commutative-algebra.md#discrete-valuation) on a field $K$ is a surjective group homomorphism

$$
v:K^\times\longrightarrow\mathbb Z
$$

satisfying

$$
v(x+y)\geq\min\{v(x),v(y)\}
$$

whenever $x+y\ne0$. Its [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) is

$$
\boxed{R_v=\{0\}\cup\{x\in K^\times:v(x)\geq0\}}.
$$

One standard characterization defines a [Dedekind domain](../../../commutative-algebra.md#dedekind-domain) as a Noetherian integrally closed domain of Krull dimension one. Equivalently, all its localizations at nonzero prime ideals are discrete valuation rings.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Choose $0\ne a\in\mathfrak m$. Since the one-dimensional local domain has no nonzero prime ideal other than $\mathfrak m$, one has $\sqrt{(a)}=\mathfrak m$. Finite generation of $\mathfrak m$ therefore gives some $n\geq1$ with $\mathfrak m^n\subseteq(a)$. Choose $n$ minimal and

$$
x\in\mathfrak m^{n-1}\setminus(a).
$$

In the fraction field of $A$, put $y=x/a$. Then $y\notin A$ but

$$
y\mathfrak m\subseteq A.
$$

If $y\mathfrak m\subseteq\mathfrak m$, multiplication by $y$ would preserve the nonzero finitely generated faithful $A$-module $\mathfrak m$. The [determinant trick](../../../module-theory.md#determinant-trick) would make $y$ integral over $A$, contradicting that $A$ is integrally closed and $y\notin A$. Hence some $t\in\mathfrak m$ satisfies $yt\notin\mathfrak m$. Since $yt\in A$ and $A$ is local, $yt$ is a unit.

For any $z\in\mathfrak m$, one has $yz\in A$, and therefore

$$
\frac zt=\frac{yz}{yt}\in A.
$$

Thus $\mathfrak m\subseteq(t)$, while the reverse inclusion follows from $t\in\mathfrak m$. Consequently

$$
\boxed{\mathfrak m=(t)}.
$$

This proves the [principal maximal ideal in a one-dimensional normal local domain](../../../commutative-algebra.md#principal-maximal-ideal-in-a-one-dimensional-normal-local-domain) result.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/a">a</h4>

↑ **Parent:** [Iii](#5/iii)

<h5 id="5/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#5/iii/a)

Let $J$ be an ideal of $S^{-1}A$ and contract it to an ideal $I$ of $A$. Every element $a/s\in J$ has $a/1=(s/1)(a/s)\in J$, so $a\in I$ and

$$
J=S^{-1}I.
$$

Because $A$ is a [Noetherian ring](../../../algebra.md#noetherian-ring), write $I=(a_1,\ldots,a_r)$. Then

$$
J=(a_1/1,\ldots,a_r/1),
$$

so every ideal of $S^{-1}A$ is finitely generated. Hence every localization of a Noetherian ring is Noetherian, proving the [Localization of a Noetherian ring](../../../commutative-algebra.md#localization-of-a-noetherian-ring) theorem.

<h4 id="5/iii/b">b</h4>

↑ **Parent:** [Iii](#5/iii)

<h5 id="5/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#5/iii/b)

Because $0\notin S$, the localization $S^{-1}A$ remains an integral domain. Part (a) makes it Noetherian. Integral closedness is preserved by localization: if $x$ in the common fraction field is integral over $S^{-1}A$, clearing the finitely many denominators in a monic equation shows that $sx$ is integral over $A$ for some $s\in S$, whence $sx\in A$ and $x\in S^{-1}A$.

The [prime ideal correspondence for localization](../../../commutative-algebra.md#prime-ideal-correspondence-for-localization) shows that every chain of primes in $S^{-1}A$ comes from a chain in $A$, so

$$
\dim S^{-1}A\leq1.
$$

If its dimension is one, it is a Noetherian integrally closed domain of dimension one and hence a [Dedekind domain](../../../commutative-algebra.md#dedekind-domain). If its dimension is zero, its zero ideal is maximal, so the domain is a field. This proves the [Localization of a Dedekind domain](../../../commutative-algebra.md#localization-of-a-dedekind-domain) alternative.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
