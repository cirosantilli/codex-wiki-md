# Paper 142

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_142.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_142.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 142](paper-142.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $p:\mathbb P(E)\to X$ be the [projectivization of a real vector bundle](../../../fiber-bundle.md#projectivization-of-a-real-vector-bundle), let $L_E$ be its [tautological bundle](../../../fiber-bundle.md#tautological-bundle), and put

$$
u=w_1(L_E)\in H^1(\mathbb P(E);\mathbb F_2).
$$

The mod-two projective bundle formula says that $H^*(\mathbb P(E);\mathbb F_2)$ is a free $H^*(X;\mathbb F_2)$-module on $1,u,\ldots,u^{d-1}$. The [Projective bundle definition of Stiefel–Whitney classes](../../../fiber-bundle.md#projective-bundle-definition-of-stiefel-whitney-classes) is the unique relation

$$
u^d+p^*w_1(E)u^{d-1}+\cdots+p^*w_d(E)=0.
$$

Apply the [splitting principle for real vector bundles](../../../fiber-bundle.md#splitting-principle-for-real-vector-bundles). After an injective pullback, write

$$
E=L_1\oplus\cdots\oplus L_d,
\qquad
E'=L'_1\oplus\cdots\oplus L'_{d'}.
$$

If $x_i=w_1(L_i)$, the projective-bundle relation factors as

$$
\prod_{i=1}^d(u+x_i)=0,
$$

so

$$
w(E)=\prod_{i=1}^d(1+x_i).
$$

The line summands of $E\oplus E'$ are the union of the two lists, hence

$$
w(E\oplus E')=w(E)w(E').
$$

Comparing the degree-$k$ components proves the [Whitney product formula for Stiefel–Whitney classes](../../../fiber-bundle.md#whitney-product-formula-for-stiefel-whitney-classes)

$$
w_k(E\oplus E')=\sum_{i+j=k}w_i(E)w_j(E').
$$

Injectivity of the splitting pullback returns the identity to $X$.

For real line bundles, the transition functions take values in $O(1)=\{\pm1\}$. Tensor product multiplies these signs, while the identification $\{\pm1\}\cong\mathbb Z/2$ turns multiplication into addition. The corresponding degree-one characteristic classes therefore satisfy the [First Stiefel–Whitney class of a tensor product of real line bundles](../../../fiber-bundle.md#first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles) formula

$$
w_1(L\otimes L')=w_1(L)+w_1(L').
$$

Equivalently, this follows from the classification of real line bundles by $H^1(X;\mathbb F_2)$.

Now take $M=\mathbb{RP}^n$ and $E=k\gamma_{\mathbb R}^{1,n+1}$. Since

$$
E=\gamma_{\mathbb R}^{1,n+1}\otimes\mathbb R^k,
$$

a line in $E_x$ is the fixed line $\gamma_x$ tensored with a line in $\mathbb R^k$. Thus the [projectivization of copies of the real tautological line bundle](../../../fiber-bundle.md#projectivization-of-copies-of-the-real-tautological-line-bundle) is

$$
\mathbb P(E)\cong\mathbb{RP}^n\times\mathbb{RP}^{k-1}.
$$

Let $x$ and $v$ be the degree-one generators pulled back from the first and second factors. The [mod-two cohomology ring of real projective space](../../../algebraic-topology.md#mod-two-cohomology-ring-of-real-projective-space) and the [Künneth theorem](../../../cohomology.md#kunneth-theorem) give

$$
H^*(\mathbb P(E);\mathbb F_2)
\cong
\mathbb F_2[x,v]/(x^{n+1},v^k).
$$

The tautological line $L_E$ is the tensor product of the two tautological lines, so $w_1(L_E)=x+v$. In the alternative generator $u=w_1(L_E)$, the same ring is

$$
\mathbb F_2[x,u]/(x^{n+1},(u+x)^k).
$$

The stable tangent-bundle identity

$$
T\mathbb{RP}^n\oplus\mathbf1\cong(n+1)\gamma_{\mathbb R}^{1,n+1}
$$

gives

$$
w(T\mathbb{RP}^n)=(1+x)^{n+1}.
$$

For the vertical part of the [tangent bundle of a projectivized real vector bundle](../../../fiber-bundle.md#tangent-bundle-of-a-projectivized-real-vector-bundle),

$$
\mathbf1\oplus\operatorname{Hom}(L_E,\omega_E)
\cong L_E^*\otimes p^*E.
$$

Each of the $k$ line summands on the right has first Stiefel–Whitney class

$$
w_1(L_E^*\otimes p^*\gamma)=w_1(L_E)+x=v.
$$

The [Whitney product formula for Stiefel–Whitney classes](../../../fiber-bundle.md#whitney-product-formula-for-stiefel-whitney-classes) therefore yields

$$
w(T\mathbb P(E))
=(1+x)^{n+1}(1+v)^k,
$$

the [Total Stiefel–Whitney class of the projectivization of copies of the tautological line](../../../fiber-bundle.md#total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line).

## 2

↑ **Parent:** [Paper 142](paper-142.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Bott isomorphism](../../../algebraic-topology.md#bott-isomorphism) is multiplication by the [Bott element](../../../algebraic-topology.md#bott-element) $\beta\in\widetilde K^0(S^2)$:

$$
K^i(X)\xrightarrow{\ \cong\ }
\widetilde K^i(S^2\wedge X)
\cong K^{i-2}(X).
$$

Together with the [suspension isomorphism](../../../algebraic-topology.md#suspension-isomorphism) and

$$
K^0(\mathrm{pt})=\mathbb Z,
\qquad
K^{-1}(\mathrm{pt})=0,
$$

it gives the [Complex K-theory of a sphere](../../../algebraic-topology.md#complex-k-theory-of-a-sphere)

$$
\widetilde K^i(S^d)\cong K^{i-d}(\mathrm{pt})
\cong
\begin{cases}
\mathbb Z,&i-d\text{ even},\\
0,&i-d\text{ odd}.
\end{cases}
$$

Let

$$
\varnothing=Y_{-1}\subset Y_0\subset\cdots\subset Y_m=Y
$$

be a [CW filtration](../../../algebraic-topology.md#cw-filtration) in which each quotient $Y_r/Y_{r-1}$ is a wedge of even-dimensional spheres. The six-term exact sequence in [Topological K-theory](../../../algebraic-topology.md#topological-k-theory), the sphere calculation, and induction give

$$
K^{-1}(Y_r)=0
$$

and a short exact sequence whose new summand in $K^0(Y_r)$ is free abelian on the newly attached cells. Every such extension splits as an extension of [free abelian groups](../../../group-theory.md#free-abelian-group), so $K^0(Y)$ is free, with one generator for each cell. This proves the [Complex K-theory of an even-cell complex](../../../algebraic-topology.md#complex-k-theory-of-an-even-cell-complex) result.

The exterior product defines

$$
K^0(Y)\otimes K^i(X)\longrightarrow K^i(Y\times X).
$$

For a point it is the identity. Attaching one layer of even cells gives corresponding exact sequences on the source and target; the sphere case is the [suspension isomorphism](../../../algebraic-topology.md#suspension-isomorphism), and induction with the [Five lemma](../../../category-theory.md#five-lemma) proves that the product map remains an isomorphism. This is the [Künneth theorem for complex K-theory with an even-cell factor](../../../algebraic-topology.md#kunneth-theorem-for-complex-k-theory-with-an-even-cell-factor).

For a [mapping torus](../../../algebraic-topology.md#mapping-torus) $T_f$, the [K-theory Wang sequence of a mapping torus](../../../algebraic-topology.md#k-theory-wang-sequence-of-a-mapping-torus) contains

$$
K^{-1}(Z)\xrightarrow{1-f^*}K^{-1}(Z)
\longrightarrow K^0(T_f)
\longrightarrow K^0(Z)\xrightarrow{1-f^*}K^0(Z).
$$

When $K^{-1}(Z)=0$, exactness gives

$$
K^0(T_f)\cong\ker(1-f^*:K^0(Z)\to K^0(Z)).
$$

For $Z=\mathbb{CP}^2\times\mathbb{CP}^2$, the [Complex K-theory of complex projective space](../../../algebraic-topology.md#complex-k-theory-of-complex-projective-space) and the K-theory Künneth isomorphism give

$$
K^0(Z)\cong\mathbb Z[x,y]/(x^3,y^3).
$$

The factor swap interchanges $x$ and $y$. Its invariant subgroup has the basis

$$
1,\quad xy,\quad x^2y^2,\quad x+y,\quad x^2+y^2,\quad xy^2+x^2y.
$$

It follows that the [K-theory of the mapping torus of the factor swap on two complex projective planes](../../../algebraic-topology.md#k-theory-of-the-mapping-torus-of-the-factor-swap-on-two-complex-projective-planes) is

$$
\boxed{K^0(T_f)\cong\mathbb Z^6.}
$$

## 3

↑ **Parent:** [Paper 142](paper-142.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [splitting principle for complex vector bundles](../../../algebraic-topology.md#splitting-principle-for-complex-vector-bundles) says that for every complex vector bundle $E\to X$ there is a map $p:F(E)\to X$ such that $p^*$ is injective on cohomology and

$$
p^*E=L_1\oplus\cdots\oplus L_r
$$

splits into complex line bundles. Write $x_i=c_1(L_i)$ for the formal [Chern roots](../../../algebraic-topology.md#chern-root).

Define the [Chern character](../../../algebraic-topology.md#chern-character) after this injective pullback by

$$
\operatorname{ch}(E)=\sum_{i=1}^r e^{x_i}.
$$

Each homogeneous component is a symmetric polynomial in the $x_i$ with rational coefficients, hence a polynomial in the elementary symmetric functions $c_j(E)$. It therefore descends uniquely to $H^{\mathrm{ev}}(X;\mathbb Q)$ and depends only on $E$. Set

$$
\operatorname{ch}(E-F)=\operatorname{ch}(E)-\operatorname{ch}(F)
$$

on the [Grothendieck group](../../../algebraic-topology.md#grothendieck-group) $K^0(X)$; additivity under direct sums makes this well defined.

If $E$ has roots $x_i$ and $F$ has roots $y_j$, then $E\otimes F$ has roots $x_i+y_j$. Consequently

$$
\begin{aligned}
\operatorname{ch}(E\oplus F)
&=\sum_i e^{x_i}+\sum_j e^{y_j}
=\operatorname{ch}(E)+\operatorname{ch}(F),\\
\operatorname{ch}(E\otimes F)
&=\sum_{i,j}e^{x_i+y_j}
=\left(\sum_i e^{x_i}\right)
\left(\sum_j e^{y_j}\right)
=\operatorname{ch}(E)\operatorname{ch}(F).
\end{aligned}
$$

It also sends the trivial line to $1$, so it is a unital ring homomorphism.

For $S^{2n}$, a generator of $\widetilde K^0(S^{2n})$ is the $n$-fold exterior product of the degree-two [Bott element](../../../algebraic-topology.md#bott-element). The Chern character respects exterior products, and the degree-two Bott element has Chern character equal, up to sign, to the integral generator of $\widetilde H^2(S^2;\mathbb Z)$. Its $n$-fold product maps to the integral top-dimensional generator. Hence the [Chern character on an even-dimensional sphere is integral](../../../algebraic-topology.md#chern-character-on-an-even-dimensional-sphere-is-integral).

Let the formal Chern roots of $E\to S^{2n}$ be $x_1,\ldots,x_r$ and write $p_n=\sum_i x_i^n$. Since

$$
H^{2j}(S^{2n};\mathbb Z)=0
\qquad(0<j<n),
$$

all lower Chern classes $c_1(E),\ldots,c_{n-1}(E)$ vanish. The [Newton identities](../../../polynomial.md#newton-s-identities) then reduce to

$$
p_n=(-1)^{n+1}n\,c_n(E).
$$

The degree-$2n$ term of the Chern character is therefore

$$
\operatorname{ch}_n(E)
=\frac{p_n}{n!}
=(-1)^{n+1}\frac{c_n(E)}{(n-1)!}.
$$

Its evaluation on the [fundamental class](../../../cohomology.md#fundamental-class) is an integer by integrality of the reduced Chern character. Thus

$$
\left\langle c_n(E),[S^{2n}]\right\rangle
$$

is divisible by $(n-1)!$, proving the [Divisibility of the top Chern number on an even-dimensional sphere](../../../algebraic-topology.md#divisibility-of-the-top-chern-number-on-an-even-dimensional-sphere).

## 4

↑ **Parent:** [Paper 142](paper-142.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The cofibration

$$
S(E)\longrightarrow D(E)\longrightarrow\operatorname{Th}(E)
$$

gives the long exact sequence of a pair in [Topological K-theory](../../../algebraic-topology.md#topological-k-theory). Identify $D(E)$ with $X$ by deformation retraction and use multiplication by the [K-theory Thom class](../../../algebraic-topology.md#k-theory-thom-class)

$$
\lambda_E\in\widetilde K^0(\operatorname{Th}(E))
$$

to identify the relative term with $K^*(X)$. Pullback along the zero section sends $\lambda_E$ to the [K-theory Euler class](../../../algebraic-topology.md#k-theory-euler-class)

$$
e^K(E)=\Lambda_{-1}(\overline E).
$$

The map from the relative term to $K^*(D(E))$ is therefore multiplication by $e^K(E)$, giving the [K-theory Gysin sequence of a sphere bundle](../../../algebraic-topology.md#k-theory-gysin-sequence-of-a-sphere-bundle)

$$
\cdots\to
K^i(X)\xrightarrow{\cdot e^K(E)}K^i(X)
\xrightarrow{p^*}K^i(S(E))
\xrightarrow{p_!}K^{i+1}(X)
\to\cdots.
$$

For

$$
Y=S(\gamma_{\mathbb C}^{1,n+1}\oplus\gamma_{\mathbb C}^{1,n+1})
$$

over $\mathbb{CP}^n$, put $t=1-[\overline\gamma]$. The [Complex K-theory of complex projective space](../../../algebraic-topology.md#complex-k-theory-of-complex-projective-space) is

$$
K^0(\mathbb{CP}^n)=\mathbb Z[t]/(t^{n+1}),
\qquad
K^{-1}(\mathbb{CP}^n)=0,
$$

and

$$
e^K(\gamma\oplus\gamma)
=(1-[\overline\gamma])^2=t^2.
$$

The Gysin sequence consequently identifies

$$
K^{-1}(Y)
\cong\ker\left(t^2:\mathbb Z[t]/(t^{n+1})\to
\mathbb Z[t]/(t^{n+1})\right)
=\mathbb Z\{t^{n-1},t^n\}
\cong\mathbb Z^2
$$

for $n\geq1$. This is the [Odd K-theory of the sphere bundle of two tautological lines](../../../algebraic-topology.md#odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines).

If $n=0$, then the base is a point and $Y=S^3$, so $K^{-1}(Y)\cong\mathbb Z$ by [Bott periodicity](../../../algebraic-topology.md#bott-isomorphism).

The [cannibalistic class](../../../algebraic-topology.md#cannibalistic-class) is defined by the identity

$$
\psi^k(\lambda_E)=\rho^k(E)\lambda_E
$$

for the [Adams operation](../../../algebraic-topology.md#adams-operation) $\psi^k$. The Thom class of a direct sum is the product of the pulled-back Thom classes. Applying the ring homomorphism $\psi^k$ gives

$$
\rho^k(E\oplus E')=\rho^k(E)\rho^k(E').
$$

If $L$ is a line bundle, restriction along the zero section gives

$$
(1-\overline L^k)
=\rho^k(L)(1-\overline L),
$$

so

$$
\rho^k(L)
=1+\overline L+\cdots+\overline L^{k-1}.
$$

Let $\delta:K^{-1}(S(E))\to\widetilde K^0(\operatorname{Th}(E))$ be the boundary map. By definition of $p_!$,

$$
\delta x=\lambda_Ep_!(x).
$$

The natural operation $\psi^k$ commutes with $\delta$, and therefore

$$
\lambda_Ep_!(\psi^kx)
=\psi^k(\lambda_Ep_!(x))
=\rho^k(E)\lambda_E\psi^k(p_!(x)).
$$

Cancelling the Thom class proves the [Adams operation and the boundary pushforward of a sphere bundle](../../../algebraic-topology.md#adams-operation-and-the-boundary-pushforward-of-a-sphere-bundle) formula

$$
p_!(\psi^kx)=\rho^k(E)\psi^k(p_!(x)).
$$

Choose the basis $a,b$ of $K^{-1}(Y)$ characterized by

$$
p_!(a)=t^{n-1},
\qquad
p_!(b)=t^n.
$$

For $E=\gamma\oplus\gamma$,

$$
\rho^2(E)=(1+\overline\gamma)^2=(2-t)^2,
\qquad
\psi^2(t)=1-\overline\gamma^2=2t-t^2=t(2-t).
$$

Modulo $t^{n+1}$, this gives

$$
\begin{aligned}
p_!(\psi^2a)
&=(2-t)^2\bigl(t(2-t)\bigr)^{n-1}\\
&=2^{n+1}t^{n-1}-(n+1)2^nt^n,\\
p_!(\psi^2b)
&=(2-t)^2\bigl(t(2-t)\bigr)^n
=2^{n+2}t^n.
\end{aligned}
$$

Since $p_!$ identifies $K^{-1}(Y)$ with this kernel, the [Second Adams operation on the odd K-theory of the sphere bundle of two tautological lines](../../../algebraic-topology.md#second-adams-operation-on-the-odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines) is

$$
\psi^2(a)=2^{n+1}a-(n+1)2^nb,
\qquad
\psi^2(b)=2^{n+2}b.
$$

For $n=0$, the single generator of $K^{-1}(S^3)$ is multiplied by $4$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
