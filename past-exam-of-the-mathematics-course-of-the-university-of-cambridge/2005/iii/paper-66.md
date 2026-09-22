# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $B_j^n(t)=\binom njt^j(1-t)^{n-j}$ for the [Bernstein basis](../../../functional-analysis.md#bernstein-basis), and set $B_j^n=0$ when $j$ is outside its index range. Differentiating and using $j\binom nj=n\binom{n-1}{j-1}$ and $(n-j)\binom nj=n\binom{n-1}j$ gives

$$
\frac{d}{dt}B_j^n(t)=nB_{j-1}^{n-1}(t)-nB_j^{n-1}(t).
$$

Hence, after shifting the first sum by one index,

$$
\begin{aligned}
P'(t)&=n\sum_{j=0}^nP_jB_{j-1}^{n-1}(t)-n\sum_{j=0}^nP_jB_j^{n-1}(t)\\
&=n\sum_{j=0}^{n-1}(P_{j+1}-P_j)B_j^{n-1}(t).
\end{aligned}
$$

Thus **the [derivative](../../../calculus.md#derivative) is a degree-at-most-$(n-1)$ [Bézier curve](../../../numerical-analysis.md#bezier-curve) whose [control points](../../../numerical-analysis.md#control-point) are $n(P_{j+1}-P_j)$**. They are vectors rather than necessarily positions on the original [Bézier curve](../../../numerical-analysis.md#bezier-curve). This is the [Bézier derivative control polygon](../../../numerical-analysis.md#bezier-derivative-control-polygon).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Applying the preceding [derivative](../../../calculus.md#derivative) identity repeatedly yields the [Bézier derivative control polygon](../../../numerical-analysis.md#bezier-derivative-control-polygon) for every order:

$$
\boxed{P^{(r)}(t)=\frac{n!}{(n-r)!}\sum_{j=0}^{n-r}\Delta^rP_jB_j^{n-r}(t),\qquad0\le r\le n,}
$$

where the forward [finite difference](../../../finite-difference.md) is $\Delta P_j=P_{j+1}-P_j$ and

$$
\Delta^rP_j=\sum_{k=0}^r(-1)^{r-k}\binom rkP_{j+k}.
$$

The induction step multiplies by the remaining degree $n-r$ and takes one more [finite difference](../../../finite-difference.md). [Derivatives](../../../calculus.md#derivative) above order $n$ vanish. In particular,

$$
P^{(r)}(0)=\frac{n!}{(n-r)!}\Delta^rP_0,\qquad P^{(r)}(1)=\frac{n!}{(n-r)!}\Delta^rP_{n-r}.
$$

If the actual parameter interval has length $h$ and $t$ is its normalized coordinate, [derivatives](../../../calculus.md#derivative) in the original parameter acquire the additional factor $h^{-r}$. These formulas allow [derivative](../../../calculus.md#derivative) evaluation and join tests using only the [control polygon](../../../numerical-analysis.md#control-polygon).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Let the first [Bézier curve](../../../numerical-analysis.md#bezier-curve) have degree $n$ and [control points](../../../numerical-analysis.md#control-point) $P_0,\ldots,P_n$, and the next have degree $m$ and [control points](../../../numerical-analysis.md#control-point) $Q_0,\ldots,Q_m$. Use one increasing parameter on the two adjacent intervals. For a continuous join, their endpoints must agree: $P_n=Q_0$. If each interval has length $h$, the endpoint [derivatives](../../../calculus.md#derivative) are $n(P_n-P_{n-1})/h$ and $m(Q_1-Q_0)/h$. Therefore the [parametric first-derivative join of Bézier curves](../../../numerical-analysis.md#parametric-first-derivative-join-of-bezier-curves) is exactly

$$
\boxed{P_n=Q_0,\qquad n(P_n-P_{n-1})=m(Q_1-Q_0).}
$$

For equal degrees, the two polygon edges incident on the common endpoint are equal vectors. Equivalently, $P_{n-1},P_n=Q_0,Q_1$ are collinear with the join as their midpoint. Agreement of edge directions without these lengths gives only geometric tangent [continuity](../../../calculus.md#continuous-function) at a nonzero tangent, not equality of [derivatives](../../../calculus.md#derivative) in the chosen parameter. The displayed condition also covers zero endpoint [derivatives](../../../calculus.md#derivative). With unequal interval lengths $h,k$, the condition is instead $n(P_n-P_{n-1})/h=m(Q_1-Q_0)/k$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

A cubic [polynomial](../../../polynomial.md) on either half is determined by its endpoint positions and endpoint [derivatives](../../../calculus.md#derivative). Use normalized parameters $s=2t$ on the first half and $s=2t-1$ on the second, so that [derivatives](../../../calculus.md#derivative) with respect to $s$ are half the [derivatives](../../../calculus.md#derivative) with respect to $t$. Evaluation of the [Bernstein basis](../../../functional-analysis.md#bernstein-basis) at the split gives

$$
H=P(1/2)=\frac{P_0+3P_1+3P_2+P_3}{8},\qquad P'(1/2)=\frac34(-P_0-P_1+P_2+P_3).
$$

If the left [control points](../../../numerical-analysis.md#control-point) are $L_0,\ldots,L_3$, endpoint positions give $L_0=P_0,L_3=H$. The cubic endpoint-derivative formulas give $3(L_1-L_0)=P'(0)/2$ and $3(L_3-L_2)=P'(1/2)/2$. On the right, $R_0=H,R_3=P_3$, $3(R_1-R_0)=P'(1/2)/2$ and $3(R_3-R_2)=P'(1)/2$. Substitution yields

$$
\boxed{\begin{aligned}
(L_0,L_1,L_2,L_3)&=\left(P_0,\frac{P_0+P_1}{2},\frac{P_0+2P_1+P_2}{4},H\right),\\
(R_0,R_1,R_2,R_3)&=\left(H,\frac{P_1+2P_2+P_3}{4},\frac{P_2+P_3}{2},P_3\right).
\end{aligned}}
$$

These are exact restricted [Bézier curves](../../../numerical-analysis.md#bezier-curve), since they match all four endpoint Hermite data of the respective cubics.

The construction is also the midpoint case of [De Casteljau's algorithm](../../../numerical-analysis.md#de-casteljau-s-algorithm). Form $A_j=(P_j+P_{j+1})/2$ for $j=0,1,2$, then $B_0=(A_0+A_1)/2$, $B_1=(A_1+A_2)/2$, and $H=(B_0+B_1)/2$. The two polygons are $(P_0,A_0,B_0,H)$ and $(H,B_1,A_2,P_3)$. Their common tangent edges satisfy $H-B_0=B_1-H$, as required for equal half-intervals. Thus the triangular midpoint construction simultaneously evaluates the split point and supplies the two exact representations.

<a id="1/iv/image-midpoint-construction-and-the-two-exact-cubic-bezier-subcurves"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66-bezier-halves.png)

**[Figure 1](#1/iv/image-midpoint-construction-and-the-two-exact-cubic-bezier-subcurves). Midpoint construction and the two exact cubic Bézier subcurves**.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Put $U=B_0-A_0$, $T=D_0-C_0$, $D=A_0-C_0$ and $v=V-W$. A point on each moving segment has the form $A_0+sU+tV$ and $C_0+rT+tW$, with $s,r\in[0,1]$. Contact is therefore equivalent to

$$
D+sU-rT+tv=0,\qquad0\le s,r\le1,\quad t\ge0.
$$

The [contact time of translating line segments](../../../mathematical-optimization.md#contact-time-of-translating-line-segments) is the minimum feasible $t$. This reduces the entire continuous-motion problem to three [linear equations](../../../linear-algebra.md#linear-equation) and linear inequalities.

In three-dimensional space form the [matrix](../../../vector-space.md#matrix) $H=[U,-T,v]$. If it is nonsingular, solve

$$
\begin{pmatrix}s\\r\\t\end{pmatrix}=-H^{-1}D
$$

using a stable linear solver. A candidate with $s,r$ in the unit interval and $t\ge0$ is the only contact event and hence the earliest one; otherwise no contact occurs. Check initial intersection explicitly, so an already touching pair returns time zero.

If $H$ is singular, use a rank-revealing factorization to test consistency. Write every solution as $x=x_0+Nz$, with columns of $N$ spanning the [null space](../../../linear-algebra.md#kernel-of-a-linear-map), and minimize its time coordinate subject to the box and nonnegative-time constraints. This is a small [linear programming](../../../mathematical-optimization.md#linear-programming) problem. It handles parallel segments, collinear overlap, a continuum of contact times and segments degenerated to points. Infeasibility means no future contact. When $v=0$, the relative geometry is stationary: initially disjoint segments never meet. **The first contact is the least feasible nonnegative time, not just an intersection of the two supporting lines.**

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The same relative coordinates give the [proximity time of translating line segments](../../../mathematical-optimization.md#proximity-time-of-translating-line-segments) as

$$
\boxed{\min t\quad\text{subject to}\quad\|D+sU-rT+tv\|\le d,\quad0\le s,r\le1,\quad t\ge0.}
$$

This is a convex norm-constrained problem, rather than the linear feasibility problem for contact. One can solve it as a small [second-order cone](../../../mathematical-optimization.md#second-order-cone) problem. If the distance between the initial [line segments](../../../mathematical-optimization.md#line-segment) is at most $d$, the answer is zero; if no [feasible point](../../../mathematical-optimization.md#feasible-point) exists, the threshold is never reached.

For an elementary analytic algorithm, consider the nine combinations in which each of $s,r$ is either free, fixed at zero or fixed at one. In each case, minimize the squared distance over the free parameters. Writing $q(t)$ for $D+tv$ plus the fixed endpoint contributions, and $K$ for the columns belonging to free parameters, stationarity is

$$
K^T(Kz+q(t))=0.
$$

If the [Gram matrix](../../../linear-algebra.md#gram-matrix) $K^TK$ is nonsingular, $z(t)=-(K^TK)^{-1}K^Tq(t)$ is affine in time. Retain only the time interval on which its entries lie in $[0,1]$. The residual is then $r_0+tr_1$, and feasibility reduces to

$$
\|r_1\|^2t^2+2(r_0\cdot r_1)t+\|r_0\|^2-d^2\le0.
$$

Intersect its solution interval with $t\ge0$ and the free-parameter validity interval, and record the first point. Include the four endpoint–endpoint cases, where there are no unfixed segment parameters. Take the earliest valid candidate among all cases. The actual closest pair belongs to one of these faces of the parameter square, so this enumeration cannot miss the first approach.

The complications are the quadratic threshold equation, changes of the active closest-point feature and singular [Gram matrices](../../../linear-algebra.md#gram-matrix) for parallel or degenerate segments. In a singular case, keep the affine family of minimizers and its feasibility bounds, or use the original convex problem; a pseudoinverse answer alone can fall outside the segment even when another minimizer is feasible. Constant-distance cases and tangential threshold contact must also be retained. Merely checking moving endpoints misses approaches between interior points.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Fix the indexing convention

$$
P_i^{\ell+1}=\sum_jM_{i-aj}P_j^\ell,\qquad t_i^\ell=i/a^\ell,
$$

where the [subdivision arity](../../../numerical-analysis.md#subdivision-arity) $a>1$ is an [integer](../../../number-theory.md#integer). A change of the initial control $P_0^0$ can influence only indices $i=j_1$ after one step, where $M_{j_1}\ne0$. After $\ell$ steps the possible descendant indices are

$$
i=a^{\ell-1}j_1+a^{\ell-2}j_2+\cdots+j_\ell.
$$

Let $j_{\min},j_{\max}$ be the smallest and largest active [subdivision mask](../../../numerical-analysis.md#subdivision-mask) indices. Dividing by $a^\ell$ gives the enclosure

$$
\frac{j_{\min}}{a-1}(1-a^{-\ell})\le t_i^\ell\le\frac{j_{\max}}{a-1}(1-a^{-\ell}).
$$

Therefore the [support of a stationary subdivision scheme](../../../numerical-analysis.md#support-of-a-stationary-subdivision-scheme), in initial control-grid units, is enclosed by

$$
\boxed{\left[\frac{j_{\min}}{a-1},\frac{j_{\max}}{a-1}\right],\qquad\text{width }\frac{j_{\max}-j_{\min}}{a-1}.}
$$

For the stated symmetric [subdivision mask](../../../numerical-analysis.md#subdivision-mask) with active extremes $-w,w$, the width is $2w/(a-1)$. For a nonzero compactly supported basic limit function $\phi$, this is an exact endpoint calculation: its refinement equation is $\phi(x)=\sum_jM_j\phi(ax-j)$. If $\beta$ is its right support endpoint, only the largest active [subdivision mask](../../../numerical-analysis.md#subdivision-mask) index can contribute sufficiently close to the rightmost point of this sum; all smaller indices have argument beyond $\beta$. Hence $\beta=(\beta+j_{\max})/a$, giving $\beta=j_{\max}/(a-1)$. The left endpoint follows in the same way. This argument also excludes cancellation at an extreme for signed [subdivision masks](../../../numerical-analysis.md#subdivision-mask). The support for initial control $P_k$ is translated by $k$. If the nominal [subdivision mask](../../../numerical-analysis.md#subdivision-mask) was padded by zero coefficients, use its actual extremes; and a limiting [subdivision curve](../../../numerical-analysis.md#subdivision-curve) has to exist before its support is meaningful. This calculation describes the entire possible influence region, rather than the width of a single refinement stencil on its finer grid.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

There are no numerical [continuity](../../../calculus.md#continuous-function) bounds determined by $w$ and $a$ alone: the [subdivision mask](../../../numerical-analysis.md#subdivision-mask) coefficients matter. First check constant reproduction, $\sum_jM_{\epsilon-aj}=1$ for every residue $\epsilon$, and convergence. For the usual stationary [scalar](../../../vector-space.md#scalar) scheme, two useful calculations are a uniform contraction test and a spectral obstruction test. Higher smoothness is tested with derived difference [subdivision masks](../../../numerical-analysis.md#subdivision-mask).

Write $M(z)=\sum_jM_jz^j$ and $s_a(z)=1+z+\cdots+z^{a-1}$. Using backward differences $\Delta P_i=P_i-P_{i-1}$, the generating-function identity

$$
(1-z)M(z)=\frac{M(z)}{s_a(z)}(1-z^a)
$$

proves the [subdivision difference scheme](../../../numerical-analysis.md#subdivision-difference-scheme) relation $\Delta S_M=S_{M/s_a}\Delta$. Iterating gives $\Delta^rS_M=S_{M/s_a^r}\Delta^r$. To test a candidate $C^r$ limit, suppose the requisite sum rules hold, so $M/s_a^{r+1}$ is a finite [Laurent polynomial](../../../polynomial.md#laurent-polynomial). The scaled [derivative](../../../calculus.md#derivative) controls $q_i^\ell=a^{r\ell}\Delta^rP_i^\ell$ are refined by the [subdivision mask](../../../numerical-analysis.md#subdivision-mask)

$$
D_r(z)=a^r\frac{M(z)}{s_a(z)^r},
$$

whose residue sums are one. Their first differences are refined by

$$
B_r(z)=a^r\frac{M(z)}{s_a(z)^{r+1}}.
$$

The powers of $a$ are essential because each refinement shrinks parameter intervals by $a$.

**A lower [continuity](../../../calculus.md#continuous-function) bound comes from proving uniform contraction.** The infinity norm of one difference-refinement step is bounded by

$$
q=\max_{0\le\epsilon<a}\sum_j|(B_r)_{\epsilon-aj}|.
$$

If $q<1$, adjacent [derivative](../../../calculus.md#derivative) controls contract geometrically at every location. More generally, form the $p$-step [subdivision mask](../../../numerical-analysis.md#subdivision-mask)

$$
B_r^{[p]}(z)=\prod_{\nu=0}^{p-1}B_r(z^{a^\nu})
$$

and test $\max_{\epsilon\bmod a^p}\sum_j|(B_r^{[p]})_{\epsilon-a^pj}|<1$. This proves convergence of the constant-preserving [derivative](../../../calculus.md#derivative) scheme to a continuous limit. One justification is to compare consecutive piecewise-linear interpolants: their difference is bounded by a constant times the maximum adjacent-control difference, and the geometrically decreasing bound is summable. To identify the limit as $P^{(r)}$, use fixed-degree [Cardinal B-spline](../../../uniform-approximation.md#cardinal-b-spline) interpolants of the original refined controls. Their $r$th [derivatives](../../../calculus.md#derivative) are sums of the scaled [finite differences](../../../finite-difference.md); convergence of both functions and [derivatives](../../../calculus.md#derivative) gives $P\in C^r$. Testing successive $r$ supplies a guaranteed [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set).

**An upper [continuity](../../../calculus.md#continuous-function) bound comes from an observable noncontracting shape mode.** Build finite local [subdivision matrices](../../../numerical-analysis.md#subdivision-matrix) for $B_r$ on a refinement-invariant control neighborhood. For a digit $\epsilon$ their entries are $(A_\epsilon)_{ij}=(B_r)_{\epsilon+i-aj}$, since the new index is $ak+\epsilon+i$. Restrict to the realizable difference space and discard modes that do not affect the limit. A word $\epsilon_1,\ldots,\epsilon_p$ corresponds to a nested parameter location. If its product has an observable [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ with $|\lambda|>1$, repetition of this word makes some scaled [derivative](../../../calculus.md#derivative) differences grow rather than tend to zero. For a stable limit representation, $C^r$ regularity would force these differences to vanish; hence general-position data cannot have $C^r$ [continuity](../../../calculus.md#continuous-function). A modulus-one mode requires examination of whether it actually persists, rather than an automatic rounding rule.

The two calculations can be organized through the [joint spectral radius](../../../analysis.md#joint-spectral-radius) $\widehat\rho$ of these restricted [matrices](../../../vector-space.md#matrix):

$$
\boxed{\max_{|\epsilon|=p}\rho(A_{\epsilon_p}\cdots A_{\epsilon_1})^{1/p}\le\widehat\rho\le\max_{|\epsilon|=p}\|A_{\epsilon_p}\cdots A_{\epsilon_1}\|^{1/p}.}
$$

These [norm and spectral bounds for subdivision regularity](../../../numerical-analysis.md#norm-and-spectral-bounds-for-subdivision-regularity) make the test computable from the [subdivision mask](../../../numerical-analysis.md#subdivision-mask). The right bound certifies all-word contraction when it is less than one; the left bound detects a repeated-word obstruction when it exceeds one. Longer products improve the tests. A single [matrix](../../../vector-space.md#matrix)'s spectrum is not a substitute for controlling arbitrary products. The product estimates also appear in [Charina's analysis of subdivision regularity](https://arxiv.org/pdf/1202.2765); the strict contraction and observable-mode arguments above explain their respective roles.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A norm estimate controls the worst possible refined differences for every choice of the initial controls. Submultiplicativity turns a length-$p$ contraction into a bound for arbitrary long products, so it proves a certain number of continuous [derivatives](../../../calculus.md#derivative). Its [absolute values](../../../real-analysis.md#absolute-value) can lose cancellations; failure of the estimate is inconclusive. **It therefore gives a [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) on smoothness.**

Conversely, an observable eigenmode of a repeated local product exhibits a particular sequence of shrinking neighborhoods with inadequate decay. General-position controls have a nonzero coefficient in that mode, so greater [derivative](../../../calculus.md#derivative) [continuity](../../../calculus.md#continuous-function) is impossible. Special symmetric or [polynomial](../../../polynomial.md) data may suppress the bad mode; this is why the general-position qualification matters. **The obstruction gives an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) on smoothness, while failure to find an obstruction proves nothing.** A [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) on spectral growth becomes an [upper bound](../../../set.md#upper-bound-in-a-partially-ordered-set) on smoothness because large surviving differences correspond to rough behavior.

For example, the binary [Cardinal cubic B-spline](../../../uniform-approximation.md#cardinal-cubic-b-spline) [subdivision mask](../../../numerical-analysis.md#subdivision-mask) has symbol $M(z)=(1+z)^4/8$, up to an irrelevant index shift. At [derivative](../../../calculus.md#derivative) order $r=2$, the first-difference [subdivision mask](../../../numerical-analysis.md#subdivision-mask) is $B_2=(1+z)/2$, whose maximum parity sum is $1/2$: the limit is at least $C^2$. At $r=3$, $B_3=1$, and the surviving difference mode does not decay. For generic controls the third [derivative](../../../calculus.md#derivative) is piecewise constant with nonzero jumps, so the [subdivision curve](../../../numerical-analysis.md#subdivision-curve) is not $C^3$. Here the lower and upper tests determine the exact [integer](../../../number-theory.md#integer) [continuity](../../../calculus.md#continuous-function), but they need not coincide for an arbitrary [subdivision mask](../../../numerical-analysis.md#subdivision-mask). Stability, sum rules and borderline modes must be handled explicitly before interpreting any numerical estimate as a [continuity](../../../calculus.md#continuous-function) level.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis) is $b_{jk}(u,v)=\phi_j(u)\psi_k(v)$. If both univariate bases consist of [nonnegative functions](../../../function.md#nonnegative-function), then

$$
\boxed{b_{jk}(u,v)\ge0.}
$$

If both factors are strictly positive at the chosen parameters, their product is strictly positive there as well. Its support is the [Cartesian product](../../../set-theory.md#cartesian-product) of the two factor supports. With [partition of unity](../../../differential-geometry.md#partition-of-unity), this nonnegativity additionally places the [parametric surface](../../../differential-geometry.md#parametric-surface) point in the [convex hull](../../../mathematical-optimization.md#convex-hull) of the active [control points](../../../numerical-analysis.md#control-point).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

If each univariate basis sums to one, distribute the finite sums, or use local finiteness when the basis is infinite:

$$
\boxed{\sum_j\sum_kb_{jk}(u,v)=\left(\sum_j\phi_j(u)\right)\left(\sum_k\psi_k(v)\right)=1.}
$$

Thus the [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis) is a [partition of unity](../../../differential-geometry.md#partition-of-unity). In particular, translating every [control point](../../../numerical-analysis.md#control-point) by a fixed vector translates the [parametric surface](../../../differential-geometry.md#parametric-surface) by precisely that vector, and constant control data produce a constant [parametric surface](../../../differential-geometry.md#parametric-surface).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Suppose $\phi_j\in C^r$ in $u$ and $\psi_k\in C^s$ in $v$, including their respective knot joins. The mixed [derivatives](../../../calculus.md#derivative) of the [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis) are

$$
\boxed{\partial_u^p\partial_v^q b_{jk}(u,v)=\phi_j^{(p)}(u)\psi_k^{(q)}(v),\qquad p\le r,\ q\le s.}
$$

These are continuous because each factor is continuous. A finite or locally finite control sum has the same property. In the usual total-order notation the [parametric surface](../../../differential-geometry.md#parametric-surface) is therefore at least $C^{\min(r,s)}$, and also has the stronger stated rectangular set of continuous mixed [derivatives](../../../calculus.md#derivative). Across a $u$-knot its guaranteed order is $r$, and across a $v$-knot its guaranteed order is $s$. No general improvement over a factor's smoothness is possible: setting $P_{jk}=A_j$ and using $\sum_k\psi_k=1$ recovers the univariate curve $\sum_jA_j\phi_j(u)$ as a [parametric surface](../../../differential-geometry.md#parametric-surface) constant in $v$.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Let the univariate [linear precision](../../../numerical-analysis.md#linear-precision-of-a-geometric-basis) sites be $\xi_j,\eta_k$, meaning

$$
\sum_j\phi_j(u)=1,\quad\sum_j\xi_j\phi_j(u)=u,\qquad\sum_k\psi_k(v)=1,\quad\sum_k\eta_k\psi_k(v)=v.
$$

Then their Cartesian-product grid is a [linear precision](../../../numerical-analysis.md#linear-precision-of-a-geometric-basis) set for the [tensor-product surface basis](../../../differential-geometry.md#tensor-product-surface-basis):

$$
\sum_{j,k}(\xi_j,\eta_k)\phi_j(u)\psi_k(v)=(u,v).
$$

Indeed, the first coordinate is $(\sum_j\xi_j\phi_j)(\sum_k\psi_k)=u$, and the second is $(\sum_j\phi_j)(\sum_k\eta_k\psi_k)=v$. More generally, take controls $P_{jk}=A+\xi_jB+\eta_kC$. The resulting [parametric surface](../../../differential-geometry.md#parametric-surface) is exactly

$$
\boxed{P(u,v)=A+uB+vC.}
$$

This proves [linear precision of a geometric basis](../../../numerical-analysis.md#linear-precision-of-a-geometric-basis) and [affine map](../../../geometry-and-topology.md#affine-map) reproduction, including arbitrary changes of the embedding plane. In fact the products also reproduce the bilinear coordinate $uv$, since $\sum_{j,k}\xi_j\eta_k\phi_j\psi_k=uv$; affine precision is the requested consequence.

## 5

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The core [parametric surface interrogation](../../../differential-geometry.md#parametric-surface-interrogation) is evaluation of the position and its [derivatives](../../../calculus.md#derivative) through second order:

$$
\boxed{S(u,v),\quad S_u,S_v,\quad S_{uu},S_{uv},S_{vv}.}
$$

Position answers point queries; first [derivatives](../../../calculus.md#derivative) give the [differential](../../../differential-geometry.md#differential-of-a-smooth-map), tangent directions and [normal vector](../../../differential-geometry.md#normal-vector); [second derivatives](../../../calculus.md#second-derivative) supply [curvature](../../../differential-geometry.md#curvature). An evaluator should also report the parameter domain, patch adjacency, boundary curves and knot or crease locations, and whether these [derivatives](../../../calculus.md#derivative) exist at the queried point. At a discontinuity boundary it should provide the relevant [one-sided limits](../../../calculus.md#one-sided-limit) rather than silently average them.

For spatial searches, provide restriction or subdivision into equivalent smaller patches and certified [bounding volumes](../../../numerical-analysis.md#bounding-volume), with error estimates when an approximate mesh is used. These allow intersection and closest-point algorithms to reject remote patches and refine the remaining candidates. A useful interface therefore combines [differential](../../../differential-geometry.md#differential-of-a-smooth-map) evaluation with domain/topology and enclosure information. Inverse parameter lookup, ray intersection and nearest-point search can be built from these primitives using subdivision and local root or minimization solves; they need not be presumed exact basic evaluations of every representation.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Evaluate all quantities at $(u_0,v_0)$ and assume a [regular surface](../../../differential-geometry.md#smooth-surface) point, $S_u\times S_v\ne0$. The [tangent plane](../../../differential-geometry.md#tangent-plane) passes through $S_0=S(u_0,v_0)$ and is spanned by $S_u,S_v$. Thus

$$
\boxed{x=S_0+\alpha S_u+\beta S_v,\qquad (S_u\times S_v)\cdot(x-S_0)=0.}
$$

Choose the [unit normal](../../../differential-geometry.md#unit-normal) $n=(S_u\times S_v)/\|S_u\times S_v\|$. The [first fundamental form](../../../differential-geometry.md#first-fundamental-form) has coefficients

$$
E=S_u\cdot S_u,\qquad F=S_u\cdot S_v,\qquad G=S_v\cdot S_v,
$$

while the [second fundamental form](../../../second-fundamental-form.md) has coefficients

$$
e=n\cdot S_{uu},\qquad f=n\cdot S_{uv},\qquad g=n\cdot S_{vv}.
$$

To derive the [curvature](../../../differential-geometry.md#curvature) formula, differentiate $n\cdot S_u=n\cdot S_v=0$. This gives $-n_u\cdot S_u=e$, $-n_u\cdot S_v=f$, $-n_v\cdot S_u=f$ and $-n_v\cdot S_v=g$. Therefore the [shape operator](../../../second-fundamental-form.md#shape-operator) $-dn$, expressed in the tangent basis, is

$$
\begin{pmatrix}E&F\\F&G\end{pmatrix}^{-1}\begin{pmatrix}e&f\\f&g\end{pmatrix}.
$$

Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are the [principal curvatures](../../../second-fundamental-form.md#principal-curvature). Their product, the [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature), is its [determinant](../../../linear-algebra.md#determinant):

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}.}
$$

Regularity ensures $EG-F^2=\|S_u\times S_v\|^2>0$. Reversing $n$ changes the signs of $e,f,g$ and both [principal curvatures](../../../second-fundamental-form.md#principal-curvature) but leaves $K$ unchanged. At a singular parameter point this quotient and the cross-product [normal vector](../../../differential-geometry.md#normal-vector) are undefined; an alternative regular chart or separate geometric analysis is required.

## 6

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

A useful [subdivision curve interrogation](../../../numerical-analysis.md#subdivision-curve-interrogation) supplies the following connected capabilities. It describes the parameter interval, open or closed topology, endpoints and break points; it evaluates the limit point $C(t)$ and, where the scheme guarantees them, $C'(t)$ and $C''(t)$; and it refines or restricts an interval while retaining the mapping to the original parameter. It also provides enclosing bounds and a certified curve-to-chord error on each restricted piece. These are enough to build clipping, intersections, closest-point searches, tangents, [curvature](../../../differential-geometry.md#curvature) and adaptive sampling.

The enquiries concern the subdivision limit, not just a finite refined [control polygon](../../../numerical-analysis.md#control-polygon). For a stationary local refinement [matrix](../../../vector-space.md#matrix) $A$, a limit vertex can be obtained from a normalized [left eigenvector](../../../linear-operator-theory.md#left-eigenvector) $w^TA=w^T$, $w^T\mathbf1=1$, as $w^TP$. [Derivatives](../../../calculus.md#derivative) use the appropriately scaled difference schemes or equivalent spline evaluation on regular intervals. The convergence and [derivative](../../../calculus.md#derivative) hypotheses must actually hold for the scheme; no [second derivative](../../../calculus.md#second-derivative) can be requested at an intrinsic crease.

If the [subdivision mask](../../../numerical-analysis.md#subdivision-mask) is nonnegative and preserves constants, descendants and limit points lie in the relevant control-point [convex hull](../../../mathematical-optimization.md#convex-hull), giving a useful enclosing volume. For [subdivision masks](../../../numerical-analysis.md#subdivision-mask) with negative weights, that hull need not be an enclosure: the interface must supply another valid bound, for example from a proven refinement-error estimate. This distinction is important for safe spatial rejection in an algorithm.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

The corresponding [subdivision surface interrogation](../../../numerical-analysis.md#subdivision-surface-interrogation) needs mesh connectivity and patch adjacency, boundary and crease flags, local coordinate charts with transition maps, and subdivision into smaller patches with their original-chart mappings. Its evaluation enquiry returns a limit point, tangent [derivatives](../../../calculus.md#derivative) and a [normal vector](../../../differential-geometry.md#normal-vector); [second derivatives](../../../calculus.md#second-derivative) are supplied only where the limit is sufficiently smooth. Certified [bounding volumes](../../../numerical-analysis.md#bounding-volume) and patch approximation errors allow a hierarchy for intersection and proximity searches. Boundary-curve enquiries complete the interface for clipping.

On regular parts of a [subdivision surface](../../../numerical-analysis.md#subdivision-surface), these evaluations may use its equivalent tensor-product or [box spline](../../../uniform-approximation.md#box-spline) patch. Near an [extraordinary subdivision vertex](../../../numerical-analysis.md#extraordinary-subdivision-vertex), the local [subdivision matrix](../../../numerical-analysis.md#subdivision-matrix) determines the limit position through its constant [left eigenvector](../../../linear-operator-theory.md#left-eigenvector), and its tangent modes determine the [normal vector](../../../differential-geometry.md#normal-vector) under the scheme's [characteristic map of a subdivision surface](../../../numerical-analysis.md#characteristic-map-of-a-subdivision-surface) regularity conditions. Refinement alone does not establish those conditions. A [subdivision surface](../../../numerical-analysis.md#subdivision-surface) may have a well-defined [tangent plane](../../../differential-geometry.md#tangent-plane) there without possessing [second derivatives](../../../calculus.md#second-derivative) or [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature). An interrogation interface must distinguish these cases and can work on surrounding regular charts when a higher [derivative](../../../calculus.md#derivative) is unavailable at the vertex itself.

Together, subdivision, bounds, topology and limit evaluation support ray–[subdivision surface](../../../numerical-analysis.md#subdivision-surface) intersection: bounds eliminate irrelevant patches; surviving patches are refined, and regular candidate intersections are corrected using position and first [derivatives](../../../calculus.md#derivative). The returned intersection is a point of the limit [subdivision surface](../../../numerical-analysis.md#subdivision-surface) with an error certificate, rather than automatically a point on the last control mesh.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Let the point light be at $L$. For a [subdivision curve](../../../numerical-analysis.md#subdivision-curve) point $C(t)$, its projected shadow lies on the ray beyond the [subdivision curve](../../../numerical-analysis.md#subdivision-curve):

$$
R_t(\lambda)=L+\lambda(C(t)-L),\qquad\lambda>1.
$$

The shadow is the first intersection of that ray with the receiving [subdivision surface](../../../numerical-analysis.md#subdivision-surface) after the [subdivision curve](../../../numerical-analysis.md#subdivision-curve) point. Thus solve

$$
F(u,v,\lambda;t)=S(u,v)-L-\lambda(C(t)-L)=0
$$

and retain the smallest admissible $\lambda$. This is the defining equation for [shadow tracing for a subdivision curve](../../../numerical-analysis.md#shadow-tracing-for-a-subdivision-curve).

First organize the [subdivision surface](../../../numerical-analysis.md#subdivision-surface) patches into a [bounding volume hierarchy](../../../numerical-analysis.md#bounding-volume-hierarchy). For a restricted [subdivision curve](../../../numerical-analysis.md#subdivision-curve) interval, rays through its enclosing volume define an enclosing ray cone from $L$; [subdivision surface](../../../numerical-analysis.md#subdivision-surface) bounds that do not meet this cone can be rejected. Refine surviving [subdivision curve](../../../numerical-analysis.md#subdivision-curve) intervals and [subdivision surface](../../../numerical-analysis.md#subdivision-surface) patches. For a fixed $t$, isolate all possible ray intersections using those bounds, then correct each regular candidate with the [Jacobian matrix](../../../calculus.md#jacobian-matrix) for the [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization)

$$
J=[S_u,S_v,-(C(t)-L)].
$$

The [scalar triple product](../../../linear-algebra.md#scalar-triple-product) shows that $J$ is invertible exactly when $n\cdot(C(t)-L)\ne0$. Enforce the patch domain and $\lambda>1$ throughout correction, and choose the smallest valid $\lambda$. Bounds or validated root isolation, rather than a fixed list of [subdivision curve](../../../numerical-analysis.md#subdivision-curve) samples, are needed if every shadow component is to be found.

Once a regular intersection is known, follow it as $t$ changes. Differentiating $F=0$ gives a useful predictor:

$$
\boxed{J\begin{pmatrix}u'\\v'\\\lambda'\end{pmatrix}=\lambda C'(t),\qquad Q'(t)=S_u\,u'+S_v\,v'=\lambda C'(t)+\lambda'(C(t)-L).}
$$

Take a small predictor step in $(u,v,\lambda)$ and apply a [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization) correction at the new [subdivision curve](../../../numerical-analysis.md#subdivision-curve) parameter. Move through patch adjacency with its chart transition; shrink steps when [derivatives](../../../calculus.md#derivative) or error estimates change rapidly. Subdivide further and test a geometric curve-to-chord bound to approximate the resulting shadow trace to a chosen tolerance.

Surface-boundary crossings terminate or clip a trace. If a ray has no admissible [subdivision surface](../../../numerical-analysis.md#subdivision-surface) intersection, that [subdivision curve](../../../numerical-analysis.md#subdivision-curve) parameter contributes no shadow on $S$. At grazing contact the Jacobian is singular, so use interval subdivision and root isolation to detect the event and seed any outgoing branches. If several intersections are possible, recheck which is first; facing the light locally is helpful but is not a proof of global uniqueness. Open-curve endpoints and closed-curve seams must also be accounted for. With a compact represented geometry, transversal intersections and validated subdivision bounds, this algorithm traces every visible component; a purely sampled implementation gives only a tolerance-dependent approximation and cannot certify arbitrary tiny missed components.

For a directional light, replace the ray by $C(t)+\lambda d$ for a fixed propagation vector $d$ and $\lambda>0$. The intersection equation becomes $S-C-\lambda d=0$, with Jacobian $[S_u,S_v,-d]$ and continuation right-hand side $C'(t)$. The same enquiries and event handling apply.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
