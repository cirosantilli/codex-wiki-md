# Paper 132

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_132.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_132.pdf)

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

## 1

↑ **Parent:** [Paper 132](paper-132.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Fix $z_0\in\mathcal U$. We prove the [Riemann mapping theorem](../../../complex-analysis.md#riemann-mapping-theorem) in this case by maximizing a normalized [derivative](../../../calculus.md#derivative). Choose $a\notin\mathcal U$. Since $\mathcal U$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain) and $z-a$ never vanishes, it has a [holomorphic square root](../../../complex-analysis.md#holomorphic-square-root) $g$. This $g$ is [injective](../../../algebra.md#injective-function), and $g(\mathcal U)$ is disjoint from $-g(\mathcal U)$: equality up to sign would first force the original points to coincide. Choose $b\in g(\mathcal U)$ and $r>0$ with $B(b,r)\subset g(\mathcal U)$. The ball $B(-b,r)$ is omitted, so $1/(g+b)$ is a bounded [univalent function](../../../complex-analysis.md#univalent-function). Scaling and composing with an [automorphism of the unit disk](../../../topology.md#automorphism-of-the-unit-disk) produces an [injective](../../../algebra.md#injective-function) [holomorphic function](../../../complex-analysis.md#holomorphic-function) $\phi:\mathcal U\to\mathbb D$ with $\phi(z_0)=0$ and $\phi'(z_0)>0$.

Let $\mathcal F$ be the family of all such normalized [univalent functions](../../../complex-analysis.md#univalent-function). A [Cauchy estimate](../../../analysis.md#cauchy-estimate) in a small disk about $z_0$ bounds their [derivatives](../../../calculus.md#derivative), so $M=\sup_{\phi\in\mathcal F}\phi'(z_0)$ is finite and positive. Choose a maximizing sequence in this [normal family](../../../complex-dynamics.md#normal-family). [Montel theorem](../../../complex-dynamics.md#montel-s-theorem) gives a subsequence converging uniformly on [compact](../../../topology.md#compact-space) subsets to $\phi$. Its [derivative](../../../calculus.md#derivative) at $z_0$ is $M>0$. The [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) puts its image in $\mathbb D$, and [Hurwitz's theorem](../../../complex-analysis.md#hurwitz-s-theorem) implies that a nonconstant limit of [injective](../../../algebra.md#injective-function) [holomorphic functions](../../../complex-analysis.md#holomorphic-function) is [injective](../../../algebra.md#injective-function). Thus the maximum is attained.

If $a_1\in\mathbb D$ is omitted, then $a_1\ne0$. Put $T_a(w)=(w-a)/(1-\overline a w)$. A [holomorphic square root](../../../complex-analysis.md#holomorphic-square-root) $v$ of $T_{a_1}\circ\phi$ exists, is [injective](../../../algebra.md#injective-function), and takes values in $\mathbb D$. Compose $v$ with $T_{v(z_0)}$ and a rotation to normalize it. Writing $s=|a_1|\in(0,1)$, the new [derivative](../../../calculus.md#derivative) has magnitude

$$
M\frac{1-s^2}{2\sqrt s(1-s)}
=M\frac{1+s}{2\sqrt s}>M,
$$

a contradiction. Therefore $\phi$ maps onto $\mathbb D$. The [Cayley transform between the half-plane and disk](../../../complex-analysis.md#cayley-transform-between-the-half-plane-and-disk) now gives

$$
\boxed{f(z)=i\,\frac{1+\phi(z)}{1-\phi(z)}:\mathcal U\xrightarrow{\sim}\mathbb H,\qquad
\operatorname{Im}f(z)=\frac{1-|\phi(z)|^2}{|1-\phi(z)|^2}>0.}
$$

Its inverse is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) by the [holomorphic inverse function theorem](../../../geometry-and-topology.md#holomorphic-inverse-function-theorem), so this is a [biholomorphism](../../../complex-analysis.md#biholomorphism). The proper-subset hypothesis was used to choose $a\notin\mathcal U$; the whole [complex plane](../../../complex-analysis.md#complex-plane) cannot be mapped this way, by [Liouville theorem](../../../complex-analysis.md#liouville-theorem).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Interpret the printed congruence entrywise in the integer lattice:

$$
a,d\in1+2\mathbb Z,\qquad b,c\in2\mathbb Z.
$$

It then defines the usual level-two [principal congruence subgroup](../../../group-theory.md#principal-congruence-subgroup) of $\mathrm{SL}_2(\mathbb Z)$, despite the PDF's ambient $\mathrm{SL}_2(\mathbb R)$. A literal ideal congruence inside $\mathbb R$ would be vacuous because $2\mathbb R=\mathbb R$, and would make the asserted conclusion false. The integer-lattice interpretation is essential.

Pass to $\overline{\Gamma(2)}=\Gamma(2)/\{\pm I\}$, which has exactly the same action. Reduction modulo two maps the [modular group](../../../modular-function.md#modular-group) onto $\mathrm{SL}_2(\mathbb F_2)$, a group of order six: the reductions of $S$ and $T$ generate it. Its kernel is $\overline{\Gamma(2)}$, so the [index of a subgroup](../../../group.md#index-of-a-subgroup) is six. The [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) has [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) $\pi/3$, and hence the quotient has [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) $2\pi$.

There are no nonidentity [elliptic Möbius transformations](../../../geometry-and-topology.md#elliptic-element-of-psl2-r) in $\overline{\Gamma(2)}$. An integral matrix representing an [elliptic Möbius transformation](../../../geometry-and-topology.md#elliptic-element-of-psl2-r) has [trace](../../../linear-algebra.md#matrix-trace) $0$ or $\pm1$. Here the [trace](../../../linear-algebra.md#matrix-trace) is even, excluding $\pm1$; [trace](../../../linear-algebra.md#matrix-trace) zero would give $d=-a$ and $1=-a^2-bc\equiv-1\pmod4$, impossible. Thus the effective action is a free [properly discontinuous group action](../../../geometric-group-theory.md#properly-discontinuous-group-action), and the quotient is a [Riemann surface](../../../complex-analysis.md#riemann-surfaces).

A [cusp of a modular group](../../../modular-function.md#cusp-of-a-modular-group) is represented by a rational boundary point. Their orbits correspond to

$$
\mathrm{SL}_2(\mathbb F_2)/\langle\overline T\rangle,
$$

which has $6/2=3$ elements. They are represented by $\infty,0,1$, or by the three nonzero parity vectors of a primitive numerator-denominator pair. Each [width of a cusp](../../../modular-function.md#width-of-a-cusp) is two. A union of six copies of the [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) gives a fundamental region for this subgroup. Removing small [horocycle](../../../geometry-and-topology.md#horocycle) neighbourhoods of its cusps leaves a [compact](../../../topology.md#compact-space) core. Adding one point at each [cusp of a modular group](../../../modular-function.md#cusp-of-a-modular-group), using the local parameter $e^{\pi i z}$ after moving that cusp to infinity, gives a [compact](../../../topology.md#compact-space) [Riemann surface](../../../complex-analysis.md#riemann-surfaces) $\overline X$.

For a finite-area [hyperbolic surface](../../../geometry-and-topology.md#hyperbolic-surface) of [genus](../../../topology.md#genus-of-a-surface) $g$ with $r$ cusps, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives area $2\pi(2g-2+r)$. Thus $2\pi=2\pi(2g-2+3)$ and $g=0$. A [compact](../../../topology.md#compact-space) [genus](../../../topology.md#genus-of-a-surface)-zero [Riemann surface](../../../complex-analysis.md#riemann-surfaces) is the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), by the [uniformization theorem](../../../complex-analysis.md#uniformization-theorem). A [Möbius transformation](../../../group-theory.md#mobius-transformation) sends the three added points to $0,1,\infty$. Restricting it gives

$$
\boxed{\mathbb H/\Gamma(2)\cong\mathbb P^1\setminus\{0,1,\infty\}
=\mathbb C\setminus\{0,1\}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) $-1$ normalization

$$
ds^2=\frac{dx^2+dy^2}{y^2}
$$

of the [Poincaré half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model). This is a complete [conformal metric](../../../complex-analysis.md#conformal-metric), invariant under real [Möbius transformations](../../../group-theory.md#mobius-transformation). Its quotient by the free effective [principal congruence subgroup](../../../group-theory.md#principal-congruence-subgroup) is again complete: a [geodesic](../../../riemannian-geometry.md#geodesic) lifts to the complete covering plane and extends there for all time. Transporting the quotient metric through the [biholomorphism](../../../complex-analysis.md#biholomorphism) supplies the required complete [conformal metric](../../../complex-analysis.md#conformal-metric).

A nonconstant closed [geodesic](../../../riemannian-geometry.md#geodesic) corresponds to a [hyperbolic Möbius transformation](../../../geometry-and-topology.md#hyperbolic-element-of-psl2-r) $A$ of $\Gamma(2)$, and its [hyperbolic translation length](../../../geometry-and-topology.md#hyperbolic-translation-length) is $2\operatorname{arcosh}(|\operatorname{tr}A|/2)$. Indeed its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have magnitudes $\lambda,\lambda^{-1}$ with $\lambda>1$, and its axis quotient has length $2\log\lambda$. For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ in $\Gamma(2)$, $bc\equiv0\pmod4$ implies $ad\equiv1\pmod4$. The odd numbers $a,d$ therefore have the same residue modulo four, and

$$
\operatorname{tr}A=a+d\equiv2\pmod4.
$$

A [hyperbolic Möbius transformation](../../../geometry-and-topology.md#hyperbolic-element-of-psl2-r) must have $|\operatorname{tr}A|>2$, so its smallest possible absolute [trace](../../../linear-algebra.md#matrix-trace) is six. It is attained by

$$
\begin{pmatrix}1&2\\0&1\end{pmatrix}
\begin{pmatrix}1&0\\2&1\end{pmatrix}
=\begin{pmatrix}5&2\\2&1\end{pmatrix}.
$$

Consequently

$$
\boxed{\ell_{\min}=2\operatorname{arcosh}3=2\log(3+2\sqrt2).}
$$

This element is primitive: a proper power would have a shorter root represented by a [hyperbolic Möbius transformation](../../../geometry-and-topology.md#hyperbolic-element-of-psl2-r), contradicting the [trace](../../../linear-algebra.md#matrix-trace) bound. No essential simple closed [geodesic](../../../riemannian-geometry.md#geodesic) exists on the three-punctured sphere, since every essential simple loop is peripheral and corresponds to a [parabolic Möbius transformation](../../../geometry-and-topology.md#parabolic-element-of-psl2-r). The minimizing closed [geodesic](../../../riemannian-geometry.md#geodesic) is therefore nonsimple. Finally, the PDF leaves the numerical [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) unspecified: the displayed length uses [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) $-1$; for [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) $-\kappa^2$, it is divided by $\kappa$.

## 2

↑ **Parent:** [Paper 132](paper-132.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

First use the nonzero loci, as required by the standard [SL2R action on differentials](../../../complex-analysis.md#sl2r-action-on-differentials). A nonzero [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) has, away from its zeros, [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential)

$$
w=\int\omega,\qquad\omega=dw,
$$

whose changes of coordinate are translations. A nonzero [holomorphic quadratic differential](../../../complex-geometry.md#holomorphic-quadratic-differential) similarly has local [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) $w=\int\sqrt q$, with $q=dw^2$ and changes of coordinate $w_j=\pm w_i+c_{ij}$. These are respectively [translation surfaces](../../../complex-analysis.md#translation-surface) and [half-translation surfaces](../../../complex-geometry.md#half-translation-surface).

Identify a [flat coordinate](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) with a vector in $\mathbb R^2$. For $A\in\mathrm{SL}_2(\mathbb R)$, replace every [flat coordinate](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) by $W=Aw$. Since $A$ preserves [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) and commutes with multiplication by $-1$, the new changes of coordinate are

$$
W_j=W_i+Ac_{ij},\qquad\text{or}\qquad W_j=\pm W_i+Ac_{ij}.
$$

They are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in the new coordinates, and so define a new [complex structure](../../../complex-geometry.md#complex-structure). Define $\omega_A=dW$ or $q_A=dW^2$ in that structure. The forms glue because translations preserve $dW$, and the extra signs preserve $dW^2$.

The zeros also extend. A zero of order $m$ of a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) has [cone angle](../../../differential-geometry.md#cone-angle) $2\pi(m+1)$; a zero of order $m$ of a [holomorphic quadratic differential](../../../complex-geometry.md#holomorphic-quadratic-differential) has [cone angle](../../../differential-geometry.md#cone-angle) $(m+2)\pi$. The real-linear deformation preserves the corresponding winding multiplicity. Filling the cone in a local coordinate $\zeta$ gives $W=\zeta^{m+1}$ in the first case, or a local branch of $W=\zeta^{(m+2)/2}$ in the second. Thus the resulting forms are constant multiples of $\zeta^m\,d\zeta$ or $\zeta^m\,d\zeta^2$ and have the same [zero orders](../../../complex-geometry.md#order-of-a-zero-of-a-differential). This verifies extension across the missing points, rather than merely producing an atlas on the punctured surface.

An isomorphism preserving the original differential identifies its [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) up to the permitted translations or signs; applying $A$ identifies the deformed atlases too. Hence the construction descends to the corresponding [moduli spaces](../../../geometry-and-topology.md#moduli-space). Applying $B$ after $A$ replaces $w$ by $BAw$, so

$$
\boxed{B\cdot(A\cdot(X,\omega))=(BA)\cdot(X,\omega),\qquad
B\cdot(A\cdot(X,q))=(BA)\cdot(X,q).}
$$

The [area of a quadratic differential](../../../complex-geometry.md#area-of-a-quadratic-differential), and the analogous area of a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form), are preserved because $\det A=1$.

For $q=\omega^2$, the [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) obtained from $\omega$ already give the required [half-translation surface](../../../complex-geometry.md#half-translation-surface) atlas for $q$. The same replacement $w\mapsto Aw$ therefore constructs both deformations, and

$$
\boxed{A\cdot(X,\omega^2)=(X_A,\omega_A^2)=s\bigl(A\cdot(X,\omega)\bigr).}
$$

The printed sets include identically zero differentials. They have no [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential), so the customary geometric [group action](../../../group-theory.md#group-action) is defined on the nonzero loci. One can obtain a set-theoretic action on the displayed entire sets by declaring $A\cdot(X,0)=(X,0)$; the same equivariance identity then holds at zero. This extension is generally not continuous: as $t\omega\to0$, the deformed underlying surface is the same $X_A$ for every real $t>0$, and can differ from $X$. Thus a claim about the standard continuous geometric [group action](../../../group-theory.md#group-action) requires the nonzero convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**The analogous flat-coordinate construction does not define a full $\mathrm{SL}_2(\mathbb R)$ action on arbitrary cubic differentials.** Away from zeros, a nonzero [holomorphic cubic differential](../../../complex-geometry.md#holomorphic-cubic-differential) has [flat coordinates](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential)

$$
w=\int c^{1/3},\qquad c=dw^3.
$$

Their changes of coordinate are $w_j=\zeta w_i+b_{ij}$ with $\zeta^3=1$. A branch change is therefore a rotation through $2\pi/3$, not merely a sign. Applying a real-linear map $A$ changes its linear part to $ARA^{-1}$, where $R$ is that rotation. In general this is not a [complex-linear map](../../../vector-space.md#complex-linear-map), so the proposed changes of coordinate are not [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) and cannot define the required deformed [complex structure](../../../complex-geometry.md#complex-structure).

For example, take $A=\operatorname{diag}(2,1/2)$ and $R=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}$ with $\theta=2\pi/3$. Then

$$
ARA^{-1}=
\begin{pmatrix}\cos\theta&-4\sin\theta\\\frac14\sin\theta&\cos\theta\end{pmatrix},
$$

whose off-diagonal entries fail the condition for a [complex-linear map](../../../vector-space.md#complex-linear-map). This dependence on the choice of cube-root coordinate is the obstruction even when considering descent from the locus $c=\omega^3$: the three possible roots need not lead to the same deformation of the cubic pair.

The real matrices preserving [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) that normalize the order-three rotations are precisely the matrices of [complex-linear maps](../../../vector-space.md#complex-linear-map); intersecting with $\mathrm{SL}_2(\mathbb R)$ leaves $\mathrm{SO}(2)$. Indeed a nonreal rotation determines its [complex structure](../../../complex-geometry.md#complex-structure), and conjugation to its inverse would reverse that structure's [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). Thus there is a natural rotation action,

$$
\boxed{R_\theta\cdot(X,c)=(X,e^{3i\theta}c).}
$$

The conclusion concerns the geometric [group action](../../../group-theory.md#group-action) analogous to that for [translation surfaces](../../../complex-analysis.md#translation-surface) and [half-translation surfaces](../../../complex-geometry.md#half-translation-surface); it does not rule out artificial group actions unrelated to these atlases.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Label the polygon vertices $v_0,\ldots,v_{2n-1}$ cyclically. Translation pairing of opposite sides identifies

$$
v_i\sim v_{i+n+1},\qquad v_{i+1}\sim v_{i+n},
$$

with indices modulo $2n$. The vertex classes are consequently the cosets of the subgroup generated by $n-1$ in $\mathbb Z/(2n)$, and their number is

$$
V=\gcd(2n,n-1)=
\begin{cases}1,&n\text{ even},\\2,&n\text{ odd}.\end{cases}
$$

The quotient is a [compact](../../../topology.md#compact-space) [Hausdorff space](../../../topology.md#hausdorff-space). An interior point has a disk neighbourhood, a paired-side point has two half-disks joined to a disk, and each vertex class has its incident sectors cyclically joined to a cone, topologically a disk. Thus it is a [connected](../../../geometry-and-topology.md#connected-space) [closed surface](../../../differential-geometry.md#closed-surface) with an [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). Its [Euler characteristic](../../../homology.md#euler-characteristic) is $V-n+1$, since there are $n$ paired edges and one face. Hence

$$
\boxed{g(X_n)=\frac{n+1-V}{2}=\left\lfloor\frac n2\right\rfloor.}
$$

The polygon interior and paired-side charts are [translation surface](../../../complex-analysis.md#translation-surface) charts with $\omega_n=dz$. Each corner angle is $(n-1)\pi/n$. For even $n$, all $2n$ corners meet, giving [cone angle](../../../differential-geometry.md#cone-angle) $2\pi(n-1)$; for odd $n$, each of the two classes contains $n$ corners, giving [cone angle](../../../differential-geometry.md#cone-angle) $(n-1)\pi$. Both are integral multiples of $2\pi$. A cone of angle $2\pi(k+1)$ has the local uniformizing coordinate $\zeta$ with $w=\zeta^{k+1}$; the [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) is $(k+1)\zeta^k\,d\zeta$. Filling the vertices therefore supplies the [Riemann surface](../../../complex-analysis.md#riemann-surfaces) structure and the [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form), with

$$
\boxed{\begin{array}{ll}
n\text{ even}:&\text{one vertex class of zero order }n-2,\\
n\text{ odd}:&\text{two vertex classes, each of zero order }(n-3)/2.
\end{array}}
$$

An order-zero entry denotes a regular point, not an actual zero: for $n=2,3$ the surface is a [torus](../../../topology.md#torus) and the form is nowhere zero. The [zero orders](../../../complex-geometry.md#order-of-a-zero-of-a-differential) otherwise sum to $2g-2$, as a check against the degree of the [canonical bundle](../../../complex-geometry.md#canonical-bundle).

<a id="2/c/image-opposite-side-pairings-one-vertex-class-in-the-octagon-and-two-in-the-decagon"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132-polygons.png)

**[Figure 1](#2/c/image-opposite-side-pairings-one-vertex-class-in-the-octagon-and-two-in-the-decagon). Opposite-side pairings: one vertex class in the octagon and two in the decagon**.

For $n=4$, the form has one double zero and lies in the [stratum of holomorphic one-forms](../../../complex-geometry.md#stratum-of-holomorphic-one-forms) $\mathcal H(2)$; for $n=5$, it has two simple zeros and lies in $\mathcal H(1,1)$. The [SL2R action on differentials](../../../complex-analysis.md#sl2r-action-on-differentials) preserves zero multiplicities, as the local cone argument shows. Therefore

$$
\boxed{(X_4,\omega_4)\text{ and }(X_5,\omega_5)\text{ are not in the same }\mathrm{SL}_2(\mathbb R)\text{ orbit}.}
$$

Their equal [genus](../../../topology.md#genus-of-a-surface) and area do not distinguish the orbits; their different [strata of holomorphic one-forms](../../../complex-geometry.md#stratum-of-holomorphic-one-forms) do.

## 3

↑ **Parent:** [Paper 132](paper-132.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A generalized [conformal metric](../../../complex-analysis.md#conformal-metric) is locally $ds_\rho=\rho(z)|dz|$, where $\rho$ is nonnegative and measurable and transforms as a length density under a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) change of coordinate. Its area is $A_\rho=\int_X\rho^2\,dx\,dy$. Use the usual convention of using [locally rectifiable paths](../../../geometry-and-topology.md#locally-rectifiable-path) for a [path family](../../../geometry-and-topology.md#path-family) $\Gamma$, and put $L_\rho(\Gamma)=\inf_{\gamma\in\Gamma}\int_\gamma\rho|dz|$. Then

$$
\boxed{\lambda(\Gamma,X)=\sup_{\rho:\ 0<A_\rho<\infty}
\frac{L_\rho(\Gamma)^2}{A_\rho}.}
$$

This is [extremal length](../../../complex-analysis.md#extremal-length). Zeros and isolated singularities of an admissible density are allowed; requiring a [smooth](../../../analysis.md#smooth-function) strictly positive [Riemannian metric](../../../differential-geometry.md#riemannian-metric) would unnecessarily restrict the definition. Line integrals have their extended nonnegative values; if an arbitrary family is supplied, use its members that are [locally rectifiable paths](../../../geometry-and-topology.md#locally-rectifiable-path). An empty [path family](../../../geometry-and-topology.md#path-family) has infinite infimal length, whereas a family containing a constant path has [extremal length](../../../complex-analysis.md#extremal-length) zero.

Both numerator and denominator scale quadratically when $\rho$ is multiplied by a positive constant. The coordinate transformation of the area element makes the quotient unchanged under [conformal equivalence](../../../geometry-and-topology.md#conformal-equivalence).

The normalization relevant later is worth deriving. On the [conformal cylinder](../../../complex-analysis.md#conformal-cylinder) $(\mathbb R/\mathbb Z)\times(0,M)$, let $\Gamma$ contain the loops going once around it. For the horizontal loop at height $t$, [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\left(\int_0^1\rho(x,t)\,dx\right)^2\leq\int_0^1\rho(x,t)^2\,dx.
$$

Integrating in $t$ shows $L_\rho(\Gamma)^2\leq A_\rho/M$. The constant density achieves equality, since every winding-one loop has Euclidean length at least one. Hence

$$
\boxed{\lambda(\Gamma,\text{cylinder})=\frac1M.}
$$

Here $M$ is the height divided by circumference, the [conformal modulus of an annulus](../../../complex-analysis.md#conformal-modulus-of-an-annulus); the reciprocal is used for the family joining its boundary components.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

In local [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate), write the two positive [singular values](../../../linear-algebra.md#singular-value) of $Df$ as $s_1\geq s_2$. Preservation of [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) gives $J_f=s_1s_2$, and [quasiconformality](../../../complex-analysis.md#quasiconformal-mapping) gives $s_1/s_2\leq K$.

For an admissible [conformal metric](../../../complex-analysis.md#conformal-metric) $\rho|dw|$ on $Y$, define a density on $X$ by $\sigma(z)=\rho(f(z))s_1(z)$. Along each path,

$$
\int_{f(\gamma)}\rho|dw|
\leq\int_\gamma\sigma|dz|,
$$

so $L_\rho(f(\Gamma))\leq L_\sigma(\Gamma)$. The [change of variables formula](../../../calculus.md#change-of-variables-formula) and $s_1^2\leq KJ_f$ give

$$
A_\sigma=\int_X\rho(f(z))^2s_1(z)^2\,dx\,dy
\leq K\int_X\rho(f(z))^2J_f(z)\,dx\,dy
=KA_\rho.
$$

Also $s_1^2\geq J_f$, so $A_\sigma\geq A_\rho>0$. Thus $\sigma$ has positive finite area and is admissible, and

$$
\frac{L_\rho(f(\Gamma))^2}{A_\rho}
\leq K\,\frac{L_\sigma(\Gamma)^2}{A_\sigma}
\leq K\,\lambda(\Gamma,X).
$$

Taking the [supremum](../../../real-analysis.md#supremum) over $\rho$ proves

$$
\boxed{\lambda(f(\Gamma),Y)\leq K\lambda(\Gamma,X).}
$$

Applying the same argument to $f^{-1}$, which has the same bound on its [maximal dilatation](../../../complex-analysis.md#maximal-dilatation), also gives $K^{-1}\lambda(\Gamma,X)\leq\lambda(f(\Gamma),Y)$. The inequalities remain valid for extended [extremal lengths](../../../complex-analysis.md#extremal-length); no extremizing density need exist.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the closed [genus](../../../topology.md#genus-of-a-surface) $g\geq2$ version of [Teichmüller's uniqueness theorem](../../../complex-analysis.md#teichmuller-s-uniqueness-theorem). Let $f_0:X\to Y$ be a [Teichmüller map](../../../complex-analysis.md#teichmuller-map): for a nonzero [holomorphic quadratic differential](../../../complex-geometry.md#holomorphic-quadratic-differential) $q$, normalized by $\int_X|q|=1$, and $0<k_0<1$,

$$
\mu_{f_0}=k_0\frac{|q|}{q},\qquad K_0=\frac{1+k_0}{1-k_0}.
$$

The value at a zero of $q$ is irrelevant to the [Beltrami coefficient](../../../complex-analysis.md#beltrami-coefficient), which is defined almost everywhere. For every [quasiconformal map](../../../complex-analysis.md#quasiconformal-mapping) $f:X\to Y$ preserving [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) and [homotopic](../../../algebraic-topology.md#homotopy) to $f_0$, the conclusion is

$$
\boxed{K(f)\geq K_0,\qquad K(f)=K_0\ \Longrightarrow\ f=f_0.}
$$

The normalized $q$ is also uniquely determined when $k_0>0$.

We use the following analytic input, stated with its hypotheses. The [Reich–Strebel inequality](../../../complex-analysis.md#reich-strebel-inequality) says that if $f_0$ has the displayed [Beltrami coefficient](../../../complex-analysis.md#beltrami-coefficient) and a competitor $f$ has the same target and [homotopy class](../../../algebraic-topology.md#homotopy-class), then, for $\mu=\mu_f$,

$$
K_0\leq\int_X\frac{|1+\mu q/|q||^2}{1-|\mu|^2}\,|q|.
$$

This is the standard fundamental inequality for an integrable [holomorphic quadratic differential](../../../complex-geometry.md#holomorphic-quadratic-differential); it also holds on a finite-type punctured surface with the homotopy fixing the punctures. Its formulation is given in [Gardiner and Hu, §5](https://userhome.brooklyn.cuny.edu/gardiner/A%20short%20course%20on%20Teichmuller%27s%20theorem.pdf). We quote this analytic inequality as the lecture result used in the proof.

Put $k=\|\mu\|_\infty$. Pointwise, away from the isolated zeros of $q$,

$$
\frac{|1+\mu q/|q||^2}{1-|\mu|^2}
\leq\frac{(1+|\mu|)^2}{1-|\mu|^2}
=\frac{1+|\mu|}{1-|\mu|}
\leq\frac{1+k}{1-k}.
$$

Integrating against the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $|q|$ proves $K_0\leq K(f)$. If $K(f)=K_0$, all these inequalities are equalities almost everywhere. The strictly increasing last function forces $|\mu|=k_0$ almost everywhere; equality in the [triangle inequality](../../../topological-analysis.md#triangle-inequality) then forces $\mu q/|q|=k_0$. Therefore

$$
\mu_f=\mu_{f_0}\quad\text{almost everywhere}.
$$

Two [quasiconformal maps](../../../complex-analysis.md#quasiconformal-mapping) with the same [Beltrami coefficient](../../../complex-analysis.md#beltrami-coefficient) differ by postcomposition with a [biholomorphism](../../../complex-analysis.md#biholomorphism), by the local chain rule for the [Beltrami equation](../../../complex-analysis.md#beltrami-equation). Consequently $h=f\circ f_0^{-1}$ is a [biholomorphism](../../../complex-analysis.md#biholomorphism) from $Y$ to itself [homotopic](../../../algebraic-topology.md#homotopy) to the identity.

For completeness, such a [biholomorphism](../../../complex-analysis.md#biholomorphism) is the identity when $g\geq2$. Apply the [uniformization theorem](../../../complex-analysis.md#uniformization-theorem) and choose the lift of the homotopy to $\mathbb H$ starting at the identity. Its endpoint lift $\widetilde h$ commutes with every [deck transformation](../../../algebraic-topology.md#deck-transformation). It is a real [Möbius transformation](../../../group-theory.md#mobius-transformation). The [compact](../../../topology.md#compact-space) quotient has no [parabolic Möbius transformations](../../../geometry-and-topology.md#parabolic-element-of-psl2-r) in its deck group, and freeness excludes [elliptic Möbius transformations](../../../geometry-and-topology.md#elliptic-element-of-psl2-r). Two distinct hyperbolic axes exist: a discrete free group preserving just one axis would be cyclic, contradicting the [fundamental group](../../../algebraic-topology.md#fundamental-group) of a [closed surface](../../../differential-geometry.md#closed-surface) of [genus](../../../topology.md#genus-of-a-surface) at least two. Commutation with two [deck transformations](../../../algebraic-topology.md#deck-transformation) represented by [hyperbolic Möbius transformations](../../../geometry-and-topology.md#hyperbolic-element-of-psl2-r) having distinct axes makes it fix their boundary endpoints individually; there are at least three such endpoints. A [Möbius transformation](../../../group-theory.md#mobius-transformation) fixing three points is the identity. Hence $h=\operatorname{id}$ and $f=f_0$.

If $q_1$ is another unit-area differential for the same map, then $|q_1|/q_1=|q|/q$, so $q_1/q$ is positive real wherever defined. This [meromorphic function](../../../isolated-singularity.md#meromorphic-function) is constant by the [open mapping theorem](../../../functional-analysis.md#open-mapping-theorem-functional-analysis), and normalization makes the constant one. Without normalization, positive multiples of $q$ describe the same map. At $k_0=0$, uniqueness of the map still holds in [genus](../../../topology.md#genus-of-a-surface) at least two, but there is no distinguished $q$. In [genus](../../../topology.md#genus-of-a-surface) one, translations supply nontrivial [biholomorphisms](../../../complex-analysis.md#biholomorphism) [homotopic](../../../algebraic-topology.md#homotopy) to the identity, so equality determines the map only up to those [biholomorphisms](../../../complex-analysis.md#biholomorphism); the [genus](../../../topology.md#genus-of-a-surface) hypothesis cannot be omitted.

## 4

↑ **Parent:** [Paper 132](paper-132.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For fixed $g\geq2$, [Mumford's compactness theorem](../../../geometry-and-topology.md#mumford-s-compactness-theorem) states that

$$
\boxed{\mathcal M_g^\varepsilon
=\{X\in\mathcal M_g:\operatorname{sys}_{\rm hyp}(X)\geq\varepsilon\}
\text{ is compact for every }\varepsilon>0.}
$$

Here $\mathcal M_g$ is the unmarked [moduli space of Riemann surfaces](../../../geometry-and-topology.md#moduli-space-of-riemann-surfaces), with its usual topology, and the [hyperbolic systole](../../../geometry-and-topology.md#hyperbolic-systole) is the shortest nonconstant closed hyperbolic [geodesic](../../../riemannian-geometry.md#geodesic), in [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) $-1$. Equivalently, a subset of $\mathcal M_g$ is relatively [compact](../../../topology.md#compact-space) exactly when its [hyperbolic systoles](../../../geometry-and-topology.md#hyperbolic-systole) have a common positive lower bound.

We use two standard structural results. The [Bers pants decomposition theorem](../../../geometry-and-topology.md#bers-pants-decomposition-theorem) provides a constant $B_g$ such that every closed [genus](../../../topology.md#genus-of-a-surface)-$g$ [hyperbolic surface](../../../geometry-and-topology.md#hyperbolic-surface) has a [pants decomposition](../../../geometry-and-topology.md#pants-decomposition) with all $3g-3$ cuff lengths at most $B_g$. For a fixed topological [pants decomposition](../../../geometry-and-topology.md#pants-decomposition), the [Fenchel–Nielsen coordinates](../../../geometry-and-topology.md#fenchel-nielsen-coordinates) identify [Teichmüller space](../../../complex-analysis.md#teichmuller-space) with

$$
(0,\infty)^{3g-3}\times\mathbb R^{3g-3}.
$$

The length coordinates are $\ell_i$, and the twist coordinates $\tau_i$ are measured in length units: a full [Dehn twist](../../../topology.md#dehn-twist) changes $\tau_i$ by $\ell_i$. Reconstruction from these coordinates is continuous; locally the marked metrics can be chosen to vary smoothly on a fixed reference surface, and the quotient by the [mapping class group](../../../topology.md#mapping-class-group) is the Hausdorff [moduli space of Riemann surfaces](../../../geometry-and-topology.md#moduli-space-of-riemann-surfaces).

Take any sequence in $\mathcal M_g^\varepsilon$. The [pants decompositions](../../../geometry-and-topology.md#pants-decomposition) supplied by the [Bers pants decomposition theorem](../../../geometry-and-topology.md#bers-pants-decomposition-theorem) have cuff lengths in $[\varepsilon,B_g]$. There are finitely many topological types of [pants decomposition](../../../geometry-and-topology.md#pants-decomposition): their dual graphs have $2g-2$ vertices and $3g-3$ edges, with loops and multiple edges allowed, giving finitely many finite graphs. Choose a subsequence of one type, and choose markings carrying each decomposition to a fixed reference one. Compose these markings with [Dehn twists](../../../topology.md#dehn-twist) so that $0\leq\tau_i\leq\ell_i$. The resulting points of [Teichmüller space](../../../complex-analysis.md#teichmuller-space) lie in the [compact](../../../topology.md#compact-space) box

$$
[\varepsilon,B_g]^{3g-3}\times[0,B_g]^{3g-3}.
$$

They therefore have a convergent subsequence inside [Teichmüller space](../../../complex-analysis.md#teichmuller-space); its continuous projection gives a convergent subsequence in the [moduli space of Riemann surfaces](../../../geometry-and-topology.md#moduli-space-of-riemann-surfaces). If $\varepsilon>B_g$ the thick set is empty, which is already [compact](../../../topology.md#compact-space). Equivalently, using all the finitely many reference decompositions gives a finite union of [compact](../../../topology.md#compact-space) projected boxes containing the whole thick set.

Finally the [hyperbolic systole](../../../geometry-and-topology.md#hyperbolic-systole) is continuous. Nearby marked [hyperbolic surfaces](../../../geometry-and-topology.md#hyperbolic-surface) admit metric comparisons with [bi-Lipschitz distortion](../../../functional-analysis.md#stretch-factor) tending to one; the length of every loop, and hence the [infimum](../../../real-analysis.md#infimum) over all essential loops, obeys the same multiplicative comparison. Therefore $\mathcal M_g^\varepsilon$ is closed in that [compact](../../../topology.md#compact-space) union and is [compact](../../../topology.md#compact-space). A [compact](../../../topology.md#compact-space) subset has a positive minimum [hyperbolic systole](../../../geometry-and-topology.md#hyperbolic-systole), proving the converse characterization of relative compactness. This theorem concerns the unmarked quotient: repeated [Dehn twists](../../../topology.md#dehn-twist) can give an unbounded sequence in [Teichmüller space](../../../complex-analysis.md#teichmuller-space) while leaving the underlying surface and its [hyperbolic systole](../../../geometry-and-topology.md#hyperbolic-systole) unchanged.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The given $\gamma$ is a [simple closed curve](../../../geometry-and-topology.md#simple-closed-curve). Assume it is essential; for a contractible class both infimal lengths are already zero. Write $\ell_n=\ell_{X_n}(\gamma)$. The [collar lemma](../../../geometry-and-topology.md#collar-lemma) supplies an embedded [annulus](../../../topology.md#annulus-mathematics) with coordinates $r\in(-w_n,w_n)$ and $t\in\mathbb R/\mathbb Z$, and metric

$$
ds^2=dr^2+\ell_n^2\cosh^2r\,dt^2,\qquad
\sinh w_n\,\sinh(\ell_n/2)=1.
$$

Set $y(r)=\ell_n^{-1}\int_0^r\operatorname{sech}s\,ds$. This changes the metric to a positive scalar multiple of $dt^2+dy^2$, so the [conformal modulus of an annulus](../../../complex-analysis.md#conformal-modulus-of-an-annulus) is

$$
M_n=\frac2{\ell_n}\int_0^{w_n}\operatorname{sech}r\,dr
=\frac2{\ell_n}\arctan\!\left(\frac1{\sinh(\ell_n/2)}\right)
\sim\frac\pi{\ell_n}\longrightarrow\infty.
$$

The [extremal length](../../../complex-analysis.md#extremal-length) of its core curves is $1/M_n$. Allowing all curves [homotopic](../../../algebraic-topology.md#homotopy) to $\gamma$ in $X_n$ can only decrease infimal lengths, while the area of a metric on all of $X_n$ is at least its area on the collar. Thus $\lambda(\gamma,X_n)\leq1/M_n$. Use the particular [conformal metric](../../../complex-analysis.md#conformal-metric) $|q_n|^{1/2}$, whose [area of a quadratic differential](../../../complex-geometry.md#area-of-a-quadratic-differential) is one:

$$
\boxed{L(\gamma,|q_n|^{1/2})^2
\leq\lambda(\gamma,X_n)\leq\frac1{M_n}\longrightarrow0.}
$$

This proves the required implication uniformly over all the area-one [holomorphic quadratic differentials](../../../complex-geometry.md#holomorphic-quadratic-differential) on these surfaces.

**The converse is false.** Here is an explicit [slit connected sum of translation tori](../../../complex-analysis.md#slit-connected-sum-of-translation-tori). Start with square flat copies of a [torus](../../../topology.md#torus) $T_1=\mathbb C/(\mathbb Z+i\mathbb Z)$ and $T_\delta=\mathbb C/(\delta\mathbb Z+i\delta\mathbb Z)$, where $\delta\to0$. Cut a horizontal slit of physical length $\delta^2$ in each, centred in an interior coordinate disk, and cross-glue the banks by translation. The resulting surface has [genus](../../../topology.md#genus-of-a-surface) two. Its two slit endpoints have [cone angle](../../../differential-geometry.md#cone-angle) $4\pi$, so the locally defined $dz$ extends to a [holomorphic one-form](../../../complex-geometry.md#holomorphic-one-form) $\omega_\delta$ with two simple zeros. Its flat area is $1+\delta^2$. Set

$$
q_\delta=\frac{\omega_\delta^2}{1+\delta^2},
$$

which is a [holomorphic quadratic differential](../../../complex-geometry.md#holomorphic-quadratic-differential) of area one. Let $\gamma$ be a horizontal generator in the small [torus](../../../topology.md#torus), taken away from the slit and fixed by the marking of this small handle. Then

$$
L(\gamma,|q_\delta|^{1/2})\leq\frac{\delta}{\sqrt{1+\delta^2}}\longrightarrow0.
$$

To verify that its hyperbolic length does not tend to zero, construct a uniform lower bound on [extremal length](../../../complex-analysis.md#extremal-length). On the unit square [torus](../../../topology.md#torus) choose a disk $D$ about the eventual slit centre and a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\chi$ equal to one on a smaller disk and supported in $D$. Let $x$ denote a local real coordinate on $D$; in the first term below, $dx$ is the globally defined torus one-form, while $\chi x$ is extended by zero outside $D$. The real [closed differential form](../../../differential-form.md#closed-differential-form)

$$
\alpha=dx-d(\chi x)
$$

is globally defined, vanishes on the smaller disk, and has period one on the horizontal generator. Pull it to $T_\delta$ by the rescaling map $z\mapsto z/\delta$, and extend it by zero across the slit and over the other [torus](../../../topology.md#torus). For sufficiently small $\delta$, the slit is inside the region where the form vanishes. Hence this extension $\alpha_\delta$ is a [smooth](../../../analysis.md#smooth-function) [closed differential form](../../../differential-form.md#closed-differential-form) on the [connected](../../../geometry-and-topology.md#connected-space) sum, with $\int_\gamma\alpha_\delta=1$.

Define a nonnegative [conformal metric](../../../complex-analysis.md#conformal-metric) density by the pointwise norm of $\alpha_\delta$ relative to the flat metric. Two-dimensional scale invariance gives

$$
A_\rho=\int|\alpha_\delta|^2\,dA=\int_{T_1}|\alpha|^2\,dA=:C<\infty,
$$

independently of $\delta$. For every representative $\widetilde\gamma$ [homotopic](../../../algebraic-topology.md#homotopy) to $\gamma$,

$$
\int_{\widetilde\gamma}\rho\,ds
\geq\left|\int_{\widetilde\gamma}\alpha_\delta\right|=1,
$$

because the period of a [closed differential form](../../../differential-form.md#closed-differential-form) is unchanged by homotopy. This is the [extremal length lower bound from a closed one-form](../../../complex-analysis.md#extremal-length-lower-bound-from-a-closed-one-form); therefore $\lambda(\gamma,X_\delta)\geq1/C>0$. If $\ell_{X_\delta}(\gamma)$ tended to zero along any subsequence, the collar estimate would force $\lambda(\gamma,X_\delta)\to0$, a contradiction. In fact its hyperbolic lengths are uniformly bounded away from zero. Thus

$$
\boxed{L(\gamma,|q_\delta|^{1/2})\to0
\quad\text{while}\quad
\inf_{\delta\text{ small}}\ell_{X_\delta}(\gamma)>0.}
$$

For every fixed $g>2$, replace $T_1$ by the area-one [translation surface](../../../complex-analysis.md#translation-surface) $X_{2g-2}$ constructed in the polygon argument; its [genus](../../../topology.md#genus-of-a-surface) is $g-1$. Cut its slit inside a nonsingular [flat coordinate](../../../complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) disk. The new connected sum has [genus](../../../topology.md#genus-of-a-surface) $g$, and the area normalization, small-handle length bound and closed-one-form energy argument are unchanged. Thus the converse fails at every fixed [genus](../../../topology.md#genus-of-a-surface) $g\geq2$.

<a id="4/b/image-a-small-translation-torus-joined-by-equal-slits-its-generator-is-flat-short-while-retaining-a-positive-extremal-length-bound"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132-shrinking-handle.png)

**[Figure 2](#4/b/image-a-small-translation-torus-joined-by-equal-slits-its-generator-is-flat-short-while-retaining-a-positive-extremal-length-bound). A small translation torus joined by equal slits; its generator is flat-short while retaining a positive extremal-length bound**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
