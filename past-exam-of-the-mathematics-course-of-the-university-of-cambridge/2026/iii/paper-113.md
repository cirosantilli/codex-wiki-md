# Paper 113

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20113.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20113.pdf)

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
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $R$ be a [valuation ring](../../../commutative-algebra.md#valuation-ring) with [fraction field](../../../commutative-algebra.md#field-of-fractions) $K$. For every commutative square

$$
\begin{array}{ccc}
\operatorname{Spec}K&\longrightarrow&X\\
\downarrow&&\downarrow f\\
\operatorname{Spec}R&\longrightarrow&Y,
\end{array}
$$

the [valuative criterion for separatedness](../../../ringed-space.md#valuative-criterion-for-separatedness) says that a [finite type morphism](../../../ringed-space.md#morphism-of-finite-type) $f$ between [Noetherian schemes](../../../ringed-space.md#noetherian-scheme) is [separated](../../../ringed-space.md#separated-morphism) exactly when there is at most one dotted lift $\operatorname{Spec}R\to X$ completing the diagram.

Under the same finiteness hypotheses, the [valuative criterion for properness](../../../ringed-space.md#valuative-criterion-for-properness) says that $f$ is [proper](../../../ringed-space.md#proper-morphism) exactly when every such square has a unique lift. Thus separatedness supplies uniqueness, while properness supplies existence as well.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The composite $g\circ f$ is [proper](../../../ringed-space.md#proper-morphism), hence separated. If two lifts $\operatorname{Spec}R\to X$ solve a valuation-ring lifting problem for $f$, they also solve the corresponding problem for $g\circ f$. The [valuative criterion for separatedness](../../../ringed-space.md#valuative-criterion-for-separatedness) for $g\circ f$ makes them equal, so $f$ is separated.

It remains to prove existence. Start with a square

$$
\begin{array}{ccc}
\operatorname{Spec}K&\xrightarrow{u}&X\\
\downarrow&&\downarrow f\\
\operatorname{Spec}R&\xrightarrow{v}&Y.
\end{array}
$$

After composing the lower map with $g$, properness of $g\circ f$ gives a lift $a:\operatorname{Spec}R\to X$ over $Z$ whose generic restriction is $u$. The two maps $f\circ a$ and $v$ from $\operatorname{Spec}R$ to $Y$ agree on $\operatorname{Spec}K$ and have the same composite with $g$. Since $g$ is separated, its valuative uniqueness criterion gives $f\circ a=v$. Hence $a$ is the required lift for $f$.

The morphism $f$ is of finite type by hypothesis, and it is separated and satisfies valuative existence. The [valuative criterion for properness](../../../ringed-space.md#valuative-criterion-for-properness) therefore proves that $f$ is proper.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $R$ be a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) with [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$, [fraction field](../../../commutative-algebra.md#field-of-fractions) $K$, and normalized discrete valuation $\nu:K^\times\to\mathbb Z$. A map $\operatorname{Spec}K\to\mathbb P^n_{\mathbb Z}$ is a [projective point](../../../projective-space.md#projective-point)

$$
[a_0:\cdots:a_n],\qquad a_i\in K,
$$

with at least one nonzero coordinate. Put $m=\min_{a_i\ne0}\nu(a_i)$ and set $b_i=\pi^{-m}a_i$. Then every $b_i$ lies in $R$, and at least one $b_j$ is a unit.

On the standard affine chart $U_j$ of [projective space](../../../projective-space.md), the ratios $b_i/b_j$ all lie in $R$. They therefore define a map $\operatorname{Spec}R\to U_j\subseteq\mathbb P^n_{\mathbb Z}$ whose generic restriction is the original point. This proves existence in the DVR case. The assumed separatedness of $\mathbb P^n_{\mathbb Z}\to\operatorname{Spec}\mathbb Z$, through the [valuative criterion for separatedness](../../../ringed-space.md#valuative-criterion-for-separatedness), gives uniqueness. Thus the morphism satisfies the requested DVR form of the [valuative criterion for properness](../../../ringed-space.md#valuative-criterion-for-properness).

## 2

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [tensor product of sheaves](../../../ringed-space.md#tensor-product-of-sheaves) $\mathcal F\otimes_{\mathcal O_X}\mathcal G$ is the sheafification of the presheaf

$$
U\longmapsto\mathcal F(U)\otimes_{\mathcal O_X(U)}\mathcal G(U).
$$

Equivalently, its stalk at $x$ is $\mathcal F_x\otimes_{\mathcal O_{X,x}}\mathcal G_x$.

The [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) is defined on each open set $V\subseteq Y$ by

$$
(f_*\mathcal F)(V)=\mathcal F(f^{-1}V).
$$

The [pullback of a sheaf of modules](../../../ringed-space.md#pullback-of-a-sheaf-of-modules) is

$$
f^*\mathcal E=\mathcal O_X\otimes_{f^{-1}\mathcal O_Y}f^{-1}\mathcal E,
$$

where $f^{-1}\mathcal E$ is the [inverse image sheaf](../../../ringed-space.md#inverse-image-sheaf) and the tensor product uses the structural morphism $f^{-1}\mathcal O_Y\to\mathcal O_X$ of the given [ringed-space morphism](../../../ringed-space.md#morphism-of-ringed-spaces).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The $\mathcal O_Y$-module $\mathcal E$ is a [locally free sheaf](../../../ringed-space.md#locally-free-sheaf) of finite rank if every $y\in Y$ has an open neighborhood $V$ and a finite integer $r$ for which

$$
\mathcal E|_V\cong\mathcal O_V^{\oplus r}.
$$

The rank is locally constant and is therefore constant on each connected component.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The adjunction morphism $f^{-1}f_*\mathcal F\to\mathcal F$, together with $f^{-1}\mathcal E\to f^*\mathcal E$, gives

$$
f^{-1}(f_*\mathcal F\otimes_{\mathcal O_Y}\mathcal E)
\longrightarrow
\mathcal F\otimes_{\mathcal O_X}f^*\mathcal E.
$$

Adjunction between the [inverse image sheaf](../../../ringed-space.md#inverse-image-sheaf) and [direct image sheaf](../../../ringed-space.md#direct-image-sheaf) turns this into the [projection formula for sheaves](../../../ringed-space.md#projection-formula) morphism

$$
f_*\mathcal F\otimes_{\mathcal O_Y}\mathcal E
\longrightarrow
f_*\bigl(\mathcal F\otimes_{\mathcal O_X}f^*\mathcal E\bigr).
$$

On local sections it sends a pure tensor $s\otimes e$ over $V\subseteq Y$ to $s\otimes f^\#e$ over $f^{-1}V$.

Whether this morphism is an isomorphism is local on $Y$. If $\mathcal E|_V\cong\mathcal O_V^{\oplus r}$ for finite $r$, its restriction becomes the canonical identification

$$
(f_*\mathcal F|_V)^{\oplus r}
\longrightarrow
f_*\bigl(\mathcal F|_{f^{-1}V}^{\oplus r}\bigr)
=(f_*\mathcal F|_V)^{\oplus r}.
$$

**Thus the projection-formula morphism is an isomorphism whenever $\mathcal E$ is [locally free](../../../ringed-space.md#locally-free-sheaf) of finite rank.**

## 3

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For an indexed open cover $\mathcal U=(U_i)_{i\in I}$ and a sheaf $\mathcal F$, the [Čech cohomology](../../../ringed-space.md#cech-cohomology) cochain groups are

$$
\check C^p(\mathcal U,\mathcal F)
=\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}).
$$

The differential is the alternating sum of restrictions:

$$
(dc)_{i_0\ldots i_{p+1}}
=\sum_{j=0}^{p+1}(-1)^j
c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}
\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

Since $d^2=0$, the cohomology

$$
\check H^p(\mathcal U,\mathcal F)
=\ker(d:\check C^p\to\check C^{p+1})/operatorname{im}(d:\check C^{p-1}\to\check C^p)
$$

is well defined.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $A=k[x,y]$ and $\mathfrak m=(x,y)$. Since $f(0,0)\ne0$, the [principal open subscheme](../../../ringed-space.md#principal-open-subscheme) $D(f)=\operatorname{Spec}A_f$ contains $\mathfrak m$, and

$$
V=D(f)\setminus\{\mathfrak m\}.
$$

Cover $V$ by the two affine opens $D(xf)$ and $D(yf)$, whose intersection is $D(xyf)$. The degree-zero part of the resulting [Čech cohomology](../../../ringed-space.md#cech-cohomology) complex gives

$$
H^0(V,\mathcal O_V)=A_{xf}\cap A_{yf}=A_f
$$

inside the [fraction field](../../../commutative-algebra.md#field-of-fractions) of $A$. The last equality follows because $A_f$ is a [unique factorization domain](../../../algebra.md#unique-factorization-domain) and a rational function regular after localizing at both $x$ and $y$ has no possible prime factor left in its denominator.

The same affine cover is acyclic, so its degree-one Čech group computes [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) and gives

$$
H^1(V,\mathcal O_V)
\cong A_{xyf}/(A_{xf}+A_{yf}).
$$

Before localizing at $f$, the quotient

$$
Q=A_{xy}/(A_x+A_y)
$$

has the $k$-basis

$$
\{x^{-a}y^{-b}:a,b\geq1\}.
$$

Writing $f=c+h$ with $c=f(0,0)\in k^\times$ and $h\in(x,y)$, multiplication by $h$ is locally nilpotent on $Q$: for each negative monomial, a sufficiently high power of $(x,y)$ moves every term into $A_x+A_y$. Hence $c+h$ acts invertibly on $Q$ by a finite geometric series on each element. Localizing at $f$ therefore leaves $Q$ unchanged, and

$$
H^1(V,\mathcal O_V)\cong Q_f\cong Q.
$$

The displayed infinite basis proves that this vector space is infinite-dimensional.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the cover $\mathcal U=\{X_1,X_2\}$ of the [affine plane with doubled origin](../../../ringed-space.md#affine-plane-with-doubled-origin), the overlap is the [punctured affine plane](../../../ringed-space.md#punctured-affine-plane) $U$. Since $H^0(U,\mathcal O_U)=k[x,y]$, the Čech complex begins

$$
k[x,y]\oplus k[x,y]\longrightarrow k[x,y],
\qquad (a,b)\longmapsto b-a.
$$

This map is surjective, and the normalized complex has no terms in degrees at least two. Consequently

$$
\check H^p(\mathcal U,\mathcal O_Y)=0\qquad(p>0).
$$

The [Mayer-Vietoris sequence for sheaf cohomology](../../../ringed-space.md#mayer-vietoris-sequence-for-sheaf-cohomology) also gives $H^1(Y,\mathcal O_Y)=0$, but its next part gives

$$
H^2(Y,\mathcal O_Y)\cong H^1(U,\mathcal O_U).
$$

Part b with $f=1$ shows that the group on the right is infinite-dimensional. Thus

$$
\check H^2(\mathcal U,\mathcal O_Y)=0
\ne H^2(Y,\mathcal O_Y).
$$

This does not contradict the [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem). Although $X_1$ and $X_2$ are affine, their intersection $U$ is not acyclic: it has nonzero first structure-sheaf cohomology. Equivalently, this affine cover does not satisfy the theorem's hypotheses; the doubled-origin plane is not a [semi-separated scheme](../../../ringed-space.md#semi-separated-scheme).

## 4

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) $i:Z\to X$ is a [closed immersion](../../../ringed-space.md#closed-immersion) if it identifies $Z$ homeomorphically with a closed subset of $X$ and the morphism of sheaves

$$
\mathcal O_X\longrightarrow i_*\mathcal O_Z
$$

is surjective. Equivalently, every point of $X$ has an affine neighborhood $\operatorname{Spec}A$ on which $i$ is isomorphic to $\operatorname{Spec}(A/I)\to\operatorname{Spec}A$ for some [ideal](../../../commutative-algebra.md#ideal) $I\subseteq A$.

A [closed subscheme](../../../ringed-space.md#closed-subscheme) of $X$ is a scheme $Z$ supplied with a closed immersion $Z\hookrightarrow X$, considered up to isomorphism over $X$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

On an affine open $W=\operatorname{Spec}A\subseteq X$, write $Z\cap W=V(I)$. Give $Z\cap W$ the [reduced induced subscheme](../../../ringed-space.md#reduced-induced-subscheme) structure $\operatorname{Spec}(A/\sqrt I)$. These constructions agree under localization and therefore glue to a reduced closed subscheme $Z\hookrightarrow X$.

Let $Z'\hookrightarrow X$ be another [closed immersion](../../../ringed-space.md#closed-immersion) with the same underlying closed set. Affine-locally write $Z'=\operatorname{Spec}(A/J)$. Since $V(J)=Z\cap W$, its vanishing ideal is $\sqrt J=\sqrt I$, and the inclusion $J\subseteq\sqrt J$ induces a quotient homomorphism

$$
A/J\longrightarrow A/\sqrt J.
$$

Contravariance of the [spectrum of a commutative ring](../../../ringed-space.md#spectrum-of-a-commutative-ring) gives a factorization

$$
Z\cap W\longrightarrow Z'\cap W\longrightarrow W.
$$

The quotient maps force these local factorizations to agree on overlaps, so they glue. They are also the only possible maps over $X$, which proves uniqueness.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write $X=\operatorname{Spec}B$, $Y=\operatorname{Spec}A$, and let the morphism correspond to a homomorphism $\varphi:A\to B$. Put $I=\ker\varphi$ and

$$
Z=\operatorname{Spec}(A/I).
$$

The injection $A/I\hookrightarrow B$ gives $X\to Z$, and the quotient $A\to A/I$ gives a [closed immersion](../../../ringed-space.md#closed-immersion) $Z\hookrightarrow Y$, so $f$ factors through $Z$.

If $f$ factors through another closed subscheme $Z'=\operatorname{Spec}(A/J)$, then $J\subseteq\ker\varphi=I$. The resulting quotient $A/J\to A/I$ induces the unique factorization $Z\to Z'\to Y$. Thus $Z$ is the [scheme-theoretic image](../../../ringed-space.md#scheme-theoretic-image).

It remains to identify its underlying set. A [principal open subscheme](../../../ringed-space.md#principal-open-subscheme) $D(a)\subseteq\operatorname{Spec}A$ misses $f(X)$ exactly when $D(\varphi(a))$ is empty, equivalently when $\varphi(a)$ is a [nilpotent element](../../../commutative-algebra.md#nilpotent). Hence the ideal of functions vanishing set-theoretically on $f(X)$ has radical $\sqrt{\ker\varphi}$. The closure is therefore

$$
V(\sqrt{\ker\varphi})=V(\ker\varphi)=|Z|,
$$

as required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
