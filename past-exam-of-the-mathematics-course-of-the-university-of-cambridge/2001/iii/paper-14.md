# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper14.pdf)

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
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) $F,G$ defining the two [projective plane curves](../../../algebraic-geometry.md#projective-plane-curve). Their absence of a common [irreducible component](../../../algebraic-geometry.md#irreducible-component) makes them coprime. For a point $O=[1:0:0]$ outside both [curves](../../../topology.md#curve), they have degrees $n,m$ in $X$ and nonzero constant leading coefficients. The [resultant](../../../polynomial.md#resultant)

$$
R(Y,Z)=\operatorname{Res}_X(F(X,Y,Z),G(X,Y,Z))
$$

is therefore nonzero. Indeed, a vanishing [resultant](../../../polynomial.md#resultant) over $k(Y,Z)$ would give a common factor there, and [Gauss's lemma](../../../riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) would give a common component of the original [curves](../../../topology.md#curve).

The [homogeneity](../../../real-analysis.md#homogeneity) of $F,G$ makes $R$ a [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) of degree $nm$: scaling $(Y,Z)$ by $a$ scales their $X$-roots by $a$, and the product of the $nm$ differences of roots scales by $a^{nm}$. Every point in the [intersection](../../../set.md#set-intersection) projects from $O$ to a zero of $R$ in the [projective line](../../../finite-group-theory.md#projective-line). Each such projection line contains only finitely many points of either [curve](../../../topology.md#curve), since it passes through $O$ outside them. Thus the [intersection](../../../set.md#set-intersection) is finite already.

We may now choose $O$ also outside the finitely many joining lines of distinct intersection points. Projection is then injective on the [intersection](../../../set.md#set-intersection). A nonzero degree-$nm$ [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) on the [projective line](../../../finite-group-theory.md#projective-line) has at most $nm$ distinct zeros, so the [resultant bound for intersections of plane curves](../../../algebraic-geometry.md#resultant-bound-for-intersections-of-plane-curves) gives

$$
\boxed{|C\cap D|\le nm.}
$$

This derives the required cardinality bound without assuming the full intersection-multiplicity statement of [Bézout's theorem](../../../algebraic-geometry.md#bezout-s-theorem).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Blow up the distinct singular points of the [integral projective curve](../../../algebraic-geometry.md#integral-projective-curve), once at each original point, and let $C'$ be its [strict transform of an algebraic subvariety](../../../algebraic-geometry.md#strict-transform-of-an-algebraic-subvariety). Write $H$ for the pullback of a [projective line](../../../finite-group-theory.md#projective-line) and $E_i$ for the [algebraic exceptional divisors](../../../algebraic-geometry.md#algebraic-exceptional-divisor). The [multiplicity of a plane curve at a point](../../../algebraic-geometry.md#multiplicity-of-a-plane-curve-at-a-point) and the [intersection formula for blowing up a surface](../../../algebraic-geometry.md#intersection-formula-for-blowing-up-a-surface) give

$$
[C']=dH-\sum_i m_iE_i,\qquad
H^2=1,\qquad H\cdot E_i=0,\qquad E_i\cdot E_j=-\delta_{ij}.
$$

The [canonical divisor formula for a surface blowup](../../../algebraic-geometry.md#canonical-divisor-formula-for-a-surface-blowup) gives $K=-3H+\sum_iE_i$. Applying the [arithmetic adjunction formula on a smooth surface](../../../algebraic-geometry.md#arithmetic-adjunction-formula-on-a-smooth-surface), rather than a formula requiring a smooth strict transform, yields

$$
2p_a(C')-2=d^2-3d-\sum_i m_i(m_i-1),
$$

and hence

$$
p_a(C')=\frac{(d-1)(d-2)}2-\frac12\sum_i m_i(m_i-1).
$$

The [strict transform of an algebraic subvariety](../../../algebraic-geometry.md#strict-transform-of-an-algebraic-subvariety) is still an [integral projective curve](../../../algebraic-geometry.md#integral-projective-curve). Its [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) is $h^1(C',\mathcal O_{C'})\ge0$, even if some singularities remain. Therefore the [plane curve singularity multiplicity bound](../../../algebraic-geometry.md#plane-curve-singularity-multiplicity-bound) is

$$
\boxed{\sum_i m_i(m_i-1)\le(d-1)(d-2).}
$$

The argument uses only one [blowup of a smooth algebraic surface](../../../algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) at each original singular point; it does not assume these blowups resolve every singularity.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [genus-degree formula](../../../algebraic-geometry.md#genus-degree-formula) gives [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) three for a [plane quartic](../../../algebraic-geometry.md#plane-quartic). Each of its three double points has [multiplicity of a plane curve at a point](../../../algebraic-geometry.md#multiplicity-of-a-plane-curve-at-a-point) two, so the [arithmetic genus drop under a point blowup](../../../algebraic-geometry.md#arithmetic-genus-drop-under-a-point-blowup) is one at each point. The resulting [integral projective curve](../../../algebraic-geometry.md#integral-projective-curve) $C'$ has

$$
p_a(C')=3-3=0.
$$

For its finite [normalization of an algebraic curve](../../../normalization-of-an-algebraic-curve.md) $\nu:\widetilde C\to C'$, the [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) identity is

$$
p_a(C')=g(\widetilde C)+\operatorname{length}(\nu_*\mathcal O_{\widetilde C}/\mathcal O_{C'}).
$$

Both terms are nonnegative, so $g(\widetilde C)=0$. Over the [algebraically closed field](../../../algebra.md#algebraically-closed-field), the [rationality of a smooth projective genus-zero curve](../../../projective-space.md#rationality-of-a-smooth-projective-genus-zero-curve) identifies $\widetilde C$ with the [projective line](../../../finite-group-theory.md#projective-line): a point $P$ exists, and [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) gives a degree-one map from the two-dimensional space $L(P)$. Consequently $C$ is [birational](../../../algebraic-geometry.md#birational-variety) to $\mathbb P^1$. This proves the [rationality of a plane quartic with three double points](../../../algebraic-geometry.md#rationality-of-a-plane-quartic-with-three-double-points) even when a double point is not an ordinary node.

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $F$ define the [nonsingular plane cubic](../../../algebraic-geometry.md#nonsingular-plane-cubic) and let $H_F=\det\operatorname{Hess}F$ be its [Hessian curve of a plane cubic](../../../algebraic-geometry.md#hessian-curve-of-a-plane-cubic) equation. The [Hessian criterion for a flex](../../../algebraic-geometry.md#hessian-criterion-for-a-flex) applies in the allowed [field characteristic](../../../algebra.md#characteristic-of-a-field). Here is the local calculation, so no characteristic-zero argument is needed.

Move any point $P$ to $[0:1:0]$ and its [tangent line](../../../calculus.md#tangent-line) to $Z=0$. Smoothness gives a nonzero coefficient $g$ of $Y^2Z$, while the coefficients of $Y^3$ and $XY^2$ vanish. Thus

$$
F(X,Y,0)=aX^3+bX^2Y,\qquad
\operatorname{Hess}F(P)=
\begin{pmatrix}2b&0&f\\0&0&2g\\f&2g&2i\end{pmatrix},
\qquad H_F(P)=-8bg^2.
$$

The [intersection multiplicity](../../../algebraic-geometry.md#intersection-multiplicity) with the [tangent line](../../../calculus.md#tangent-line) is at least three precisely when $b=0$, which is precisely $H_F(P)=0$ because the [field characteristic](../../../algebra.md#characteristic-of-a-field) is not two. The tangent cannot be a component of a [nonsingular plane cubic](../../../algebraic-geometry.md#nonsingular-plane-cubic).

If $H_F$ vanishes identically, every point is a [flex](../../../algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve) by this calculation. Otherwise it is a degree-three [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial). Its zero locus meets the cubic by [Bézout's theorem](../../../algebraic-geometry.md#bezout-s-theorem); if they share a component, that also supplies a point of intersection. Every such point is smooth and satisfies the criterion, so a [flex](../../../algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve) exists.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose a [flex](../../../algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve) as $O=[0:1:0]$, with [tangent line](../../../calculus.md#tangent-line) $Z=0$. The [flex coordinates for a smooth plane cubic](../../../algebraic-geometry.md#flex-coordinates-for-a-smooth-plane-cubic) give

$$
F=aX^3+bY^2Z+cXYZ+dX^2Z+eYZ^2+fXZ^2+gZ^3,
\qquad ab\ne0.
$$

The coefficient $a$ is nonzero because $Z=0$ is not a component, and $b\ne0$ expresses smoothness at $O$. Since the [field characteristic](../../../algebra.md#characteristic-of-a-field) is not two, the projective linear change

$$
Y'=Y+\frac{cX+eZ}{2b}
$$

completes the square. The equation becomes $Y'^2Z=P_3(X,Z)$ after dividing by a nonzero constant, where $P_3$ is a degree-three [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) with nonzero $X^3$ coefficient.

On $Z=1$, the [polynomial](../../../polynomial.md) $P_3(x,1)$ has three distinct roots $r_1,r_2,r_3$ in the [algebraically closed field](../../../algebra.md#algebraically-closed-field). A repeated root $r$ would make $(r,0)$ a [singular point](../../../algebraic-geometry.md#singular-point-of-an-algebraic-variety) of $y'^2=P_3(x,1)$, since both first partial derivatives vanish there. Put

$$
x'=\frac{x-r_1}{r_2-r_1},\qquad
\lambda=\frac{r_3-r_1}{r_2-r_1}.
$$

A further nonzero scaling of $y'$ absorbs the leading coefficient and $(r_2-r_1)^3$; the required square root exists in the [algebraically closed field](../../../algebra.md#algebraically-closed-field). These are projective linear changes of the original coordinates. Renaming the new coordinates gives the [Legendre form of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#legendre-form-of-an-elliptic-curve)

$$
\boxed{y^2=x(x-1)(x-\lambda),\qquad\lambda\notin\{0,1\}.}
$$

Its projective completion is $Y^2Z=X(X-Z)(X-\lambda Z)$, with the chosen [flex](../../../algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve) at infinity.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [genus-degree formula](../../../algebraic-geometry.md#genus-degree-formula) gives

$$
g(C)=p_a(C)=\frac{(3-1)(3-2)}2=1,
$$

because the [nonsingular plane cubic](../../../algebraic-geometry.md#nonsingular-plane-cubic) is already its own [normalization of an algebraic curve](../../../normalization-of-an-algebraic-curve.md). If it were [birational](../../../algebraic-geometry.md#birational-variety) to the [projective line](../../../finite-group-theory.md#projective-line), the two [smooth projective curves](../../../projective-space.md#smooth-projective-curve) would have isomorphic [function fields](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety). The uniqueness of the [finite normalization model of a one-variable function field](../../../normalization-of-an-algebraic-curve.md#finite-normalization-model-of-a-one-variable-function-field) would then make them isomorphic. But the [projective line](../../../finite-group-theory.md#projective-line) has [genus of a smooth projective curve](../../../projective-space.md#genus-of-a-smooth-projective-curve) zero. Therefore **the cubic is not rational**. This obstruction works in the stated positive characteristics as well as in characteristic zero.

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Every [projective line](../../../finite-group-theory.md#projective-line) on the [smooth algebraic surface](../../../algebraic-geometry.md#smooth-algebraic-surface) through $P$ lies in the [projective tangent plane](../../../algebraic-geometry.md#projective-tangent-plane) $T_PS$, since its tangent direction is contained in the surface's [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space). The [plane section](../../../algebraic-geometry.md#plane-section) $S\cap T_PS$ is a nonzero [plane cubic](../../../algebraic-geometry.md#plane-cubic). It cannot be the entire plane, since a [smooth cubic surface](../../../algebraic-geometry.md#smooth-cubic-surface) is irreducible and has no plane component.

Each distinct [projective line](../../../finite-group-theory.md#projective-line) through $P$ is therefore a distinct degree-one factor of the cubic restricted to $T_PS$. A degree-three [polynomial](../../../polynomial.md) has at most three such factors. Hence there are **at most three lines through any point**. This is the [lines through a point of a smooth cubic surface](../../../algebraic-geometry.md#lines-through-a-point-of-a-smooth-cubic-surface) bound; equality is allowed when the tangent section consists of three concurrent lines.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Use coordinates in which $l=\{x_2=x_3=0\}$ and write the defining cubic as

$$
F=x_2Q_2+x_3Q_3
$$

with [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) $Q_2,Q_3$ of degree two. Their restrictions $A=Q_2|_l$, $B=Q_3|_l$ have no common zero: at such a zero all first partial derivatives of $F$ would vanish. The rational projection $[x_2:x_3]$ therefore extends to a [morphism of algebraic varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties)

$$
f:S\longrightarrow\mathbb P^1,
\qquad f|_l=[-B:A].
$$

Indeed, wherever $Q_2\ne0$, the surface equation gives $[x_2:x_3]=[-Q_3:Q_2]$, which remains regular on $l$; the analogous formula works wherever $Q_3\ne0$.

For the plane with $x_2=sw$, $x_3=tw$, its [plane section](../../../algebraic-geometry.md#plane-section) is $l$ together with the residual [plane conic](../../../algebraic-geometry.md#plane-conic)

$$
q_{s,t}(u,v,w)=sQ_2(u,v,sw,tw)+tQ_3(u,v,sw,tw)=0.
$$

These residual [plane conics](../../../algebraic-geometry.md#plane-conic) are exactly the [fibres of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism) of $f$, giving the [conic bundle from a line on a smooth cubic surface](../../../algebraic-geometry.md#conic-bundle-from-a-line-on-a-smooth-cubic-surface). The family itself is smooth: off $l$ it is the graph of projection, and over $l$ the condition $sA+tB=0$ chooses the unique value $[-B:A]$.

Write $q_{s,t}=z^{\mathsf T}M(s,t)z$ with $z=(u,v,w)^{\mathsf T}$ and $M$ symmetric. The degrees of its entries in $(s,t)$ are

$$
\begin{pmatrix}1&1&2\\1&1&2\\2&2&3\end{pmatrix}.
$$

Thus the [conic discriminant](../../../algebraic-geometry.md#conic-discriminant) $\Delta(s,t)=\det M(s,t)$ is a [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) of degree five.

Smoothness also shows that every zero of $\Delta$ is simple and has [matrix rank](../../../vector-space.md#matrix-rank) two. To see the first point, at a rank-two singular fibre let $z_0$ span the kernel and use a local base coordinate $\tau$. All fibre-coordinate derivatives vanish at $z_0$, so smoothness of the total family requires $z_0^{\mathsf T}M'(\tau)z_0\ne0$. Since the [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) of a rank-two symmetric matrix is a nonzero scalar multiple of $z_0z_0^{\mathsf T}$, the determinant derivative is nonzero. If the rank were at most one, the projective kernel would contain a line, on which the quadratic $z^{\mathsf T}M'z$ has a zero over the [algebraically closed field](../../../algebra.md#algebraically-closed-field); that point would be singular in the total family. This proves the [reduced singular fibres of a smooth conic bundle](../../../algebraic-geometry.md#reduced-singular-fibres-of-a-smooth-conic-bundle) assertion and also rules out $\Delta$ vanishing identically.

The [discriminant quintic of a cubic surface conic bundle](../../../algebraic-geometry.md#discriminant-quintic-of-a-cubic-surface-conic-bundle) consequently has five distinct zeros in $\mathbb P^1$. At each, a rank-two [plane conic](../../../algebraic-geometry.md#plane-conic) splits into two distinct [projective lines](../../../finite-group-theory.md#projective-line) $l_i,l_i'$. Neither equals $l$: that would require $sA+tB$ to vanish identically, making $A,B$ proportional, contrary to their having no common zero. The original [plane section](../../../algebraic-geometry.md#plane-section) is therefore $l\cup l_i\cup l_i'$, proving the required coplanarity and giving **five distinct pairs**.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The two [projective lines](../../../finite-group-theory.md#projective-line) in the $i$th pair form the [fibre of a morphism](../../../algebraic-geometry.md#fiber-of-a-morphism) $f^{-1}([s_i:t_i])$ of the extended [conic bundle from a line on a smooth cubic surface](../../../algebraic-geometry.md#conic-bundle-from-a-line-on-a-smooth-cubic-surface) constructed above. Distinct points of the [projective line](../../../finite-group-theory.md#projective-line) have disjoint inverse images, so

$$
(l_i\cup l_i')\cap(l_j\cup l_j')=\varnothing\qquad(i\ne j).
$$

The extension of $f$ across $l$ matters: arguing only that distinct planes through $l$ meet along $l$ would not by itself exclude intersections there. The formula $f|_l=[-B:A]$ excludes them as well. Lines within a single pair do intersect; the assertion concerns different pairs.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose one [projective line](../../../finite-group-theory.md#projective-line) from each of two different pairs. They are [skew lines](../../../geometry-and-topology.md#skew-lines) by the preceding disjointness result. After a projective linear coordinate change call them

$$
L=\{x_2=x_3=0\},\qquad M=\{x_0=x_1=0\}.
$$

For $A\in L$, $B\in M$, their joining line meets the [cubic surface](../../../algebraic-geometry.md#cubic-surface) at $A,B$ and a third point. This defines a [rational map](../../../isolated-singularity.md#rational-map-complex-analysis) $L\times M\dashrightarrow S$ on the [Zariski-open set](../../../algebraic-geometry.md#zariski-open-set) where that third intersection is distinct and the joining line is not contained in $S$.

More explicitly, because $F$ vanishes on both [projective lines](../../../finite-group-theory.md#projective-line),

$$
F(\alpha A+\beta B)=\alpha\beta\bigl(\alpha U(A,B)+\beta V(A,B)\bigr).
$$

The third point is $[VA-UB]$. Both [polynomials](../../../polynomial.md) $U,V$ are nonzero: if either vanished identically, one of the two [projective lines](../../../finite-group-theory.md#projective-line) would lie in the [singular locus](../../../algebraic-geometry.md#singular-locus). Thus $UV\ne0$ supplies a nonempty [Zariski-open set](../../../algebraic-geometry.md#zariski-open-set).

Conversely, a point $P=[x_0:x_1:x_2:x_3]$ outside $L\cup M$ lies on the unique joining line whose endpoints have coordinates $[x_0:x_1]$ on $L$ and $[x_2:x_3]$ on $M$. This is a rational inverse on the same generic locus. The [rational parametrization of a cubic surface from two skew lines](../../../algebraic-geometry.md#rational-parametrization-of-a-cubic-surface-from-two-skew-lines) gives

$$
S\ \text{birational to}\ L\times M\cong\mathbb P^1\times\mathbb P^1.
$$

The latter contains the [affine plane](../../../ringed-space.md#affine-plane) as a dense open subset, as does $\mathbb P^2$. Hence $S$ is [birational](../../../algebraic-geometry.md#birational-variety) to $\mathbb P^2$.

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [dimension of an algebraic set](../../../algebraic-geometry.md#dimension-of-an-algebraic-set) is the supremum of lengths of strict chains of nonempty [irreducible closed subsets](../../../algebraic-geometry.md#irreducible-closed-subset). It is the maximum of the dimensions of the [irreducible components](../../../algebraic-geometry.md#irreducible-component). On an [affine variety](../../../algebraic-geometry.md#affine-algebraic-set) $X=\operatorname{Spec}A$, it equals the [Krull dimension](../../../commutative-algebra.md#krull-dimension) of $A$; if $X$ is irreducible, [Noether normalization](../../../algebraic-geometry.md#noether-normalization) identifies this with the [transcendence degree](../../../algebra.md#transcendence-degree) of its [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) over $k$. Nonempty [Zariski-open subsets](../../../algebraic-geometry.md#zariski-open-set) of an irreducible [algebraic variety](../../../algebraic-geometry.md#algebraic-variety) have the same dimension, so the definition is compatible with affine charts and with [birational maps](../../../algebraic-geometry.md#birational-map). In particular, $\dim\mathbb A^n=\dim\mathbb P^n=n$ and $\dim(X\times Y)=\dim X+\dim Y$ for irreducible [algebraic varieties](../../../algebraic-geometry.md#algebraic-variety).

The [fiber dimension theorem](../../../algebraic-geometry.md#fiber-dimension-theorem) says that a dominant [morphism of algebraic varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties) $f:X\to Y$ between irreducible [algebraic varieties](../../../algebraic-geometry.md#algebraic-variety) has generic fibre dimension

$$
r=\dim X-\dim Y.
$$

Every [irreducible component](../../../algebraic-geometry.md#irreducible-component) of every nonempty fibre over a closed point has dimension at least $r$. There is a nonempty [Zariski-open subset](../../../algebraic-geometry.md#zariski-open-set) of $Y$ on which the fibres are nonempty and are [equidimensional algebraic varieties](../../../algebraic-geometry.md#equidimensional-algebraic-variety) of dimension $r$. Dominance is required; for a general [morphism of algebraic varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties), replace $Y$ by the closure of its image. This gives the [dimension of image of a morphism](../../../algebraic-geometry.md#dimension-of-image-of-a-morphism) formula.

For the generic fibre, the formula is the additivity of [transcendence degree](../../../algebra.md#transcendence-degree) in the tower $k\subset k(Y)\subset k(X)$. The lower bound on closed fibres comes from cutting by at most $\dim Y$ local parameters after a finite [Noether normalization](../../../algebraic-geometry.md#noether-normalization) of an affine target chart: the [principal hypersurface dimension lemma](../../../algebraic-geometry.md#principal-hypersurface-dimension-lemma) drops dimension by at most one per equation, and the finite normalization fibre separates the finitely many target points. For the generic upper bound, take finitely many affine source charts and apply [Noether normalization](../../../algebraic-geometry.md#noether-normalization) to each coordinate ring over $k(Y)$. Clearing denominators in $k[Y]$ makes each chart finite over $\mathbb A^r$ relative to a suitable open target chart. Its fibres have dimension at most $r$. Intersecting these finitely many target opens and using the lower bound gives [generic equidimensionality of fibres](../../../algebraic-geometry.md#generic-equidimensionality-of-fibres).

The [upper semicontinuity of local fibre dimension](../../../algebraic-geometry.md#upper-semicontinuity-of-local-fibre-dimension) is a statement on the source: for a finite-type [morphism of schemes](../../../ringed-space.md#morphism-of-schemes), the points $x$ satisfying $\dim_xX_{f(x)}\le d$ form an open set. For a [proper morphism](../../../ringed-space.md#proper-morphism), the maximum fibre dimension is upper semicontinuous on the target as well. The properness qualification matters; one should not assert the latter for every finite-type [morphism of schemes](../../../ringed-space.md#morphism-of-schemes).

A first application is dimension counting for [plane sections](../../../algebraic-geometry.md#plane-section) and intersections. On an irreducible [affine variety](../../../algebraic-geometry.md#affine-algebraic-set), imposing $q$ [polynomial](../../../polynomial.md) equations gives each nonempty component [algebraic codimension](../../../algebraic-geometry.md#codimension-of-an-algebraic-subvariety) at most $q$, by repeated [principal ideal theorem](../../../commutative-algebra.md#krull-principal-ideal-theorem). On a [smooth variety](../../../algebraic-geometry.md#smooth-algebraic-variety) this underlies the [intersection dimension bound on a smooth variety](../../../algebraic-geometry.md#intersection-dimension-bound-on-a-smooth-variety). A second application is to images: if a [morphism of algebraic varieties](../../../algebraic-geometry.md#morphism-of-algebraic-varieties) has finite nonempty fibres, its image closure has the same dimension as the source. If it is also [proper](../../../ringed-space.md#proper-morphism), that image is closed. Thus an [isolated fibre point forces dominance in equal dimensions](../../../algebraic-geometry.md#isolated-fibre-point-forces-dominance-in-equal-dimensions) when the irreducible source and target have equal dimension.

For the cubic-surface application, [projective lines](../../../finite-group-theory.md#projective-line) in $\mathbb P^3$ form the [Grassmannian](../../../differential-geometry.md#grassmannian) $G=\operatorname{Gr}(2,4)$ of dimension four. Cubic forms form $\mathbb P^{19}$, since there are $\binom63=20$ degree-three [monomials](../../../polynomial.md#monomial) in four variables. The [cubic surface line incidence variety](../../../algebraic-geometry.md#cubic-surface-line-incidence-variety)

$$
I=\{(L,[F])\in G\times\mathbb P^{19}:F|_L=0\}
$$

has fibre $\mathbb P^{15}$ over every $L$: restricting a cubic to a [projective line](../../../finite-group-theory.md#projective-line) gives four independently prescribable coefficients. It is therefore an irreducible [projective-space bundle](../../../fiber-bundle.md#projective-bundle) of dimension $4+15=19$. The other projection $\pi:I\to\mathbb P^{19}$ is a [proper morphism](../../../ringed-space.md#proper-morphism), so its image $Z$ is closed and irreducible.

To show $Z=\mathbb P^{19}$, dimension counting alone is not enough; exhibit a fibre with an isolated point. Take

$$
F_0=x_0^2x_2+x_1^2x_3,\qquad L_0=\{x_2=x_3=0\}.
$$

A nearby [projective line](../../../finite-group-theory.md#projective-line) is the graph $x_2=ax_0+bx_1$, $x_3=cx_0+dx_1$. Restriction gives

$$
F_0|_L=ax_0^3+bx_0^2x_1+cx_0x_1^2+dx_1^3.
$$

It vanishes only when $a=b=c=d=0$. Thus $L_0$ is an isolated reduced point of the fibre. Applying the lower bound in the [fiber dimension theorem](../../../algebraic-geometry.md#fiber-dimension-theorem) to $I\to Z$ gives $0\ge19-\dim Z$. Since $Z\subseteq\mathbb P^{19}$, its dimension is exactly 19, and closedness forces $Z=\mathbb P^{19}$. This is the [incidence proof that a cubic surface contains a line](../../../algebraic-geometry.md#incidence-proof-that-a-cubic-surface-contains-a-line). The auxiliary cubic $F_0$ need not be smooth: the argument proves existence for every cubic form, and hence in particular for every [smooth cubic surface](../../../algebraic-geometry.md#smooth-cubic-surface).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
