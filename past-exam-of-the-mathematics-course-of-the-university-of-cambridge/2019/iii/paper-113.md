# Paper 113

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_113.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_113.pdf)

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
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
    - [iv](#4/c/iv)
      - [Solution](#4/c/iv/solution)

## 1

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write the [affine scheme](../../../ringed-space.md#affine-scheme) as $U=\operatorname{Spec}B$. A point $x\in U$ corresponds to a [prime ideal](../../../commutative-algebra.md#prime-ideal) $\mathfrak p\subset B$, and its [local ring](../../../commutative-algebra.md#local-ring) is $\mathcal O_{X,x}\cong B_{\mathfrak p}$ with [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $\mathfrak pB_{\mathfrak p}$. Hence

$$
f_x\notin\mathfrak m_x
\iff \bar f/1\notin\mathfrak pB_{\mathfrak p}
\iff \bar f\notin\mathfrak p.
$$

The last condition defines the [principal open subscheme](../../../ringed-space.md#principal-open-subscheme) $D(\bar f)$, so

$$
\boxed{U\cap X_f=D(\bar f).}
$$

Every point of the [scheme](../../../ringed-space.md#scheme) $X$ has such an affine neighbourhood. Thus $X_f$ is locally open, and hence is open in the [Zariski topology](../../../algebraic-geometry.md#zariski-topology).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Choose an [open cover](../../../topology.md#open-cover) of $X$ by affine opens $U_i=\operatorname{Spec}B_i$. Since $X$ is a [quasi-compact topological space](../../../topology.md#compact-space), finitely many suffice. Let $f_i,a_i\in B_i$ be the restrictions of $f,a$. Part (a) identifies $U_i\cap X_f$ with $D(f_i)$, whose ring of [regular functions](../../../ringed-space.md#regular-function) is the [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) $(B_i)_{f_i}$. The vanishing of $a$ there means

$$
a_i/1=0\quad\hbox{in }(B_i)_{f_i},
$$

so $f_i^{n_i}a_i=0$ for some $n_i\geq0$. Taking $n>0$ at least as large as every $n_i$ gives $(f^na)|_{U_i}=0$ on every member of the finite cover. The local identity axiom for the [sheaf of rings](../../../ringed-space.md#sheaf-of-rings) $\mathcal O_X$ therefore gives

$$
\boxed{f^na=0\text{ in }\Gamma(X,\mathcal O_X).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $X=\bigcup_{i=1}^rU_i$ be the stated finite affine cover. By the description of sections on a [principal open subscheme](../../../ringed-space.md#principal-open-subscheme), after increasing denominators separately we may write

$$
b|_{(U_i)_f}=a_i/f^{n_i}
$$

for some $a_i\in\Gamma(U_i,\mathcal O_X)$. Multiplying the numerators by powers of $f$ lets us use one exponent $n$ for every $i$.

On $W_{ij}=U_i\cap U_j$, the section $a_i-a_j$ vanishes after restriction to $(W_{ij})_f$. Each $W_{ij}$ is [quasi-compact](../../../topology.md#compact-space), so part (b) supplies $m_{ij}$ with $f^{m_{ij}}(a_i-a_j)=0$ on $W_{ij}$. Choose one $m$ valid for all the finitely many pairs. The sections $f^ma_i$ now agree on every overlap, and the gluing axiom of a [sheaf of rings](../../../ringed-space.md#sheaf-of-rings) produces $a\in\Gamma(X,\mathcal O_X)$ with $a|_{U_i}=f^ma_i$. On $X_f$,

$$
a=f^{m+n}b.
$$

Thus **some power of $f$ times $b$ extends to a global [regular function](../../../ringed-space.md#regular-function) on $X$**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Restriction and division by powers of $f$ define a natural [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism)

$$
\Phi:A_f\longrightarrow\Gamma(X_f,\mathcal O_{X_f}),
\qquad a/f^n\longmapsto f^{-n}a|_{X_f}.
$$

If $\Phi(a/f^n)=0$, then $a|_{X_f}=0$, and part (b) gives $f^ma=0$ for some $m$; this is exactly the criterion that $a/f^n=0$ in the [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) $A_f$. Hence $\Phi$ is injective. Given $b$ in the target, part (c) gives $f^Nb=a|_{X_f}$ for some $a\in A$, so $b=\Phi(a/f^N)$. Hence $\Phi$ is surjective and

$$
\boxed{\Gamma(X_f,\mathcal O_{X_f})\cong A_f.}
$$

## 2

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Condition (i) implies (ii) immediately by taking the open set $U=X$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Every restriction map of the [structure sheaf of a scheme](../../../ringed-space.md#structure-sheaf-of-a-scheme) is a unital [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism). Thus $p\cdot1=0$ in $\Gamma(X,\mathcal O_X)$ implies the same identity in $\Gamma(U,\mathcal O_X)$ for every open $U$. This proves (ii)$\Rightarrow$(i), so (i) and (ii) are equivalent.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The unique [structure morphism](../../../ringed-space.md#structure-morphism) $X\to\operatorname{Spec}\mathbb Z$ factors through the [closed subscheme](../../../ringed-space.md#closed-subscheme) $\operatorname{Spec}(\mathbb Z/p\mathbb Z)$ exactly when the ideal sheaf $p\mathcal O_X$ is zero. By (i), this is equivalent to all rings of local sections having [characteristic of a ring](../../../commutative-algebra.md#characteristic-of-a-ring) $p$. Therefore

$$
\boxed{\text{(i)},\ \text{(ii)},\ \text{and (iii) are equivalent}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

On every open set $U$, define $F_U^\#(a)=a^p$. In [characteristic of a ring](../../../commutative-algebra.md#characteristic-of-a-ring) $p$, the [binomial theorem](../../../combinatorics.md#binomial-theorem) gives $(a+b)^p=a^p+b^p$, so these are [ring homomorphisms](../../../commutative-algebra.md#ring-homomorphism); they commute with restrictions and hence define a morphism of [sheaves of rings](../../../ringed-space.md#sheaf-of-rings).

On an affine chart $\operatorname{Spec}A$, the inverse image of a [prime ideal](../../../commutative-algebra.md#prime-ideal) $\mathfrak p$ under the [Frobenius endomorphism](../../../galois-theory.md#frobenius-endomorphism) is

$$
\{a:a^p\in\mathfrak p\}=\mathfrak p,
$$

by primality. The induced continuous map is therefore the identity. These local morphisms agree on overlaps, giving the [Absolute Frobenius morphism](../../../ringed-space.md#absolute-frobenius-morphism) $F_X:X\to X$. Its action on the underlying space and on every local section was prescribed, so the morphism is unique.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take

$$
X=\mathbb P_{\mathbb F_p}^1.
$$

The [global regular functions on projective space](../../../projective-space.md#global-regular-functions-on-projective-space) give $\Gamma(X,\mathcal O_X)=\mathbb F_p$, on which the [Absolute Frobenius morphism](../../../ringed-space.md#absolute-frobenius-morphism) is the identity. On the standard [affine line](../../../ringed-space.md#affine-line) $\operatorname{Spec}\mathbb F_p[t]$, however, its map on functions is $t\mapsto t^p$, which is not surjective. Thus $F_X$ is not an [isomorphism of schemes](../../../ringed-space.md#isomorphism-of-schemes).

Choose the rational closed point $x$ given by $t=0$. The affine formula for a [fibre product of schemes](../../../ringed-space.md#fiber-product-of-schemes) gives its [scheme-theoretic fiber](../../../algebraic-geometry.md#scheme-theoretic-fiber):

$$
F_X^{-1}(x)
=\operatorname{Spec}\left(\mathbb F_p[t]\otimes_{\mathbb F_p[t],\,t\mapsto t^p}\mathbb F_p\right)
\cong\boxed{\operatorname{Spec}\mathbb F_p[t]/(t^p)}.
$$

This is the [Fibre of absolute Frobenius over a rational point of the affine line](../../../algebraic-geometry.md#fibre-of-absolute-frobenius-over-a-rational-point-of-the-affine-line): it is a one-point, length-$p$ [nonreduced scheme](../../../ringed-space.md#nonreduced-scheme), rather than a reduced point.

## 3

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A standard sufficient hypothesis is that $X$ is both a [Noetherian scheme](../../../ringed-space.md#noetherian-scheme) and an [integral scheme](../../../ringed-space.md#integral-scheme), and is [regular in codimension one](../../../ringed-space.md#regular-in-codimension-one); in particular, a Noetherian [normal scheme](../../../ringed-space.md#normal-scheme) qualifies. A [Weil divisor](../../../algebraic-geometry.md#weil-divisor) is then a finite sum

$$
D=\sum_Zn_Z[Z],\qquad n_Z\in\mathbb Z,
$$

over integral codimension-one closed subschemes $Z$. The local ring at the generic point of each $Z$ is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring), so every nonzero [rational function](../../../isolated-singularity.md#rational-function) $g\in k(X)^\times$ has a [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve)

$$
\operatorname{div}(g)=\sum_Zv_Z(g)[Z].
$$

The [divisor class group](../../../algebraic-geometry.md#divisor-class-group) is

$$
\boxed{\operatorname{Cl}(X)=\operatorname{Div}(X)/\operatorname{Prin}(X).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $R=k[x,y,z]/(xy-z^3)$ and let $X=\operatorname{Spec}R$. The ideal $P=(x,z)$ is a height-one [prime ideal](../../../commutative-algebra.md#prime-ideal), because $R/P\cong k[y]$ and $\dim R=2$. It therefore defines a [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) $D=V(x,z)$.

Localizing at $x$ eliminates $y$, giving

$$
R_x\cong k[x,x^{-1},z],
$$

a [unique factorization domain](../../../algebra.md#unique-factorization-domain). The [Nagata theorem for divisor class groups](../../../algebraic-geometry.md#nagata-theorem-for-divisor-class-groups) says that $\operatorname{Cl}(X)$ is generated by the height-one primes containing $x$. Since

$$
R/(x)\cong k[y,z]/(z^3),
$$

the only such prime is $P$, and hence $[D]$ generates. At the generic point of $D$, $y$ is a [unit in a ring](../../../algebra.md#unit-in-a-ring) and $x=z^3/y$, so the order of vanishing is three:

$$
\operatorname{div}(x)=3D.
$$

Thus $3[D]=0$.

This relation has exact order three. Indeed, if a [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) were supported on $D$, its defining rational function would be a unit on $D(x)$. The units of $R_x=k[z][x,x^{-1}]$ are precisely $c x^m$ with $c\in k^\times$ and $m\in\mathbb Z$, whose divisors are $3mD$. Consequently

$$
\boxed{\operatorname{Cl}\bigl(k[x,y,z]/(xy-z^3)\bigr)\cong\mathbb Z/3\mathbb Z,}
$$

generated by $[V(x,z)]$. This is the $n=3$ case of the [Divisor class group of an A-type surface singularity](../../../algebraic-geometry.md#divisor-class-group-of-an-a-type-surface-singularity).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

First prove that $A$ is an [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain). If $u\in\operatorname{Frac}A$ is integral over $A$, then it is integral over $A_x$. Since the [unique factorization domain](../../../algebra.md#unique-factorization-domain) $A_x$ is integrally closed, write $u=a/x^n$ with $a\in A$ and $n\geq0$ minimal. If $n>0$, an integral equation for $u$ gives, after multiplication by a suitable power of $x$,

$$
a^m+c_1a^{m-1}x^n+\cdots+c_mx^{nm}=0.
$$

Hence $a^m\in(x)$. The ideal $(x)$ is prime, so $a\in(x)$, contradicting minimality of $n$. Therefore $n=0$ and $u\in A$.

Now apply the [Nagata theorem for divisor class groups](../../../algebraic-geometry.md#nagata-theorem-for-divisor-class-groups). The class group of $A_x$ vanishes by the [divisor-class criterion for unique factorization](../../../algebraic-geometry.md#divisor-class-criterion-for-unique-factorization). Hence $\operatorname{Cl}(A)$ is generated by height-one primes that meet $\{1,x,x^2,\ldots\}$. Such a prime contains $x$ and must equal $(x)$, because the [Krull principal ideal theorem](../../../commutative-algebra.md#krull-principal-ideal-theorem) makes the nonzero prime $(x)$ itself height one. Its divisor class is principal, so $\operatorname{Cl}(A)=0$. A second application of the divisor-class criterion yields

$$
\boxed{A\text{ is a unique factorization domain}.}
$$

This argument is the [Nagata criterion for unique factorization domains](../../../algebra.md#nagata-criterion-for-unique-factorization-domains).

## 4

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose an ordering of the index set $I$. The degree-$q$ [Čech cochain group](../../../ringed-space.md#cech-cochain-group) is

$$
\check C^q(\mathcal U,\mathcal F)
=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_q}).
$$

For $s=(s_{i_0\cdots i_q})$, the [Čech coboundary](../../../ringed-space.md#cech-coboundary) is the alternating sum of restrictions

$$
(\delta s)_{i_0\cdots i_{q+1}}
=\sum_{j=0}^{q+1}(-1)^j
s_{i_0\cdots\widehat{i_j}\cdots i_{q+1}}
\big|_{U_{i_0}\cap\cdots\cap U_{i_{q+1}}}.
$$

The identity $\delta^2=0$ makes this the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex), and the required [Čech cohomology](../../../ringed-space.md#cech-cohomology) is

$$
\boxed{\check H^q(\mathcal U,\mathcal F)=\ker(\delta:\check C^q\to\check C^{q+1})/\operatorname{im}(\delta:\check C^{q-1}\to\check C^q).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) is

$$
H^p(\mathbb P_k^r,\mathcal O(n))\cong
\begin{cases}
k[x_0,\ldots,x_r]_n,&p=0,\ n\geq0,\\
k[x_0,\ldots,x_r]_{-n-r-1}^{*},&p=r,\ n\leq-r-1,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular, $H^i(X,\mathcal O_X)=H^i(X,\mathcal O_X(1))=0$ for $i>0$, while $H^0(X,\mathcal O_X)=k$ and $H^0(X,\mathcal O_X(1))\cong k^{r+1}$.

Apply the [long exact sequence in cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) to the displayed [Euler sequence](../../../algebraic-geometry.md#euler-sequence). Its degree-zero part is

$$
0\longrightarrow k\longrightarrow (k^{r+1})^{\oplus(r+1)}
\longrightarrow H^0(X,\mathcal T)\longrightarrow0,
$$

and all later terms vanish. The first map sends $1$ to the tuple of homogeneous coordinates and is injective. Therefore

$$
\boxed{H^i(X,\mathcal T)\cong
\begin{cases}
k^{(r+1)^2-1},&i=0,\\
0,&i>0.
\end{cases}}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

For the [closed immersion](../../../ringed-space.md#closed-immersion) $i:Y\hookrightarrow X$, the [ideal sheaf of a closed subscheme](../../../ringed-space.md#ideal-sheaf-of-a-closed-subscheme) gives

$$
0\longrightarrow\mathcal I_{Y/X}\longrightarrow\mathcal O_X
\longrightarrow i_*\mathcal O_Y\longrightarrow0.
$$

Because the [projective hypersurface](../../../algebraic-geometry.md#projective-hypersurface) is cut out by one [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) $f$ of degree $d$, multiplication by $f$ identifies

$$
\boxed{\mathcal I_{Y/X}\cong\mathcal O_X(-d)=\mathcal O_X(1)^{\otimes(-d)}.}
$$

This is the [ideal-sheaf sequence of a projective hypersurface](../../../algebraic-geometry.md#ideal-sheaf-sequence-of-a-projective-hypersurface).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Tensor the sequence from part (i) with the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) $\mathcal O_X(n)$:

$$
0\longrightarrow\mathcal O_X(n-d)\xrightarrow{\cdot f}\mathcal O_X(n)
\longrightarrow i_*\mathcal O_Y(n)\longrightarrow0.
$$

Its [long exact sequence in cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) contains

$$
H^0(X,\mathcal O_X(n))\longrightarrow H^0(Y,\mathcal O_Y(n))
\longrightarrow H^1(X,\mathcal O_X(n-d)).
$$

Since $\dim Y\geq1$, we have $r\geq2$, and the final group is intermediate cohomology of projective space. It vanishes by the [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space). Hence

$$
\boxed{H^0(X,\mathcal O_X(n))\twoheadrightarrow H^0(Y,\mathcal O_Y(n))\quad\text{for every }n\in\mathbb Z.}
$$

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Set $n=0$ in part (ii). The constants give an injection $k\hookrightarrow H^0(Y,\mathcal O_Y)$ because the [projective hypersurface](../../../algebraic-geometry.md#projective-hypersurface) $Y$ is nonempty, while part (ii) gives surjectivity. Thus

$$
H^0(Y,\mathcal O_Y)=k.
$$

A disconnected scheme has a nontrivial [idempotent](../../../commutative-algebra.md#idempotent) global regular function, equal to zero and one on its two clopen pieces. A [field](../../../algebra.md#field) has no such idempotent, so the [connectedness from global regular functions](../../../geometry-and-topology.md#connectedness-from-global-regular-functions) criterion gives

$$
\boxed{Y\text{ is connected}.}
$$

<h4 id="4/c/iv">iv</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/c/iv)

Use again the twisted [ideal-sheaf sequence of a projective hypersurface](../../../algebraic-geometry.md#ideal-sheaf-sequence-of-a-projective-hypersurface). For $0<i<\dim Y=r-1$, the relevant part of its [long exact sequence in cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) is

$$
H^i(X,\mathcal O_X(n))\longrightarrow H^i(Y,\mathcal O_Y(n))
\longrightarrow H^{i+1}(X,\mathcal O_X(n-d)).
$$

Both outer terms are intermediate cohomology groups on $\mathbb P_k^r$, because $1\leq i<i+1\leq r-1$. They vanish by the [cohomology of twisting sheaves on projective space](../../../projective-space.md#cohomology-of-twisting-sheaves-on-projective-space). Therefore

$$
\boxed{H^i(Y,\mathcal O_Y(n))=0\qquad(0<i<\dim Y,\ n\in\mathbb Z).}
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
