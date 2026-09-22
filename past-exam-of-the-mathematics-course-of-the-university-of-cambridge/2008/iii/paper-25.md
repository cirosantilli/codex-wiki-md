# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper25.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $A=E\times\{p\}$, $B=\{p\}\times E$ and $D=\Delta_E$. Their [self-intersection numbers](../../../algebraic-geometry.md#self-intersection-number) vanish: each factor curve has trivial [normal bundle](../../../algebraic-geometry.md#normal-bundle), and the [self-intersection of the diagonal of a curve](../../../algebraic-geometry.md#self-intersection-of-the-diagonal-of-a-curve) is $2-2g(E)=0$. Each pair meets transversely once. Their [intersection pairing](../../../homology.md#intersection-pairing) is therefore

$$
\begin{pmatrix}A^2&A\cdot B&A\cdot D\\B\cdot A&B^2&B\cdot D\\D\cdot A&D\cdot B&D^2\end{pmatrix}
=\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix},\qquad\det=2.
$$

If a rational [linear combination](../../../vector-space.md#linear-combination) of their [cycle classes](../../../algebraic-geometry.md#cycle-class) vanished in $H^2(E\times E,\mathbb Q)$, intersecting it with $A,B,D$ would multiply its coefficients by this invertible matrix and give zero. All coefficients must vanish, proving **the three classes are [linearly independent](../../../vector-space.md#linear-independence)**.

The [cycle class map](../../../algebraic-geometry.md#cycle-class-map) detects the [Chow Künneth failure for an elliptic self-product](../../../algebraic-geometry.md#chow-kunneth-failure-for-an-elliptic-self-product). The codimension-one image of the [external product of Chow classes](../../../algebraic-geometry.md#external-product-of-chow-classes) consists of sums from $\operatorname{CH}^1(E)\otimes\operatorname{CH}^0(E)$ and $\operatorname{CH}^0(E)\otimes\operatorname{CH}^1(E)$. Here $\operatorname{CH}^0(E)=\mathbb Z[E]$, and every divisor's [cohomology class](../../../cohomology.md#cohomology-class) is its [degree of a divisor](../../../algebraic-geometry.md#degree-of-a-divisor) times the class of a point. Thus the image's cohomology is contained in the span of $[A],[B]$. The diagonal's independent class lies outside that span, so its [Chow class](../../../algebraic-geometry.md#chow-class) lies outside the external-product image. Therefore **the natural map of Chow groups is not surjective**.

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Embed $Y$ in [projective space](../../../projective-space.md) and let $H$ be its hyperplane [Cartier divisor](../../../cartier-divisor.md). Since $f$ is surjective between integral surfaces, it is [generically finite](../../../algebraic-geometry.md#generically-finite-morphism), with degree $r>0$. Its [pullback of a Cartier divisor](../../../cartier-divisor.md#pullback-of-a-cartier-divisor) $L=f^*H$ is a [nef divisor](../../../cartier-divisor.md#nef-line-bundle), and the [projection formula for algebraic cycles](../../../algebraic-geometry.md#projection-formula-for-algebraic-cycles) gives $L^2=rH^2>0$. The same formula gives $L\cdot C=H\cdot f_*C=0$, because the curve is contracted to a point.

The [Hodge index theorem for algebraic surfaces](../../../algebraic-geometry.md#hodge-index-theorem-for-algebraic-surfaces) makes the [intersection pairing on the Picard group of a surface](../../../algebraic-geometry.md#intersection-pairing-on-the-picard-group-of-a-surface) have signature $(1,\rho-1)$ on $N^1(X)_{\mathbb R}$. The orthogonal complement of any positive-square vector, including $L$, is [negative definite](../../../linear-algebra.md#negative-definite-matrix). The numerical class of $C$ is nonzero, since an [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) on $X$ intersects every nonzero [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) positively. Thus the [contracted curve has negative self-intersection](../../../algebraic-geometry.md#contracted-curve-has-negative-self-intersection) conclusion applies:

$$
\boxed{C^2<0.}
$$

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $D$ be an [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) [linearly equivalent](../../../algebraic-geometry.md#linear-equivalence-of-weil-divisors) to $C$. If $C$ were not a component of $D$, all [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity) between its components and $C$ would be nonnegative, contradicting $D\cdot C=C^2<0$. Hence $D=C+D'$ with $D'$ effective and [linearly equivalent](../../../algebraic-geometry.md#linear-equivalence-of-weil-divisors) to zero. For an [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) $H$, this gives $H\cdot D'=0$. Positivity of $H$ on every irreducible component of a nonzero effective divisor forces $D'=0$. Therefore $\boxed{D=C}$, illustrating the [rigidity of a negative curve](../../../algebraic-geometry.md#rigidity-of-a-negative-curve).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use [countability of negative curves](../../../algebraic-geometry.md#countability-of-negative-curves). A [smooth projective surface](../../../algebraic-geometry.md#smooth-projective-surface) over $\mathbb C$ is a [compact](../../../topology.md#compact-space) [smooth manifold](../../../differential-geometry.md#smooth-manifold) homotopy equivalent to a [finite CW complex](../../../algebraic-topology.md#finite-cw-complex), so its integral [cohomology group](../../../cohomology.md#cohomology-group) $H^2(X,\mathbb Z)$ is finitely generated and therefore countable. Distinct irreducible curves $C,D$ with $C^2<0$ cannot have the same [cohomology class](../../../cohomology.md#cohomology-class): that would give $C\cdot D=C^2<0$, while distinct effective curves have nonnegative [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity). Assigning a [negative curve](../../../algebraic-geometry.md#negative-curve-on-a-projective-surface) its [cohomology class](../../../cohomology.md#cohomology-class) is thus [injective](../../../algebra.md#injective-function), proving **there are at most countably many negative curves**.

For zero [self-intersection](../../../algebraic-geometry.md#self-intersection-number), uncountable families do occur. On the product of two [projective lines](../../../finite-group-theory.md#projective-line) $\mathbb P^1\times\mathbb P^1$, every fiber $\mathbb P^1\times\{p\}$ has [self-intersection](../../../algebraic-geometry.md#self-intersection-number) zero, since a different fiber is disjoint and has the same [numerical equivalence of divisors](../../../cartier-divisor.md#numerical-equivalence-of-divisors) class. The parameter $p\in\mathbb P^1(\mathbb C)$ varies over an uncountable set. Thus **yes, there can be uncountably many such curves**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $X\subset\mathbb P^3$ have degree $d\geq3$ and hyperplane class $H$. The [adjunction formula](../../../complex-geometry.md#adjunction-formula) gives $K_X=(d-4)H$. For a line $L\subset X$, the same formula on the [smooth rational curve](../../../projective-space.md#smooth-rational-curve) $L$ yields $(K_X+L)\cdot L=-2$, hence

$$
\boxed{L^2=2-d<0.}
$$

Thus all lines are [negative curves](../../../algebraic-geometry.md#negative-curve-on-a-projective-surface), and part (b) makes their set countable. The [Fano scheme of lines](../../../algebraic-geometry.md#fano-scheme-of-lines) is a closed [projective scheme](../../../ringed-space.md#projective-scheme) of $\operatorname{Gr}(2,4)$. A positive-dimensional complex algebraic component would have uncountably many points, so this scheme is zero-dimensional. A [projective scheme](../../../ringed-space.md#projective-scheme) of [finite type](../../../ringed-space.md#morphism-of-finite-type) has only finitely many zero-dimensional points. This proves the [finiteness of lines on a smooth surface of degree at least three](../../../algebraic-geometry.md#finiteness-of-lines-on-a-smooth-surface-of-degree-at-least-three).

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose a [projective embedding](../../../projective-space.md#projective-embedding) of the [abelian surface](../../../algebraic-geometry.md#abelian-surface) $X$. By [Bertini's theorem](../../../cartier-divisor.md#bertini-s-theorem), a general [hyperplane section](../../../cartier-divisor.md#hyperplane-section) $C$ is a [smooth projective curve](../../../projective-space.md#smooth-projective-curve) that is [connected](../../../geometry-and-topology.md#connected-space). It is [ample](../../../ringed-space.md#ample-line-bundle), so $C^2>0$. Choose $p\in C$ and translate the inclusion so it sends $p$ to the identity of $X$. The [universal property of the Jacobian variety](../../../abelian-variety.md#universal-property-of-the-jacobian-variety) then gives a homomorphism of [abelian varieties](../../../abelian-variety.md)

$$
\Phi:J(C)\longrightarrow X
$$

whose composition with the based [Abel map of an algebraic curve](../../../abelian-variety.md#abel-map-of-an-algebraic-curve) is this translated inclusion.

The image is a closed connected algebraic subgroup, since $J(C)$ is projective, and it contains a translate of $C$. If the image had dimension one, that irreducible curve would be the image subgroup itself. A distinct coset is disjoint from it and has the same numerical divisor class: translation acts trivially on cohomology, being homotopic to the identity on the [complex torus](../../../complex-geometry.md#complex-torus). Its [self-intersection](../../../algebraic-geometry.md#self-intersection-number) would therefore be zero, contradicting $C^2>0$. The image has dimension two and is all of $X$. Thus **$\Phi$ is surjective**, as expressed by the principle that an [ample curve on an abelian surface generates the surface](../../../algebraic-geometry.md#ample-curve-on-an-abelian-surface-generates-the-surface).

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The divisors have no common irreducible component, since a common curve would give infinitely many intersection points. The [Bézout theorem](../../../algebraic-geometry.md#bezout-s-theorem) therefore gives total [intersection multiplicity](../../../algebraic-geometry.md#intersection-multiplicity) $\deg C\deg D=3\cdot3=9$. As all intersection is supported at $p$,

$$
\boxed{I_p(C,D)=9.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take $D=\{y^2z=x^3\}$, $L=\{z=0\}$ and $C=3L$. This projective [cuspidal cubic](../../../algebraic-geometry.md#cuspidal-cubic) is irreducible and meets $L$ only at $p=[0:1:0]$. At $p$, the derivative with respect to $z$ is $y^2=1$, so $D$ is smooth. In the affine chart $y=1$, it is $z=x^3$, and $L$ is $z=0$, so $I_p(L,D)=3$. Multiplicity is linear in the divisor $C=3L$, giving

$$
\boxed{I_p(C,D)=3\,I_p(L,D)=9.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Apply a [projective transformation](../../../projective-space.md#projective-linear-transformation) to put the [cuspidal cubic](../../../algebraic-geometry.md#cuspidal-cubic) in the form $D=\{F=y^2z-x^3=0\}$. Since $L$ meets $D$ at only one smooth point $p$, the [Bézout theorem](../../../algebraic-geometry.md#bezout-s-theorem) forces intersection multiplicity three there. Hence $L$ is the [tangent line](../../../calculus.md#tangent-line) at a [flex](../../../algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve).

The homogeneous [Hessian matrix](../../../calculus.md#hessian-matrix) has determinant

$$
\det\begin{pmatrix}-6x&0&0\\0&2z&2y\\0&2y&0\end{pmatrix}=24xy^2.
$$

By the [Hessian criterion for a flex](../../../algebraic-geometry.md#hessian-criterion-for-a-flex), every smooth flex lies in $D\cap\{xy^2=0\}$. These intersections are $[0:0:1]$, the [cusp](../../../algebraic-geometry.md#cusp-algebraic-geometry), and $[0:1:0]$, which is smooth. Thus the [unique smooth flex of a cuspidal cubic](../../../algebraic-geometry.md#unique-smooth-flex-of-a-cuspidal-cubic) is $p=[0:1:0]$, with [tangent line](../../../calculus.md#tangent-line) $L=\{z=0\}$. Conversely the pair in part (b) has exactly the required properties. Therefore **there is one projective-equivalence class**, represented by

$$
\boxed{(C,D)=\bigl(3\{z=0\},\ \{y^2z=x^3\}\bigr).}
$$

<a id="5/c/image-cuspidal-cubic-in-two-projective-charts-the-cusp-and-its-unique-smooth-flex"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-25-cusp-and-flex.png)

**[Figure 1](#5/c/image-cuspidal-cubic-in-two-projective-charts-the-cusp-and-its-unique-smooth-flex). Cuspidal cubic in two projective charts: the cusp and its unique smooth flex**.

## 6

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [adjunction formula](../../../complex-geometry.md#adjunction-formula) on the degree-$d$ [projective hypersurface](../../../algebraic-geometry.md#projective-hypersurface) gives $K_X=(d-4)H$. Since $C$ is a [smooth rational curve](../../../projective-space.md#smooth-rational-curve), adjunction on $C$ gives $(K_X+C)\cdot C=2g(C)-2=-2$. Its degree is $H\cdot C=a$, so the [smooth rational-curve self-intersection on a projective hypersurface](../../../complex-geometry.md#smooth-rational-curve-self-intersection-on-a-projective-hypersurface) formula is

$$
\boxed{C^2=-2-(d-4)a.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [Noether–Lefschetz theorem](../../../algebraic-geometry.md#noether-lefschetz-theorem) says that a [very general](../../../algebraic-geometry.md#very-general-point-of-an-algebraic-parameter-space) smooth degree-$d$ surface in $\mathbb P^3_{\mathbb C}$, for $d\geq4$, has [Picard group](../../../ringed-space.md#picard-group) freely generated by its hyperplane class $H$. Here very general means outside a countable union of proper closed loci in the parameter space of surfaces.

If such a surface contained a [smooth rational curve](../../../projective-space.md#smooth-rational-curve) $C$, its divisor class would be $mH$ for an integer $m$. Since $H\cdot C=md>0$, one has $m>0$ and therefore $C^2=m^2d>0$. Part (a), however, gives $C^2=-2-(d-4)\deg C\leq-2$, a contradiction. Thus **a [very general surface of degree at least four has no smooth rational curve](../../../algebraic-geometry.md#very-general-surface-of-degree-at-least-four-has-no-smooth-rational-curve)**. The statement concerns smooth embedded curves; a singular curve can still have rational normalization.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
