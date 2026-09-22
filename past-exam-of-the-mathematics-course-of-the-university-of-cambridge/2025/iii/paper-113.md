# Paper 113

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20113.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20113.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take $X=\mathbb R$, $U=(0,1)$, and let $\mathcal F$ be the [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) with value a nonzero abelian group $A$ at $p=3/4$. Cover $V=(-1,1)$ by $V_1=(-1,2/3)$ and $V_2=(1/2,1)$. The presheaf gives $(j^p\mathcal F)(V)=0=(j^p\mathcal F)(V_1)$ and $(j^p\mathcal F)(V_2)=A$. A nonzero section on $V_2$ and the zero section on $V_1$ agree on the overlap, whose skyscraper sections vanish, but cannot be glued on $V$. Thus $j^p\mathcal F$ need not be a sheaf.

[Sheafification](../../../ringed-space.md#sheafification) preserves [stalks](../../../ringed-space.md#stalk-of-a-sheaf). If $P\in U$, neighborhoods contained in $U$ are cofinal, so $(j^p\mathcal F)_P=\mathcal F_P$. If $P\notin U$, no neighborhood of $P$ lies in $U$, so every term defining the presheaf stalk is zero. Therefore

$$
(j_!\mathcal F)_P\cong
\begin{cases}
\mathcal F_P,&P\in U,\\
0,&P\notin U.
\end{cases}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On the defining presheaf, send a section over $V\subseteq U$ by the identity

$$
(j^{-1}\mathcal G)(V)=\mathcal G(V)\longrightarrow\mathcal G(V),
$$

and use the unique zero map when $V\nsubseteq U$. These maps commute with restrictions and therefore sheafify to the natural counit

$$
j_!j^{-1}\mathcal G\longrightarrow\mathcal G.
$$

After restricting $j^p\mathcal F$ back to $U$, every open set lies in $U$, so one recovers the original sheaf $\mathcal F$. Equivalently, the natural map $\mathcal F\to j^{-1}j_!\mathcal F$ is an isomorphism on every stalk and hence an isomorphism of sheaves.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the counit from part b for the first map and the restriction map $\mathcal G\to i_*i^{-1}\mathcal G$ for the second. Exactness can be checked on stalks. At $P\in U$ the sequence is

$$
0\longrightarrow\mathcal G_P\xrightarrow{1}\mathcal G_P\longrightarrow0,
$$

whereas at $P\in Z$ it is

$$
0\longrightarrow0\longrightarrow\mathcal G_P\xrightarrow{1}\mathcal G_P\longrightarrow0.
$$

Thus

$$
0\longrightarrow j_!j^{-1}\mathcal G\longrightarrow\mathcal G\longrightarrow i_*i^{-1}\mathcal G\longrightarrow0
$$

is a [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $X=\operatorname{Spec}k[x]$ and $U=D(x)$. A global section of $j_!\mathcal O_U$ is a regular function on the integral scheme $U$ whose support is closed in $X$ and contained in $U$. Every nonzero regular function on $U$ has support dense in $X$, so

$$
\Gamma(X,j_!\mathcal O_U)=0.
$$

If this sheaf were [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf), then on the affine scheme $X$ it would be the sheaf associated with this zero module and hence would vanish. Its stalks at points of $U$ are instead $\mathcal O_{U,P}\ne0$ by part a. This contradiction proves that extension by zero need not preserve quasi-coherence.

## 2

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Proj construction](../../../ringed-space.md#proj-construction) has underlying set

$$
\operatorname{Proj}S=\{\mathfrak p:\mathfrak p\text{ is a homogeneous prime ideal and }S_+\nsubseteq\mathfrak p\}.
$$

Its closed sets are $V_+(I)=\{\mathfrak p:I\subseteq\mathfrak p\}$ for homogeneous ideals $I$, and its standard opens are $D_+(f)$. The structure sheaf is characterized by

$$
\mathcal O_{\operatorname{Proj}S}(D_+(f))=(S_f)_0
$$

for homogeneous $f$ of positive degree.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A [closed immersion](../../../ringed-space.md#closed-immersion) identifies its source homeomorphically with a closed subset and induces a surjection from the target structure sheaf to the pushed-forward source structure sheaf.

The quotient map $S\to S/I$ identifies $\operatorname{Proj}(S/I)$ with $V_+(I)\subseteq\operatorname{Proj}S$. On every standard open $D_+(f)$ it induces the surjection

$$
(S_f)_0\longrightarrow((S/I)_f)_0
$$

with kernel $(I_f)_0$. These affine-local maps glue, proving that the natural morphism $\operatorname{Proj}(S/I)\to\operatorname{Proj}S$ is a closed immersion.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

It suffices to compare the localized homogeneous ideals on every $D_+(f)$. If $a\in I$ is homogeneous, choose $N$ so large that $\deg(f^Na)\geq n_0$. Then $f^Na\in I'$, and in $S_f$,

$$
\frac a1=\frac{f^Na}{f^N}.
$$

Thus $I_f\subseteq I'_f$, while the reverse inclusion follows from $I'\subseteq I$. Hence $I_f=I'_f$, so $(I_f)_0=(I'_f)_0$ and the quotient structure sheaves agree on all standard opens. The two quotients define the same closed subscheme of $\operatorname{Proj}S$.

## 3

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) is an integral closed subscheme of codimension one. If $Y$ has generic point $\eta_Y$, regularity in codimension one makes the local ring $\mathcal O_{X,\eta_Y}$ a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) with fraction field $K(X)$. Its normalized [discrete valuation](../../../commutative-algebra.md#discrete-valuation)

$$
\nu_Y:K(X)^*\longrightarrow\mathbb Z
$$

is the order of vanishing along $Y$: writing $f=u\pi^m$ for a unit $u$ and uniformizer $\pi$ gives $\nu_Y(f)=m$. Additivity of exponents makes this a group homomorphism.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Restriction sends a Weil divisor on $X$ to the sum of its components meeting $U$. Every prime divisor on $U$ has a codimension-one closure in the Noetherian scheme $X$, so the induced map $\operatorname{Cl}(X)\to\operatorname{Cl}(U)$ is surjective.

If the class of $D$ restricts to zero, then $D|_U=\operatorname{div}_U(f)$ for some $f\in K(X)^*$. The divisor $D-\operatorname{div}_X(f)$ is supported on $Z$, hence is an integral combination of $Z_1,\ldots,Z_n$. Conversely, every such combination restricts to zero. Therefore

$$
\mathbb Z^n\longrightarrow\operatorname{Cl}(X)\longrightarrow\operatorname{Cl}(U)\longrightarrow0,
$$

where the first map sends the $i$th basis vector to $[Z_i]$, is exact.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

At the generic point of $L_0$, the functions $x_1,x_2$ are units and the equation gives $x_0=x_3^3/(x_1x_2)$. Taking $x_3$ as a uniformizer yields

$$
\nu_{L_0}(x_0/x_3)=3-1=2.
$$

At $L_1$, the functions $x_0,x_2$ are units and $x_1=x_3^3/(x_0x_2)$, so $\nu_{L_1}(x_0/x_3)=-1$. Symmetrically, $\nu_{L_2}(x_0/x_3)=-1$.

The complement of the three lines is $U=D_+(x_3)$, with

$$
U\cong\operatorname{Spec}k[u_0,u_1,u_2]/(u_0u_1u_2-1)
\cong\operatorname{Spec}k[u_0^{\pm1},u_1^{\pm1}].
$$

This [unique factorization domain](../../../algebra.md#unique-factorization-domain) has trivial divisor class group, so part b says that $[L_0],[L_1],[L_2]$ generate $\operatorname{Cl}(X)$. The units on $U$ are scalar multiples of $u_0^au_1^b$, and their boundary valuation vectors are generated by

$$
(2,-1,-1),\qquad(-1,2,-1).
$$

The resulting integer matrix has [Smith normal form](../../../algebra.md#smith-normal-form) $\operatorname{diag}(1,3,0)$. Consequently

$$
\boxed{\operatorname{Cl}(X)\cong
\mathbb Z^3/\langle(2,-1,-1),(-1,2,-1)\rangle
\cong\mathbb Z\oplus\mathbb Z/3\mathbb Z.}
$$

## 4

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For an open cover $\mathcal U=(U_i)$, the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) is

$$
\check C^p(\mathcal U,\mathcal F)
=\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}),
$$

