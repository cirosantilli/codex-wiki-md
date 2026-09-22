# Paper 20

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_20.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_20.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
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
  - [e](#4/e)
    - [Solution](#4/e/solution)
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

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) is a [morphism of locally ringed spaces](../../../ringed-space.md#morphism-of-locally-ringed-spaces). Thus it consists of a continuous map $f:|X|\to|Y|$ and a homomorphism of [sheaves of rings](../../../ringed-space.md#sheaf-of-rings)

$$
f^\#: \mathcal O_Y\longrightarrow f_*\mathcal O_X
$$

such that, for every $x\in X$, the induced map on [stalks](../../../ringed-space.md#stalk-of-a-sheaf)

$$
f_x^\#: \mathcal O_{Y,f(x)}\longrightarrow\mathcal O_{X,x}
$$

is a [local homomorphism](../../../commutative-algebra.md#local-homomorphism-of-local-rings): it carries the maximal ideal of the source into the maximal ideal of the target. Equivalently, the inverse image of the target maximal ideal is the source maximal ideal. **The locality condition on every [stalk](../../../ringed-space.md#stalk-of-a-sheaf) distinguishes a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) from a general morphism of ringed spaces.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**The [affine-target adjunction for schemes](../../../ringed-space.md#affine-target-adjunction-for-schemes) gives the natural bijection**

$$
\boxed{\operatorname{Hom}_{\mathrm{Sch}}(X,\operatorname{Spec}A)
\simeq\operatorname{Hom}_{\mathrm{Ring}}(A,\Gamma(X,\mathcal O_X)).}
$$

A [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) $f$ gives the homomorphism on [global sections](../../../ringed-space.md#global-section) induced by $f^\#$, using $\Gamma(\operatorname{Spec}A,\mathcal O)=A$.

Conversely, let $\alpha:A\to\Gamma(X,\mathcal O_X)$ be a [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism). Choose an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) cover $U_i=\operatorname{Spec}B_i$ of $X$. Restriction of [global sections](../../../ringed-space.md#global-section) gives homomorphisms $A\to B_i$, hence [morphisms of schemes](../../../ringed-space.md#morphism-of-schemes) $f_i:U_i\to\operatorname{Spec}A$. On any [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $W\subseteq U_i\cap U_j$, both restrictions correspond to the same homomorphism $A\to\Gamma(W,\mathcal O_W)$. They therefore agree on $W$. Such affine opens cover the overlap, so the $f_i$ glue uniquely to a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) $f:X\to\operatorname{Spec}A$.

The two constructions are inverse: the first recovers $\alpha$ on each $U_i$, hence on all of $X$, and the second recovers every restriction $f|_{U_i}$ of a given $f$. This proof needs neither affineness nor [quasi-compactness](../../../topology.md#compact-space) of $X$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\mathfrak m$ be the maximal ideal of the [local ring](../../../commutative-algebra.md#local-ring) $A$. Every open subset of $\operatorname{Spec}A$ containing the [closed point](../../../topology.md#closed-point) $\mathfrak m$ is the whole [spectrum of a commutative ring](../../../ringed-space.md#spectrum-of-a-commutative-ring): it contains a [principal open subscheme](../../../ringed-space.md#principal-open-subscheme) $D(a)$ with $a\notin\mathfrak m$, and that $a$ is a [unit](../../../algebra.md#unit-in-a-ring), so $D(a)=\operatorname{Spec}A$.

Given $f:\operatorname{Spec}A\to\mathbb P^n_{\mathbb Z}$, choose a standard [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $D_+(x_i)$ containing $f(\mathfrak m)$. Its preimage is consequently all of $\operatorname{Spec}A$. The [affine-target adjunction for schemes](../../../ringed-space.md#affine-target-adjunction-for-schemes) expresses $f$ in this chart by elements $b_j\in A$ for $j\ne i$, the images of $x_j/x_i$. It is represented by [homogeneous coordinates](../../../projective-space.md#homogeneous-coordinate) with $a_i=1$ and $a_j=b_j$.

Conversely, a tuple $(a_0,\ldots,a_n)$ with some $a_i\in A^\times$ defines a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) into $D_+(x_i)$ by $x_j/x_i\mapsto a_j/a_i$. Choosing another unit entry gives the same [morphism of schemes](../../../ringed-space.md#morphism-of-schemes), since the usual [projective space](../../../projective-space.md) transition functions identify the ratios. Multiplying all entries by one [unit](../../../algebra.md#unit-in-a-ring) does not change any ratio. If two such tuples define the same [morphism of schemes](../../../ringed-space.md#morphism-of-schemes), choose a unit entry $a_i$ in the first and a unit entry $a_j'$ in the second. In the second chart, the function $x_i/x_j$ pulls back to $a_i'/a_j'$. Because the whole map lies in $D_+(x_i)$, this ratio is a [unit](../../../algebra.md#unit-in-a-ring), so $a_i'$ is a unit too. Equality in this chart gives $a_j/a_i=a_j'/a_i'$ for every $j$, hence $a_j'=(a_i'/a_i)a_j$.

**Thus the correspondence is exactly**

$$
\boxed{\operatorname{Hom}(\operatorname{Spec}A,\mathbb P^n_{\mathbb Z})
=\{(a_i):\text{some }a_i\in A^\times\}/A^\times.}
$$

This is the [projective coordinates over a local ring](../../../projective-space.md#projective-coordinates-over-a-local-ring) description.

For a general [ring](../../../commutative-algebra.md#ring), the key open-neighbourhood argument fails. Even a tuple generating the unit ideal need not have any unit entry. For example, over $A=k\times k$ the pair $((1,0),(0,1))$ defines a map to $\mathbb P^1$ whose two points have images $[1:0]$ and $[0:1]$. Neither coordinate is a unit, and no common unit multiple changes that fact. The map lies in no single standard chart. More generally, maps into [projective space](../../../projective-space.md) correspond to [invertible sheaf](../../../ringed-space.md#line-bundle) quotients of $A^{n+1}$; the quotient need not be a free rank-one module outside the [local ring](../../../commutative-algebra.md#local-ring) case.

## 2

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a point $y\in Y$ with [residue field](../../../commutative-algebra.md#residue-field) $\kappa(y)$, the [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is the [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes)

$$
\boxed{X_y=X\times_Y\operatorname{Spec}\kappa(y).}
$$

The map $\operatorname{Spec}\kappa(y)\to Y$ is the canonical point map. This [fibre product of schemes](../../../ringed-space.md#fiber-product-of-schemes) retains the [structure sheaf](../../../ringed-space.md#structure-sheaf-of-a-scheme), including any nilpotents, rather than just the set $f^{-1}(y)$. For an [affine scheme](../../../ringed-space.md#affine-scheme) map induced by $A\to B$, at $\mathfrak p\in\operatorname{Spec}A$ it is

$$
X_{\mathfrak p}=\operatorname{Spec}(B\otimes_A\kappa(\mathfrak p)).
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Compute each [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) by tensoring with the [residue field](../../../commutative-algebra.md#residue-field) of the chosen base point.

For the first map, put $L=\kappa(\mathfrak p)$ for a point $\mathfrak p$ of $\operatorname{Spec}k[T]$ and let $t$ be the image of $T$ in $L$. Then

$$
\boxed{X_{\mathfrak p}=\operatorname{Spec}L[U]/(U^2-t^2).}
$$

If the [characteristic of a field](../../../algebra.md#characteristic-of-a-field) is not two and $t\ne0$, the two factors $U-t$ and $U+t$ are coprime, so the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives $L[U]/(U^2-t^2)\simeq L\times L$: the [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is two distinct $L$-points. If $t=0$, its ring is $L[U]/(U^2)$, a [dual number](../../../commutative-algebra.md#dual-number) ring, so it is a [nonreduced double point](../../../ringed-space.md#nonreduced-double-point). In characteristic two, $U^2-t^2=(U-t)^2$ at every point, giving a [nonreduced double point](../../../ringed-space.md#nonreduced-double-point) in every [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre). This covers the [generic point](../../../algebraic-geometry.md#generic-point), where $L=k(T)$, as well as [closed points](../../../topology.md#closed-point) defined by irreducible polynomials.

For the arithmetic map, the generic [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is

$$
\boxed{\operatorname{Spec}\mathbb Q[T]/(T^2+1)=\operatorname{Spec}\mathbb Q(i).}
$$

Over a [closed point](../../../topology.md#closed-point) $(p)$ it is $\operatorname{Spec}\mathbb F_p[T]/(T^2+1)$. At $p=2$ this is $\operatorname{Spec}\mathbb F_2[\epsilon]/(\epsilon^2)$, since $T^2+1=(T+1)^2$. For odd $p$, the [finite field](../../../algebra.md#finite-field) multiplicative group is cyclic, and $-1$ is a square exactly when $p\equiv1\pmod4$. Thus

$$
\boxed{X_{(p)}\simeq
\begin{cases}
\operatorname{Spec}(\mathbb F_p\times\mathbb F_p),&p\equiv1\pmod4,\\
\operatorname{Spec}\mathbb F_{p^2},&p\equiv3\pmod4,\\
\operatorname{Spec}\mathbb F_2[\epsilon]/(\epsilon^2),&p=2.
\end{cases}}
$$

In the second case there is one degree-two [closed point](../../../topology.md#closed-point) over $\mathbb F_p$, which becomes two points after extending the [residue field](../../../commutative-algebra.md#residue-field) to an algebraic closure. The case $p=2$ remains nonreduced after such extension.

For $\operatorname{Spec}\mathbb C\to\operatorname{Spec}\mathbb Z$, the unique source point maps to the [generic point](../../../algebraic-geometry.md#generic-point) $(0)$. Since all nonzero integers are invertible in $\mathbb C$,

$$
\boxed{X_{(0)}=\operatorname{Spec}\mathbb C,\qquad X_{(p)}=\varnothing\text{ for every prime }p.}
$$

Indeed $\mathbb C\otimes_{\mathbb Z}\mathbb Q=\mathbb C$, whereas $\mathbb C\otimes_{\mathbb Z}\mathbb F_p=\mathbb C/p\mathbb C=0$. The distinction between a reduced split [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) and a [nonreduced double point](../../../ringed-space.md#nonreduced-double-point) is essential in the first two examples.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Necessity follows from commutativity of the [fibre product of schemes](../../../ringed-space.md#fiber-product-of-schemes) square: if $p(z)=x$ and $q(z)=y$, then $f(x)=g(y)$.

For sufficiency, put $s=f(x)=g(y)$ and $K=\kappa(s)$, $L=\kappa(x)$, $L'=\kappa(y)$. The maps on [local rings](../../../commutative-algebra.md#local-ring) induce field embeddings $K\hookrightarrow L,L'$. The canonical point maps into $X$ and $Y$ therefore give a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes)

$$
\operatorname{Spec}(L\otimes_KL')
=\operatorname{Spec}L\times_{\operatorname{Spec}K}\operatorname{Spec}L'
\longrightarrow X\times_SY.
$$

The [tensor product of commutative algebras](../../../module-theory.md#tensor-product-of-commutative-algebras) $L\otimes_KL'$ is nonzero. To see the hinted fact directly, choose a $K$-basis of $L$ containing $1$; tensoring that basis with $L'$ makes $1\otimes1$ nonzero. A nonzero unital [commutative ring](../../../commutative-algebra.md#commutative-ring) has a [prime ideal](../../../commutative-algebra.md#prime-ideal), so its [spectrum of a commutative ring](../../../ringed-space.md#spectrum-of-a-commutative-ring) has a point $w$. Its projections to the two field spectra are their unique points. The image $z$ of $w$ consequently projects to $x$ and $y$.

**The desired point exists precisely when the base images coincide.** This is the [point-lifting property of a scheme fibre product](../../../ringed-space.md#point-lifting-property-of-a-scheme-fibre-product). It does not claim that such a point is unique: different [prime ideals](../../../commutative-algebra.md#prime-ideal) of the tensor product may give different points over the same pair.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $f:X\to Y$ be a surjective [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) and let $Y'\to Y$ be any [morphism of schemes](../../../ringed-space.md#morphism-of-schemes). Take any point $y'\in Y'$ and let $y$ be its image in $Y$. Surjectivity supplies $x\in X$ with $f(x)=y$. By the [point-lifting property of a scheme fibre product](../../../ringed-space.md#point-lifting-property-of-a-scheme-fibre-product) proved in part (c), there is a point of $X\times_YY'$ projecting to both $x$ and $y'$. Thus every point of $Y'$ is hit by the projection.

**This proves that [surjectivity is preserved by base change](../../../ringed-space.md#surjectivity-is-preserved-by-base-change).** No restriction is imposed on the [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes). No flatness or finite-type assumption is required.

## 3

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a [smooth projective curve](../../../projective-space.md#smooth-projective-curve) $C$ of [geometric genus](../../../normalization-of-an-algebraic-curve.md#geometric-genus) $g$ and a [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$, write $\ell(D)=h^0(C,\mathcal O_C(D))$ and let $K_C$ be a [canonical divisor](../../../algebraic-geometry.md#canonical-divisor). The curve form of the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) is

$$
\boxed{\ell(D)-\ell(K_C-D)=\deg D+1-g.}
$$

Here $\deg K_C=2g-2$ and $\ell(K_C)=g$. In [line bundle](../../../ringed-space.md#line-bundle) form,

$$
h^0(C,\mathcal L)-h^0(C,\omega_C\otimes\mathcal L^{-1})=\deg\mathcal L+1-g.
$$

The usual curve convention is a smooth geometrically integral projective curve; geometric embedding tests may be checked after extending the ground field to an algebraic closure.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First use the [canonical map](../../../algebraic-geometry.md#canonical-map) to obtain the embedding. Its [canonical divisor](../../../algebraic-geometry.md#canonical-divisor) has degree six and $h^0(K_C)=4$. Over an algebraically closed ground field, every effective degree-two [divisor on an algebraic curve](../../../algebraic-geometry.md#divisor-on-an-algebraic-curve) $E$ satisfies $h^0(E)=1$: a second section would give a nonconstant rational function with poles bounded by $E$, hence a map $C\to\mathbb P^1$ of degree at most two. Degree one would make $C$ rational, and degree two would make it [hyperelliptic](../../../algebraic-geometry.md#hyperelliptic-curve), both excluded here.

The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) now gives

$$
h^0(K_C-E)=\deg(K_C-E)+1-g+h^0(E)=4+1-4+1=2.
$$

Thus the complete [linear system of divisors](../../../algebraic-geometry.md#linear-system-of-divisors) $|K_C|$ separates every pair of points and every tangent direction, including the tests $E=2p$. By the [length-two criterion for a very ample linear system](../../../algebraic-geometry.md#length-two-criterion-for-a-very-ample-linear-system), it is a [very ample linear system](../../../algebraic-geometry.md#very-ample-linear-system). Consequently the [canonical map](../../../algebraic-geometry.md#canonical-map) embeds $C$ in $\mathbb P^3$, with [degree of a projective curve](../../../algebraic-geometry.md#degree-of-a-projective-curve) six. Its image is a [nondegenerate projective variety](../../../algebraic-geometry.md#nondegenerate-projective-variety), since the four canonical sections are linearly independent.

The space of homogeneous quadrics in four variables has dimension ten, while the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives

$$
h^0(C,2K_C)=12+1-4=9.
$$

Restriction therefore has a nonzero kernel, giving a quadric $Q$ containing $C$. This quadric is irreducible: a reducible quadric is a union of two planes, or a double plane, and an integral curve lying in it would lie in a plane, contradicting nondegeneracy.

Similarly, homogeneous cubics form a twenty-dimensional space, whereas

$$
h^0(C,3K_C)=18+1-4=15.
$$

There are at least five independent cubics vanishing on $C$. The multiples of $Q$ by linear forms give only four dimensions, so choose a cubic $F$ vanishing on $C$ which is not divisible by $Q$.

The polynomials $Q,F$ are a [regular sequence](../../../commutative-algebra.md#regular-sequence), hence their intersection $D$ is a [projective complete intersection](../../../ringed-space.md#projective-complete-intersection) of pure dimension one and degree $2\cdot3=6$. It contains $C$, which already has degree six. The [unmixedness of a complete intersection](../../../ringed-space.md#unmixedness-of-a-complete-intersection) excludes embedded components. Equal degrees force $C$ to be the only irreducible component and force multiplicity one at its [generic point](../../../algebraic-geometry.md#generic-point). By [generic reducedness with no embedded components](../../../ringed-space.md#generic-reducedness-with-no-embedded-components), this makes $D$ reduced, so $D=C$ as schemes. **We have proved**

$$
\boxed{C\simeq V(Q,F)\subseteq\mathbb P^3,\qquad\deg Q=2,\quad\deg F=3.}
$$

This is a [canonical genus-four curve as a quadric-cubic intersection](../../../algebraic-geometry.md#canonical-genus-four-curve-as-a-quadric-cubic-intersection). The quadric may be smooth or a cone; the argument does not require it to be smooth. The same construction descends over the ground field when the curve is geometrically nonhyperelliptic, since the restriction maps and canonical embedding are defined there.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\mathcal L=\mathcal O_C(1)$. Its degree is five. Because the linear span of $C$ has dimension at least three, restrictions of linear forms supply at least four independent [global sections](../../../ringed-space.md#global-section), so

$$
h^0(C,\mathcal L)\geq4.
$$

If $h^1(C,\mathcal L)=0$, the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives $h^0(\mathcal L)=6-g$, and therefore $g\leq2$ immediately.

If instead $\mathcal L$ is special, the [Clifford inequality for curves](../../../algebraic-geometry.md#clifford-inequality-for-curves) gives

$$
h^0(\mathcal L)\leq1+\frac{\deg\mathcal L}{2}=\frac72,
$$

so its integer dimension is at most three, a contradiction. Here is a short proof of the required [Clifford inequality for curves](../../../algebraic-geometry.md#clifford-inequality-for-curves), so the bound need not be assumed. Put $r=h^0(\mathcal L)>0$ and $s=h^0(\omega_C\otimes\mathcal L^{-1})>0$. At a smooth geometric point, choose bases of these two section spaces with strictly increasing orders of vanishing $a_1<\cdots<a_r$ and $b_1<\cdots<b_s$. Such bases exist because each successive order-of-vanishing quotient has dimension at most one. The products of the first basis with the first element of the second basis, followed by products of the last element of the first basis with the remaining elements of the second, have orders

$$
a_1+b_1<\cdots<a_r+b_1<a_r+b_2<\cdots<a_r+b_s.
$$

They are linearly independent [global sections](../../../ringed-space.md#global-section) of $\omega_C$, proving the [product dimension bound for sections on a curve](../../../algebraic-geometry.md#product-dimension-bound-for-sections-on-a-curve). Thus $r+s-1\leq h^0(\omega_C)=g$. Combining this with [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem), $r-s=\deg\mathcal L+1-g$, gives $2r\leq\deg\mathcal L+2$, which is exactly the displayed [Clifford inequality for curves](../../../algebraic-geometry.md#clifford-inequality-for-curves).

**The special case is impossible, and hence**

$$
\boxed{g(C)\leq2.}
$$

This is the [genus bound for a nonplanar degree-five curve](../../../algebraic-geometry.md#genus-bound-for-a-nonplanar-degree-five-curve). The geometric argument can be carried out after extension to an algebraic closure, which preserves these section dimensions.

## 4

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [closed immersion](../../../ringed-space.md#closed-immersion) $i:X\to Y$ is a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) whose underlying map is a homeomorphism onto a closed subset and whose map of [structure sheaves](../../../ringed-space.md#structure-sheaf-of-a-scheme)

$$
\mathcal O_Y\longrightarrow i_*\mathcal O_X
$$

is surjective. Equivalently, $X$ is the [closed subscheme](../../../ringed-space.md#closed-subscheme) defined by a quasi-coherent [ideal sheaf of a closed subscheme](../../../ringed-space.md#ideal-sheaf-of-a-closed-subscheme) on $Y$. The affine-local characterization is particularly useful: for every [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V=\operatorname{Spec}A\subseteq Y$,

$$
\boxed{i^{-1}(V)\simeq\operatorname{Spec}(A/I)\longrightarrow\operatorname{Spec}A}
$$

for an ideal $I\subseteq A$, with the map induced by the quotient homomorphism.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Work over an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $V=\operatorname{Spec}A$ of $Z$. Since $g$ is a [closed immersion](../../../ringed-space.md#closed-immersion), its inverse image is $\operatorname{Spec}(A/I)$ for some ideal $I$. Since $f$ is a [closed immersion](../../../ringed-space.md#closed-immersion), the inverse image of this [affine scheme](../../../ringed-space.md#affine-scheme) in $X$ is $\operatorname{Spec}((A/I)/J)$ for an ideal $J\subseteq A/I$. Let $\widetilde J$ be the inverse image of $J$ in $A$. The composite on this open is induced by the surjection

$$
A\longrightarrow(A/I)/J\simeq A/\widetilde J.
$$

The affine-local characterization from part (a) therefore shows that **$g\circ f$ is a [closed immersion](../../../ringed-space.md#closed-immersion)**. In particular, closed-subscheme ideals compose by taking the inverse image of the second quotient ideal.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Over an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $\operatorname{Spec}A$ of the target, a [closed immersion](../../../ringed-space.md#closed-immersion) has the form $\operatorname{Spec}(A/I)\to\operatorname{Spec}A$. Pulling it back along an [affine scheme](../../../ringed-space.md#affine-scheme) map $\operatorname{Spec}B\to\operatorname{Spec}A$ gives

$$
\operatorname{Spec}((A/I)\otimes_AB)\simeq\operatorname{Spec}(B/IB).
$$

The identification follows directly by tensoring the quotient presentation; it does not require $B$ to be flat over $A$. Since $B\to B/IB$ is surjective, this is again a [closed immersion](../../../ringed-space.md#closed-immersion). These affine calculations cover every [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes).

**Being a [closed immersion](../../../ringed-space.md#closed-immersion) is stable under arbitrary [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes).**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) $f:X\to Y$ is a [separated morphism](../../../ringed-space.md#separated-morphism) if its [diagonal morphism](../../../ringed-space.md#diagonal-morphism)

$$
\boxed{\Delta_f:X\longrightarrow X\times_YX}
$$

is a [closed immersion](../../../ringed-space.md#closed-immersion). The [diagonal morphism](../../../ringed-space.md#diagonal-morphism) is induced by the pair of identity maps on $X$. Thus separatedness is a condition relative to the given target $Y$, not a requirement that $X$ be absolutely separated.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Since $g$ is a [separated morphism](../../../ringed-space.md#separated-morphism), the [diagonal morphism](../../../ringed-space.md#diagonal-morphism) $\Delta_g:Y\to Y\times_ZY$ is a [closed immersion](../../../ringed-space.md#closed-immersion). The square

$$
\begin{array}{ccc}
X&\xrightarrow{\Gamma_f}&X\times_ZY\\
{\scriptstyle f}\downarrow&&\downarrow{\scriptstyle(f\circ p_X,p_Y)}\\
Y&\xrightarrow{\Delta_g}&Y\times_ZY
\end{array}
$$

is cartesian. Indeed, on test schemes its pullback condition is $(f(x),y)=(t,t)$, forcing $y=t=f(x)$, and leaving exactly the choice of $x$. The [graph morphism of schemes](../../../ringed-space.md#graph-morphism-of-schemes) $\Gamma_f$ is therefore a [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes) of $\Delta_g$. Part (c) shows that **$\Gamma_f$ is a [closed immersion](../../../ringed-space.md#closed-immersion)**.

Now assume additionally that $h=g\circ f:X\to Z$ is a [closed immersion](../../../ringed-space.md#closed-immersion). The projection $p_Y:X\times_ZY\to Y$ is its [base change of a morphism of schemes](../../../ringed-space.md#base-change-of-a-morphism-of-schemes) along $g$, so is a [closed immersion](../../../ringed-space.md#closed-immersion) by part (c). Since

$$
\boxed{f=p_Y\circ\Gamma_f,}
$$

part (b) shows that **$f$ is a [closed immersion](../../../ringed-space.md#closed-immersion)**. This covers the further assumption in the final unheaded paragraph.

## 5

↑ **Parent:** [Paper 20](paper-20.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [line bundle](../../../ringed-space.md#line-bundle) $\mathcal L$ is a [globally generated line bundle](../../../ringed-space.md#globally-generated-line-bundle) when the evaluation map

$$
H^0(X,\mathcal L)\otimes_k\mathcal O_X\longrightarrow\mathcal L
$$

is surjective. Equivalently, its [global sections](../../../ringed-space.md#global-section) span each fibre of the [line bundle](../../../ringed-space.md#line-bundle); locally at every point, some section is a generator.

Choose a finite generating family $s_0,\ldots,s_n$. On the open set where $s_i$ generates $\mathcal L$, the ratios $s_j/s_i$ are regular functions, giving a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) into the standard chart $D_+(x_i)$ of [projective space](../../../projective-space.md). The ratios obey the usual transition rules on overlaps, so these chart maps glue to

$$
\boxed{\varphi:X\longrightarrow\mathbb P^n_k,\qquad x\longmapsto[s_0(x):\cdots:s_n(x)].}
$$

The tuple is computed using any local trivialization of $\mathcal L$; changing that trivialization multiplies all entries by the same invertible function. The construction has $\varphi^*\mathcal O(1)\simeq\mathcal L$ and pulls back the coordinate sections to the chosen $s_i$.

There is a finiteness qualification for an arbitrary $X$: global generation alone need not provide such a finite family. It does if $X$ is [quasi-compact](../../../topology.md#compact-space), since the open sets on which individual sections generate have a finite subcover. Without that hypothesis, take $X=\coprod_{m\geq1}\mathbb P^m_k$ and let $\mathcal L$ restrict to $\mathcal O(1)$ on each component. This [line bundle](../../../ringed-space.md#line-bundle) is globally generated, but any $N$ global sections have a common zero on a component $\mathbb P^m$ with $m\geq N$. Thus this is a [globally generated line bundle without finite generators](../../../ringed-space.md#globally-generated-line-bundle-without-finite-generators). This is [finite global generation on a quasi-compact scheme](../../../ringed-space.md#finite-global-generation-on-a-quasi-compact-scheme). The finite-family construction is automatic in the projective case asked next.

For projective nonsingular $X$, put $V=\langle s_0,\ldots,s_n\rangle$. **The [length-two criterion for a very ample linear system](../../../algebraic-geometry.md#length-two-criterion-for-a-very-ample-linear-system) says that $\varphi$ is a [closed immersion](../../../ringed-space.md#closed-immersion) precisely when, after extending to an algebraic closure, $V$ separates distinct points and tangent directions.** Equivalently, the evaluation

$$
V\longrightarrow H^0(E,\mathcal L|_E)
$$

is surjective for every length-two geometric [closed subscheme](../../../ringed-space.md#closed-subscheme) $E\subseteq X$. Two distinct points give point separation; a nonreduced length-two subscheme supported at one point gives separation of a direction in the [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space). For the complete space $V=H^0(X,\mathcal L)$, this says exactly that $\mathcal L$ is a [very ample line bundle](../../../ringed-space.md#very-ample-line-bundle). For a chosen smaller $V$, it is the chosen [linear system of divisors](../../../algebraic-geometry.md#linear-system-of-divisors) which must be a [very ample linear system](../../../algebraic-geometry.md#very-ample-linear-system); mere global generation is insufficient.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $U=\mathbb P^2\setminus C$. The [localization sequence for the divisor class group](../../../algebraic-geometry.md#localization-sequence-for-the-divisor-class-group) gives

$$
\mathbb Z[C]\longrightarrow\operatorname{Cl}(\mathbb P^2)\longrightarrow\operatorname{Cl}(U)\longrightarrow0.
$$

Every [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) of $U$ extends by closure to one of $\mathbb P^2$, and the only removed [prime Weil divisor](../../../algebraic-geometry.md#prime-weil-divisor) is $C$. Rational functions have the same function field on the two spaces, so the kernel on [divisor class groups](../../../algebraic-geometry.md#divisor-class-group) consists exactly of multiples of $[C]$.

The [divisor class group](../../../algebraic-geometry.md#divisor-class-group) of $\mathbb P^2$ is $\mathbb Z$, generated by the class $[H]$ of a line. To see the degree identification, if a plane curve $D$ has degree $e$ and homogeneous equation $F_D$, then $F_D/\ell^e$, for a line equation $\ell$, is a rational function with [principal Weil divisor](../../../algebraic-geometry.md#principal-weil-divisor) $D-eH$. Degrees of [principal Weil divisors](../../../algebraic-geometry.md#principal-weil-divisor) are zero, so $[H]$ has infinite order. In particular, $[C]=d[H]$. The localization sequence therefore yields

$$
\boxed{\operatorname{Cl}(\mathbb P^2\setminus C)\simeq\mathbb Z/d\mathbb Z.}
$$

This is the [divisor class group of a plane-curve complement](../../../algebraic-geometry.md#divisor-class-group-of-a-plane-curve-complement). It includes $d=1$, when the group is zero, and does not require the removed curve to be nonsingular.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The hyperplane sections through $P$ are spanned by the three linear forms $x_1,x_2,x_0-x_3$. Their common zero on $X$ is precisely $P$, so away from $P$ the [linear system of divisors](../../../algebraic-geometry.md#linear-system-of-divisors) is base-point-free and defines the [projection from a point on a smooth quadric](../../../projective-space.md#projection-from-a-point-on-a-smooth-quadric)

$$
\boxed{\varphi([x_0:x_1:x_2:x_3])=[x_1:x_2:x_0-x_3].}
$$

In particular, the chart-ratio construction in part (a) makes this a [morphism of schemes](../../../ringed-space.md#morphism-of-schemes) on $X\setminus\{P\}$, not merely a rational map there.

Write a target point as $[u:v:w]$. The corresponding line through $P$ consists of points

$$
[\lambda+\mu w:\mu u:\mu v:\lambda].
$$

Substituting in the quadric equation gives

$$
\mu\bigl((u-v)\lambda+uw\mu\bigr)=0.
$$

Removing $P$ means $\mu\ne0$, so set $\mu=1$. Over the [residue field](../../../commutative-algebra.md#residue-field) $K$ of the target point, its [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is consequently

$$
\boxed{\operatorname{Spec}K[\lambda]/\bigl((u-v)\lambda+uw\bigr).}
$$

If $u\ne v$, this is one reduced point, with $\lambda=-uw/(u-v)$. If $u=v$ and $uw\ne0$, it is empty: the corresponding line meets the quadric only at the removed point, with intersection multiplicity two. If $u=v$ and $uw=0$, the line lies entirely on the quadric, and the [scheme-theoretic fibre](../../../ringed-space.md#scheme-theoretic-fibre) is $\mathbb A^1_K$, the line with $P$ removed.

The last case occurs at exactly $[0:0:1]$ and $[1:1:0]$. Their lines are respectively

$$
L_1=\{x_1=x_2=0\},\qquad L_2=\{x_0=x_3,\ x_1=x_2\},
$$

the two [rulings of a smooth quadric surface](../../../projective-space.md#rulings-of-a-smooth-quadric-surface) through $P$. Thus the image consists of the complement of the line $u=v$, together with those two points. The line $u=v$ parametrizes directions in the tangent plane $x_1=x_2$ at $P$. The calculation describes the [scheme-theoretic fibres](../../../ringed-space.md#scheme-theoretic-fibre) over arbitrary target points and works in every characteristic.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

**Two successive point [blowups of a smooth algebraic surface](../../../algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) suffice.** Let $X_2\to X_1=\mathbb A^2$ be the [blowup of the affine plane at the origin](../../../algebraic-geometry.md#blowup-of-the-affine-plane-at-the-origin). In its chart $x=uy$, with coordinates $(y,u)$, the total-transform equation is

$$
x^2-y^5=y^2(u^2-y^3).
$$

Removing the exceptional factor gives the [strict transform](../../../complex-geometry.md#strict-transform)

$$
C_2:\ u^2-y^3=0.
$$

Above the original origin it has just one point, $(y,u)=(0,0)$, which is still singular. The other chart is $y=vx$, where the [strict transform](../../../complex-geometry.md#strict-transform) has equation $1-v^5x^3=0$ and does not meet the exceptional divisor $x=0$. Thus there are no other points above the origin to resolve.

Blow up the remaining point to obtain $X_3\to X_2$. In the chart $u=vy$, with coordinates $(y,v)$, the total transform of $C_2$ is

$$
u^2-y^3=y^2(v^2-y),
$$

and hence its [strict transform](../../../complex-geometry.md#strict-transform) is

$$
\boxed{C_3:\ y=v^2.}
$$

The derivative of $v^2-y$ with respect to $y$ is $-1$, so this is nonsingular, even in characteristics two or five. In the other chart $y=wu$, the [strict transform](../../../complex-geometry.md#strict-transform) has equation $1-w^3u=0$ and does not meet the exceptional divisor $u=0$. Therefore the only point of $C_3$ mapping to the original origin is the smooth point $(y,v)=(0,0)$.

The required sequence is

$$
\boxed{X_3=\operatorname{Bl}_{(0,0)}X_2\longrightarrow X_2=\operatorname{Bl}_0\mathbb A^2\longrightarrow X_1=\mathbb A^2.}
$$

The local parameter $v$ there gives $y=v^2$ and $x=v^5$, also verifying the resolved branch directly. This is the [resolution of the (2,5) cusp by two blowups](../../../algebraic-geometry.md#resolution-of-the-2-5-cusp-by-two-blowups). Its tangency to an exceptional divisor does not affect the requested nonsingularity of the [strict transform](../../../complex-geometry.md#strict-transform); making the whole total transform have normal crossings is a stronger task.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
