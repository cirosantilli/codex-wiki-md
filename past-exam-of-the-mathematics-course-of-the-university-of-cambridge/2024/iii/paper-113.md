# Paper 113

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_113.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_113.pdf)

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

## 1

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A morphism $f:X\to S$ is a [separated morphism](../../../ringed-space.md#separated-morphism) when its [diagonal morphism](../../../ringed-space.md#diagonal-morphism)

$$
\Delta_{X/S}:X\longrightarrow X\times_SX
$$

is a [closed immersion](../../../ringed-space.md#closed-immersion).

For the requested example, take the [affine plane with doubled origin](../../../ringed-space.md#affine-plane-with-doubled-origin): glue two copies $U,V\cong\mathbb A_k^2$ by the identity on

$$
U\cap V\cong\mathbb A_k^2\setminus\{0\}.
$$

The opens $U$ and $V$ are affine, while their intersection is the [punctured affine plane](../../../ringed-space.md#punctured-affine-plane), which is not affine. Indeed, its regular functions are still $k[x,y]$; if it were affine, the canonical map to $\operatorname{Spec}k[x,y]=\mathbb A_k^2$ would be an isomorphism, contrary to the missing origin. The resulting scheme is not separated: in a separated scheme, the intersection of two affine opens is the inverse image of the closed diagonal inside their affine product and is therefore affine.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On the standard charts $D_+(x)$ and $D_+(y)$ of $\mathbb P_k^1$, a section of the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) $\mathcal O(d)$ is represented by a degree-zero element of the corresponding localization of $k[x,y](d)$. A global section is therefore a homogeneous polynomial of degree $d$ when $d\geq0$. There are no nonzero global sections for $d<0$. Hence

$$
\boxed{\dim_kH^0(\mathbb P_k^1,\mathcal O(d))=
\begin{cases}
d+1,&d\geq0,\\
0,&d<0.
\end{cases}}
$$

Local isomorphism on every member of a fixed affine cover does not imply a global isomorphism: the local identifications may have different transition functions. For example, $\mathcal O$ and $\mathcal O(1)$ are both trivial on the two standard affine charts of $\mathbb P^1$, but they are not isomorphic because their spaces of global sections have dimensions one and two.

An injective map between [line bundles](../../../ringed-space.md#line-bundle) need not be an isomorphism. Multiplication by a nonzero section gives

$$
\mathcal O(-1)\hookrightarrow\mathcal O
$$

on $\mathbb P^1$; its cokernel is a nonzero [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) supported at the zero of the section.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $n\geq2$, the omitted point has codimension at least two in the normal integral scheme $\mathbb P_k^n$. Regular functions extend across such a subset, so

$$
\Gamma(X,\mathcal O_X)=\Gamma(\mathbb P_k^n,\mathcal O)=k.
$$

Thus

$$
\boxed{\pi_*\mathcal O_X\cong\widetilde{k}}
$$

on $\operatorname{Spec}k$, and it is a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) because it corresponds to the one-dimensional $k$-vector space $k$.

The complement of a rational point in $\mathbb P_k^1$ is $\mathbb A_k^1$. Its regular functions are $k[t]$, which is infinite-dimensional over $k$. Its pushforward to $\operatorname{Spec}k$ is therefore quasi-coherent but not coherent.

For an example on $X$, choose a projective line $L\subset\mathbb P_k^n$ through $p$. Then

$$
C=L\setminus\{p\}\cong\mathbb A_k^1
$$

is closed in $X$. For the closed immersion $i:C\hookrightarrow X$, the sheaf $\mathcal F=i_*\mathcal O_C$ is coherent, but

$$
\Gamma(X,\mathcal F)=\Gamma(C,\mathcal O_C)=k[t].
$$

**Consequently $\pi_*\mathcal F$ is not coherent on $\operatorname{Spec}k$.**

## 2

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [fibre product of schemes](../../../ringed-space.md#fiber-product-of-schemes) $X\times_SY$ comes with projections to $X$ and $Y$ having equal composites to $S$, and is universal with this property. A morphism is [universally closed](../../../ringed-space.md#universally-closed-morphism) when every base change is closed on underlying topological spaces.

The structural morphism $\mathbb A_k^1\to\operatorname{Spec}k$ is closed because its target has one point, but it is not universally closed. After base change by $\mathbb A_k^1$, it becomes the projection $\mathbb A_k^2\to\mathbb A_k^1$; the closed hyperbola $V(xy-1)$ has image $D(x)$, which is not closed.

For a finite-type universally closed nonseparated example, glue two copies of $\mathbb P_k^1$ along the complement of one rational point, producing a projective line with a doubled point. It is of finite type. After every base change, each of its two projective-line charts maps closedly to the base, so the image of any closed subset, being the union of the two closed images, is closed. Thus the structural morphism is universally closed. It is not separated because the two doubled points violate uniqueness in the [valuative criterion for separatedness](../../../ringed-space.md#valuative-criterion-for-separatedness), or equivalently because its diagonal is not closed.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix $x\in X$ and choose affine opens $x\in U\subseteq X$ and $f(x)\in W\subseteq S$ with $f(U)\subseteq W$. The open subset $U\times_WU$ of $X\times_SX$ contains $\Delta(x)$. If $U=\operatorname{Spec}A$ and $W=\operatorname{Spec}R$, its diagonal is induced by the surjection

$$
A\otimes_RA\longrightarrow A,
\qquad a\otimes b\longmapsto ab,
$$

so it is a closed immersion. Hence every [diagonal morphism](../../../ringed-space.md#diagonal-morphism) is locally a closed immersion into an open subset, and therefore is a [locally closed immersion](../../../ringed-space.md#locally-closed-immersion).

For $\mathbb A_k^1$, the product is $\mathbb A_k^2=\operatorname{Spec}k[x,y]$ and the diagonal is $V(x-y)$. Its complement is the principal affine open

$$
\boxed{D(x-y)=\operatorname{Spec}k[x,y,(x-y)^{-1}].}
$$

Take instead the separated scheme $X=\mathbb A_k^2$. The complement of its diagonal in $X\times_kX\cong\mathbb A_k^4$ is $\mathbb A_k^4\setminus\mathbb A_k^2$, where the removed diagonal has codimension two. Its global functions still form the polynomial ring of $\mathbb A_k^4$. Were the complement affine, its canonical morphism to $\operatorname{Spec}$ of this ring would identify it with all of $\mathbb A_k^4$, which is impossible. Thus this diagonal complement is not affine.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For a Noetherian separated integral scheme regular in codimension one, a [Weil divisor](../../../algebraic-geometry.md#weil-divisor) is a finite integer combination of integral codimension-one closed subschemes. Principal divisors are the valuation divisors of nonzero rational functions, and the [divisor class group](../../../algebraic-geometry.md#divisor-class-group) is

$$
\operatorname{Cl}(X)=\operatorname{Div}(X)/\operatorname{Prin}(X).
$$

For an open immersion $U\subseteq X$, restriction induces a surjection

$$
\operatorname{Cl}(X)\twoheadrightarrow\operatorname{Cl}(U):
$$

every prime divisor of $U$ closes to a prime divisor of $X$, while divisors supported in $X\setminus U$ form the kernel. Therefore $\operatorname{Cl}(X)=0$ implies $\operatorname{Cl}(U)=0$.

Affine schemes need not have trivial class group. For example,

$$
X=\operatorname{Spec}k[x,y,z]/(xy-z^2)
$$

is a normal affine surface with $\operatorname{Cl}(X)\cong\mathbb Z/2\mathbb Z$. The height-one prime $(x,z)$ represents the nonzero class: twice this divisor is the principal divisor of $x$, but the divisor itself is not principal.

## 3

↑ **Parent:** [Paper 113](paper-113.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A sheaf $\mathcal F$ of $\mathcal O_X$-modules is [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf) when every affine open $U=\operatorname{Spec}A$ has $\mathcal F|_U\cong\widetilde M$ for some $A$-module $M$.

Cover the target $\mathbb P_k^1$ by $D_+(y_0)$ and $D_+(y_1)$. On the first chart put $s=y_1/y_0$; its inverse image is $D_+(x_0)$ with coordinate $t=x_1/x_0$, and the morphism on rings is

$$
k[s]\longrightarrow k[t],
\qquad s\longmapsto t^2.
$$

As a $k[s]$-module,

$$
k[t]=k[t^2]\oplus t,k[t^2]
$$

is free of rank two. The same calculation on the other standard chart uses $s^{-1}\mapsto t^{-2}$. Hence $f_*\mathcal O_X$ is locally free of rank two on the target.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The complement $Y$ is covered by the $m$ principal affine opens $D(f_1),\ldots,D(f_m)$. Every finite intersection is again a principal affine open, so this is an acyclic cover for $\mathcal O_Y$. Its [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) has no degree-$m$ term because there is no intersection of $m+1$ distinct cover members. Therefore

$$
\boxed{H^m(Y,\mathcal O_Y)=0.}
$$

Translate $p$ to the origin. The complement $\mathbb A_k^3\setminus\{0\}$ has the affine cover $D(x),D(y),D(z)$, and its second Čech cohomology is

$$
\frac{k[x^{\pm1},y^{\pm1},z^{\pm1}]}
{k[x^{\pm1},y^{\pm1},z]+k[x^{\pm1},y,z^{\pm1}]+k[x,y^{\pm1},z^{\pm1}]}.
$$

The class of $x^{-1}y^{-1}z^{-1}$ is nonzero, so $H^2(\mathbb A_k^3\setminus\{p\},\mathcal O)\ne0$. On the other hand, $\mathbb A_k^3\setminus\ell=D(x)\cup D(y)$, and the first part with $m=2$ gives $H^2(\mathbb A_k^3\setminus\ell,\mathcal O)=0$. Since [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) is invariant under scheme isomorphism, the two complements are not isomorphic.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Two nonisomorphic [punctual schemes](../../../ringed-space.md#punctual-scheme) are

$$
\operatorname{Spec}k
\qquad\text{and}\qquad
\operatorname{Spec}k[\varepsilon]/(\varepsilon^2).
$$

Their underlying spaces each have one point, but the second has a nonzero [nilpotent element](../../../commutative-algebra.md#nilpotent) and the first is reduced.

After translating their common support to the origin, punctual closed subschemes of $\mathbb A_k^1$ correspond to ideals of $k[t]$ whose radical is $(t)$. Since $k[t]$ is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), each such ideal is $(t^r)$ for a unique $r\geq1$. Its coordinate ring has basis $1,t,\ldots,t^{r-1}$ and hence dimension $r$. Equal dimensions force equal exponents, so $Z$ and $Z'$ are in fact the same closed subscheme after the common coordinate choice, and in particular are isomorphic.

In $\mathbb A_k^2$, the ideals

$$
I=(x,y^2),
\qquad
I'=(x^2,y)
$$

define distinct punctual closed subschemes supported at the origin. Both quotient rings have dimension two over $k$, with bases $1,y$ and $1,x$ respectively. Thus they have equal-dimensional global-section spaces despite being distinct embedded closed subschemes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