with differential

$$
(\delta c)_{i_0\ldots i_{p+1}}
=\sum_{q=0}^{p+1}(-1)^q
c_{i_0\ldots\widehat{i_q}\ldots i_{p+1}}
\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

Its cohomology is $\check H^p(\mathcal U,\mathcal F)$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Suppose $\mathbb P_k^n$ had a cover by $n$ affine opens. Since projective space is separated, every finite intersection in this cover is affine. The [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem) would therefore compute the cohomology of every quasi-coherent sheaf by its Čech complex. A cover with only $n$ members has no degree-$n$ cochains, so it would imply

$$
H^n(\mathbb P_k^n,\mathcal O(-n-1))=0.
$$

But [top cohomology of projective space](../../../projective-space.md#top-cohomology-of-projective-space) gives

$$
H^n(\mathbb P_k^n,\mathcal O(-n-1))\cong k,
$$

a contradiction. Hence no such affine cover exists.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Choose a frame of a line bundle on each $U_i$. On $U_i\cap U_j$, the frames differ by $g_{ij}\in\mathcal O_X^*(U_i\cap U_j)$, and compatibility on triple intersections is the [Čech cocycle condition](../../../ringed-space.md#cech-cocycle-condition) $g_{ij}g_{jk}=g_{ik}$. Replacing the local frames by units $h_i$ changes $g_{ij}$ by the [Čech coboundary](../../../ringed-space.md#cech-coboundary) $h_i^{-1}h_j$. Conversely, a multiplicative one-cocycle glues the trivial line bundles $\mathcal O_{U_i}$ into a line bundle. Tensor product multiplies cocycles, so

$$
\operatorname{Pic}(\mathcal U)\cong\check H^1(\mathcal U,\mathcal O_X^*).
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A [Cartier divisor](../../../cartier-divisor.md) on an integral scheme is given by an open cover $(U_i)$ and rational functions $f_i\in K(X)^*$ such that $f_i/f_j\in\mathcal O_X^*(U_i\cap U_j)$. Two are linearly equivalent when their quotient is represented by one global rational function. The Cartier class group is the group of Cartier divisors modulo these principal divisors.

Let $\mathcal K_X^*$ be the sheaf of nonzero rational functions. Cartier divisors are the global sections of $\mathcal K_X^*/\mathcal O_X^*$, and the exact sequence

$$
1\longrightarrow\mathcal O_X^*\longrightarrow\mathcal K_X^*
\longrightarrow\mathcal K_X^*/\mathcal O_X^*\longrightarrow1
$$

gives a long exact cohomology sequence. On an integral scheme $\mathcal K_X^*$ is flasque: every nonempty restriction map is the identity on $K(X)^*$. Hence $H^1(X,\mathcal K_X^*)=0$, and exactness gives

$$
\boxed{\operatorname{CaCl}(X)
=\Gamma(X,\mathcal K_X^*/\mathcal O_X^*)/K(X)^*
\cong H^1(X,\mathcal O_X^*).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
