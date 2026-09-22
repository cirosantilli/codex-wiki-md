# Paper 339

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_339.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_339.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)

## 1

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [vector](../../../vector-space.md#vector) in the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant), the PDF's [matrix](../../../vector-space.md#matrix) gives the [quadratic form](../../../linear-algebra.md#quadratic-form)

$$
x^TAx=x_1^2+4x_1x_2+x_2^2\geq0.
$$

Thus it is a [copositive matrix](../../../linear-algebra.md#copositive-matrix). On the other hand, with $u=(1,-1)^T$,

$$
\boxed{u^TAu=-2<0},
$$

so it is not a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). Equivalently, the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $3$ and $-1$, with [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(1,1)^T$ and $(1,-1)^T$.

**The local TeX has corrupted the [matrix](../../../vector-space.md#matrix) entries**. The PDF has diagonal entries one and off-diagonal entries two. The all-twos [matrix](../../../vector-space.md#matrix) in the TeX would instead have [quadratic form](../../../linear-algebra.md#quadratic-form) $2(x_1+x_2)^2$ and would be a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix); it cannot demonstrate the requested distinction.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $x$ in the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant), the [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) $P$ satisfies $x^TPx\geq0$. The [nonnegative matrix](../../../vector-space.md#nonnegative-matrix) $N$ satisfies

$$
x^TNx=\sum_{i,j}N_{ij}x_ix_j\geq0,
$$

since every summand is nonnegative. Adding these inequalities proves

$$
\boxed{x^T(P+N)x\geq0\quad(x\geq0)}.
$$

Consequently $A=P+N$ is a [copositive matrix](../../../linear-algebra.md#copositive-matrix). The symmetry of $N$ follows from that of $A$ and $P$; entrywise nonnegativity alone need not imply [positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix).

This gives the inclusion of the [positive-semidefinite-plus-nonnegative cone](../../../mathematical-optimization.md#positive-semidefinite-plus-nonnegative-cone) in the [copositive cone](../../../mathematical-optimization.md#copositive-cone). It is only a sufficient construction; the argument does not claim that every [copositive matrix](../../../linear-algebra.md#copositive-matrix) has this decomposition in arbitrary [dimension](../../../vector-space.md#dimension-vector-space).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For each fixed $x$ in the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant), the map $A\mapsto x^TAx$ is a continuous [linear function](../../../vector-space.md#linear-function) on the [vector space](../../../vector-space.md) of real [symmetric matrices](../../../linear-algebra.md#symmetric-matrix). Thus

$$
K=\bigcap_{x\geq0}\{A:\langle A,xx^T\rangle_F\geq0\}
$$

is an intersection of [closed half-spaces](../../../mathematical-optimization.md#closed-half-space), using the [Frobenius inner product](../../../linear-algebra.md#frobenius-inner-product) $\langle A,B\rangle_F=\operatorname{tr}(AB)$ on this space. Arbitrary intersections of [closed sets](../../../topology.md#closed-set) are closed, so $K$ is closed.

If $A,B\in K$ and $s,t\geq0$, then $x^T(sA+tB)x=sx^TAx+tx^TBx\geq0$ for every $x\geq0$. Therefore $sA+tB\in K$, including the zero [matrix](../../../vector-space.md#matrix) when $s=t=0$. Hence

$$
\boxed{K\text{ is a closed convex cone}}.
$$

The [copositive cone](../../../mathematical-optimization.md#copositive-cone) is defined in the real space of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix); symmetry is needed later to recover every [matrix](../../../vector-space.md#matrix) entry from these [quadratic forms](../../../linear-algebra.md#quadratic-form).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A [pointed cone](../../../mathematical-optimization.md#pointed-cone) has no nonzero line through the origin: equivalently $K\cap(-K)=\{0\}$. If $A\in K\cap(-K)$, its [quadratic form](../../../linear-algebra.md#quadratic-form) vanishes on the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant). Testing the coordinate [vectors](../../../vector-space.md#vector) gives $A_{ii}=0$. Testing $e_i+e_j$ then gives

$$
0=(e_i+e_j)^TA(e_i+e_j)=2A_{ij}.
$$

Since $A$ is a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), every entry is zero. Thus $\boxed{K\cap(-K)=\{0\}}$.

The [identity matrix](../../../vector-space.md#identity-matrix) gives an [interior](../../../topology.md#interior-topology) point. For a symmetric perturbation $E$ with [operator norm](../../../continuous-dual-space.md#operator-norm) $\|E\|_2<1$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
x^T(I+E)x\geq(1-\|E\|_2)\|x\|_2^2>0\quad(x\ne0).
$$

This open [norm](../../../functional-analysis.md#norm) ball around $I$ lies even in the [positive semidefinite cone](../../../mathematical-optimization.md#positive-semidefinite-cone), hence in $K$. Consequently $\boxed{I\in\operatorname{int}K}$ and the [interior](../../../topology.md#interior-topology) is nonempty.

More generally, the [interior of the copositive cone](../../../mathematical-optimization.md#interior-of-the-copositive-cone) consists exactly of [strictly copositive matrices](../../../linear-algebra.md#strictly-copositive-matrix). Positivity on the [compact](../../../topology.md#compact-space) nonnegative [unit sphere](../../../topology.md#unit-sphere) has a positive minimum and persists under small perturbations; a zero there is destroyed by an arbitrarily small negative multiple of $I$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For a [convex cone](../../../mathematical-optimization.md#convex-cone) $D$ in an [inner product](../../../linear-algebra.md#inner-product) space, use the nonnegative-pairing convention

$$
D^*=\{B:\langle A,B\rangle\geq0\text{ for every }A\in D\}.
$$

Here the pairing is the [Frobenius inner product](../../../linear-algebra.md#frobenius-inner-product) on real [symmetric matrices](../../../linear-algebra.md#symmetric-matrix). Let $C_0$ be the [conic hull](../../../mathematical-optimization.md#conic-hull) of the nonnegative [rank-one matrices](../../../vector-space.md#rank-one-matrix) $xx^T$, and let $C=\overline{C_0}$. For $A\in K$, $\langle A,xx^T\rangle_F=x^TAx\geq0$. This extends to [conic combinations](../../../mathematical-optimization.md#conic-combination), and by [continuity](../../../calculus.md#continuous-function) to their limits. Hence $C\subseteq K^*$.

For the converse, if $B\notin C$, [separation from a closed convex cone](../../../mathematical-optimization.md#separation-from-a-closed-convex-cone) supplies a symmetric $H$ with

$$
\langle H,B\rangle_F<0,\qquad
\langle H,Z\rangle_F\geq0\quad(Z\in C).
$$

In particular $x^THx\geq0$ for every $x\geq0$, so $H\in K$. The negative pairing then excludes $B$ from $K^*$. Therefore

$$
\boxed{K^*=\overline{\operatorname{cone}\{xx^T:x\geq0\}}}.
$$

The same generator test gives $C^*=K$. This is the [duality of copositive and completely positive cones](../../../mathematical-optimization.md#duality-of-copositive-and-completely-positive-cones); the next argument removes the closure.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The real [vector space](../../../vector-space.md) of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) has [dimension](../../../vector-space.md#dimension-vector-space) $N=n(n+1)/2$. By the [conic Carathéodory theorem](../../../mathematical-optimization.md#conic-caratheodory-theorem), every member of $C_0$ is a [conic combination](../../../mathematical-optimization.md#conic-combination) of at most $N$ generators. Absorb each nonnegative [coefficient](../../../vector-space.md#coefficient) into its [vector](../../../vector-space.md#vector) through $\lambda xx^T=(\sqrt\lambda x)(\sqrt\lambda x)^T$.

If $B_\ell\in C_0$ converges to $B$, write, padding with zero [vectors](../../../vector-space.md#vector) if necessary,

$$
B_\ell=\sum_{j=1}^N x_{\ell j}x_{\ell j}^T,\qquad x_{\ell j}\geq0.
$$

The [matrix trace](../../../linear-algebra.md#matrix-trace) satisfies

$$
\operatorname{tr}B_\ell=\sum_{j=1}^N\|x_{\ell j}\|_2^2.
$$

The left side is bounded because $B_\ell$ converges. Thus the finite tuple $(x_{\ell1},\ldots,x_{\ell N})$ is bounded. The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives a subsequence on which every [vector](../../../vector-space.md#vector) converges, say $x_{\ell j}\to x_j\geq0$. [Continuity](../../../calculus.md#continuous-function) of the [outer product](../../../vector-space.md#outer-product) now gives $B=\sum_{j=1}^N x_jx_j^T\in C_0$. Hence

$$
\boxed{C_0\text{ is closed},\qquad K^*=C=C_0}.
$$

This proves [closedness of the completely positive cone](../../../mathematical-optimization.md#closedness-of-the-completely-positive-cone). The uniform bound on the number of factors and the [matrix trace](../../../linear-algebra.md#matrix-trace) bound are both essential: an arbitrary [conic hull](../../../mathematical-optimization.md#conic-hull) of a closed generating set need not be closed.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

Let $U=\{x\geq0:\|x\|_2=1\}$. This set is nonempty and [compact](../../../topology.md#compact-space) for $n\geq1$, and the [quadratic form](../../../linear-algebra.md#quadratic-form) is continuous. Its minimum $\alpha$ is therefore attained.

For every nonzero $y$ in the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant), normalizing $y$ gives

$$
y^T(Q-\lambda I)y
=\|y\|_2^2\left[\left(\frac y{\|y\|_2}\right)^T
Q\left(\frac y{\|y\|_2}\right)-\lambda\right].
$$

The zero [vector](../../../vector-space.md#vector) imposes no further condition. It follows that $Q-\lambda I$ is a [copositive matrix](../../../linear-algebra.md#copositive-matrix) exactly when $\lambda\leq\alpha$. Thus the feasible [scalar](../../../vector-space.md#scalar) set is $(-\infty,\alpha]$, and

$$
\boxed{\alpha=\max\{\lambda:Q-\lambda I\in K\}}.
$$

Both optima are attained. This [copositive reformulation of an orthant Rayleigh minimum](../../../convex-optimization.md#copositive-reformulation-of-an-orthant-rayleigh-minimum) follows directly from homogeneity; it does not require invoking a duality theorem for the original nonconvex constraint.

The restriction to $x\geq0$ matters. For the [matrix](../../../vector-space.md#matrix) in part (a), this minimum is $1$ whereas the unrestricted smallest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $-1$.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

For $X$ in the [dual cone](../../../toric-geometry.md#dual-cone) $C$, copositivity of $Q-\lambda I$ gives $\langle X,Q-\lambda I\rangle_F\geq0$. An upper-bounding [Lagrangian](../../../calculus-of-variations.md#lagrangian) for the maximization is therefore

$$
L(\lambda,X)=\lambda+\langle X,Q-\lambda I\rangle_F
=\langle Q,X\rangle_F+\lambda(1-\operatorname{tr}X).
$$

Its [supremum](../../../real-analysis.md#supremum) over unrestricted $\lambda$ is finite precisely when $\operatorname{tr}X=1$. Minimizing that upper bound gives the [conic program](../../../convex-optimization.md#conic-optimization)

$$
\boxed{\min_{X\in C}\ \langle Q,X\rangle_F
\quad\text{subject to }\operatorname{tr}X=1}.
$$

This is [completely positive optimization](../../../convex-optimization.md#completely-positive-optimization), not simply [semidefinite programming](../../../convex-optimization.md#semidefinite-programming): $C$ is the [completely positive cone](../../../mathematical-optimization.md#completely-positive-cone).

There is also a direct equality certificate. Every feasible $X=\sum_j u_ju_j^T$, $u_j\geq0$, has $\sum_j\|u_j\|_2^2=1$. Its objective is a weighted average of the nonnegative-sphere [Rayleigh quotients](../../../linear-operator-theory.md#rayleigh-quotient), hence is at least $\alpha$. For a minimizing unit [vector](../../../vector-space.md#vector) $x_*$ from part (g), $X_*=x_*x_*^T$ is feasible and has objective $\alpha$. Thus $\boxed{X_*=x_*x_*^T}$ attains the dual and both values agree, without relying on unverified regularity assumptions.

## 2

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Split the sign [vector](../../../vector-space.md#vector) as $x=(p^T,q^T)^T$. Multiplication of the two off-diagonal blocks gives

$$
x^TAx=\frac12(p^TSq+q^TS^Tp)=p^TSq,
$$

because the two terms are the same real [scalar](../../../vector-space.md#scalar). The map $(p,q)\mapsto x$ is a bijection between the feasible sign choices. Therefore

$$
\boxed{\max_{p,q}p^TSq=\max_x x^TAx}.
$$

This is the symmetric lifting of [bipartite binary quadratic optimization](../../../mathematical-optimization.md#bipartite-binary-quadratic-optimization) to [binary quadratic optimization](../../../mathematical-optimization.md#binary-quadratic-optimization). The factor $1/2$ is necessary: otherwise the two blocks would double the objective. No [positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix) of $A$ is assumed; generally its off-diagonal structure makes its [quadratic form](../../../linear-algebra.md#quadratic-form) indefinite.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Every feasible sign [vector](../../../vector-space.md#vector) gives the [rank-one matrix](../../../vector-space.md#rank-one-matrix) $X=xx^T$. It is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), since $u^TXu=(u^Tx)^2\geq0$, and $X_{ii}=x_i^2=1$. The [matrix trace](../../../linear-algebra.md#matrix-trace) identity gives

$$
\operatorname{tr}(Axx^T)=x^TAx.
$$

Thus all original feasible objectives appear among the relaxed ones, proving

$$
\boxed{p_{\rm SDP}^*\geq v^*}.
$$

The [semidefinite relaxation of binary quadratic optimization](../../../convex-optimization.md#semidefinite-relaxation-of-binary-quadratic-optimization) drops the rank-one requirement and keeps the [elliptope](../../../mathematical-optimization.md#elliptope) constraints.

An optimal relaxed [matrix](../../../vector-space.md#matrix) exists. The feasible set is nonempty, since it contains $I$, and closed. Its two-by-two [principal minors](../../../vector-space.md#principal-minor) give $|X_{ij}|^2\leq X_{ii}X_{jj}=1$, so it is bounded and therefore [compact](../../../topology.md#compact-space). The linear objective attains its maximum. Also $\operatorname{tr}(AI)=0$ and hence $p_{\rm SDP}^*\geq0$, including the zero-objective case.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write a test [vector](../../../vector-space.md#vector) as $(u,v)$ and put $s=\sum_i u_i$, $t=\sum_jv_j$. Its [quadratic form](../../../linear-algebra.md#quadratic-form) against the block-constant [matrix](../../../vector-space.md#matrix) is

$$
a(s^2+t^2)+2bst.
$$

Since $a\geq|b|$, both $a$ and $a-|b|$ are nonnegative, and

$$
a(s^2+t^2)+2bst\geq a(s^2+t^2)-2|b||st|
\geq(a-|b|)(s^2+t^2)\geq0.
$$

Equivalently it is

$$
\frac{a+b}{2}(s+t)^2+\frac{a-b}{2}(s-t)^2.
$$

Therefore the [bipartite block-constant positive semidefinite matrix](../../../linear-algebra.md#bipartite-block-constant-positive-semidefinite-matrix) satisfies $\boxed{\begin{pmatrix}aJ_{n,n}&bJ_{n,m}\\bJ_{m,n}&aJ_{m,m}\end{pmatrix}\succeq0}$.

For positive block sizes, the condition is also necessary: choose $s=t$ and $s=-t$ to obtain $a+b\geq0$ and $a-b\geq0$. Equality is allowed, and [vectors](../../../vector-space.md#vector) whose sums vanish in both blocks lie in the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). [Positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix), rather than positive definiteness, is the conclusion.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For each [coefficient](../../../vector-space.md#coefficient) index $k\geq0$, let $H_k$ have constant diagonal blocks $f_kJ$ and cross blocks $g_kJ$. The preceding block-constant argument gives $H_k\succeq0$. Define the [Hadamard powers](../../../vector-space.md#hadamard-power) $X^{\circ k}$, with

$$
X^{\circ0}=J_{n+m,n+m}.
$$

This is the constant entrywise power, including at zero entries; it is not the [identity matrix](../../../vector-space.md#identity-matrix). Repeated use of the [Schur product theorem](../../../linear-algebra.md#schur-product-theorem) shows $X^{\circ k}\succeq0$ for every $k\geq0$.

Applying the [Schur product theorem](../../../linear-algebra.md#schur-product-theorem) again makes every summand $H_k\circ X^{\circ k}$ [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix). The partial sums are [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix), and their entrywise limit is exactly $Y$. In finite [dimension](../../../vector-space.md#dimension-vector-space) this is a matrix-norm limit; the [positive semidefinite cone](../../../mathematical-optimization.md#positive-semidefinite-cone) is closed. Consequently

$$
\boxed{Y=\sum_{k=0}^\infty H_k\circ X^{\circ k}\succeq0}.
$$

Endpoint convergence follows from the stated expansions on the full interval: $f_k\geq0$ and $\sum f_k=f(1)<\infty$, while $\sum|g_k|\leq\sum f_k$. Thus the expansions converge absolutely at every [matrix](../../../vector-space.md#matrix) entry. This is [coefficient-dominated entrywise positivity](../../../linear-algebra.md#coefficient-dominated-entrywise-positivity).

**The [coefficient](../../../vector-space.md#coefficient) condition must include index zero**. We interpret the PDF's $\mathbb N$ accordingly. If it means only positive integers and no condition is imposed on $f_0,g_0$, the assertion is false: take $n=m=1$, $X=0$, $f=-1$ and $g=0$. All positive-index inequalities hold, but $Y=-I_2$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Put $t=\log(1+\sqrt2)=\operatorname{arsinh}(1)$, so $c_K=2t/\pi$. The [power series](../../../real-analysis.md#power-series) [coefficients](../../../vector-space.md#coefficient) of the [hyperbolic sine](../../../calculus.md#hyperbolic-sine) preprocessing are

$$
f_{2k}=g_{2k}=0,\qquad
f_{2k+1}=\frac{t^{2k+1}}{(2k+1)!},\qquad
g_{2k+1}=(-1)^kf_{2k+1}.
$$

Thus $f_j=|g_j|$ for every $j\geq0$, and the series converge on the full interval. Applying [coefficient-dominated entrywise positivity](../../../linear-algebra.md#coefficient-dominated-entrywise-positivity) gives $Y\succeq0$.

Every diagonal entry belongs to one of the diagonal blocks and equals $f(X_{ii})=f(1)=\sinh t$. Because $e^t=1+\sqrt2$ and $e^{-t}=\sqrt2-1$, this is $(e^t-e^{-t})/2=1$. Therefore

$$
\boxed{Y\succeq0,\qquad Y_{ii}=1}.
$$

The [matrix](../../../vector-space.md#matrix) lies in the [elliptope](../../../mathematical-optimization.md#elliptope) and admits a [Gram matrix](../../../linear-algebra.md#gram-matrix) representation by unit [vectors](../../../vector-space.md#vector). This preprocessing is the [Krivine rounding scheme](../../../mathematical-optimization.md#krivine-rounding-scheme); the equality of absolute [coefficients](../../../vector-space.md#coefficient) is what preserves [positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix) even though the cross-block [sine](../../../geometry-and-topology.md#sine) [coefficients](../../../vector-space.md#coefficient) alternate in sign.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The [Gram matrix](../../../linear-algebra.md#gram-matrix) representation and $Y_{ii}=1$ give $\|v_i\|_2=1$. For a [standard Gaussian random vector](../../../probability-and-statistics.md#standard-gaussian-random-vector) $Z$, each $\langle v_i,Z\rangle$ is a standard [normal](../../../probability-theory.md#normal-distribution) [scalar](../../../vector-space.md#scalar), so the zero event has [probability](../../../probability-theory.md#probability) zero. Choose either sign convention at zero; the resulting [vector](../../../vector-space.md#vector) is [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) a feasible sign [vector](../../../vector-space.md#vector). Consequently $y^TAy\leq v^*$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

The [Gaussian sign-correlation identity](../../../probability-and-statistics.md#gaussian-sign-correlation-identity) gives

$$
\mathbb E[y^TAy]
=\sum_{i,j}A_{ij}\mathbb E[y_iy_j]
=\frac2\pi\sum_{i,j}A_{ij}\arcsin(Y_{ij})
=\frac2\pi\operatorname{tr}(A\arcsin[Y]).
$$

The last equality uses symmetry of the real [matrices](../../../vector-space.md#matrix). Hence

$$
\boxed{v^*\geq\mathbb E[y^TAy]
=\frac2\pi\operatorname{tr}(A\arcsin[Y])}.
$$

The [inverse sine](../../../geometry-and-topology.md#inverse-sine) is applied entrywise, not through [spectral matrix functional calculus](../../../hilbert-space.md#spectral-matrix-functional-calculus).

For completeness, the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) identity has a geometric proof. If the angle between two unit [vectors](../../../vector-space.md#vector) is $\theta$, the isotropic [Gaussian random vector](../../../probability-and-statistics.md#gaussian-random-vector) direction in their two-dimensional span gives opposite signs on angular sectors with [probability](../../../probability-theory.md#probability) $\theta/\pi$. Thus the sign product has [expectation](../../../probability-theory.md#expected-value) $1-2\theta/\pi=(2/\pi)\arcsin(\cos\theta)$. Parallel and antiparallel pairs give the endpoint values $1$ and $-1$ directly. This is [Gaussian hyperplane rounding](../../../mathematical-optimization.md#gaussian-hyperplane-rounding), and needs no [independence](../../../random-variable.md#independent-random-variables) between the rounded coordinates.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

The [Krivine rounding constant](../../../mathematical-optimization.md#krivine-rounding-constant) has $t=c_K\pi/2=\log(1+\sqrt2)<\pi/2$. Since $|X_{ij}|\leq1$, the principal real [inverse sine](../../../geometry-and-topology.md#inverse-sine) satisfies

$$
\arcsin(\sin(tX_{ij}))=tX_{ij}
$$

on every cross-block entry. The [matrix](../../../vector-space.md#matrix) $A$ has zero diagonal blocks, so those cross blocks are the only contributors to its [Frobenius inner product](../../../linear-algebra.md#frobenius-inner-product) with $\arcsin[Y]$. Explicitly,

$$
\operatorname{tr}(A\arcsin[Y])
=\sum_{i=1}^n\sum_{j=1}^mS_{ij}\arcsin(g(X_{i,n+j}))
=t\sum_{i,j}S_{ij}X_{i,n+j}
=t\operatorname{tr}(AX).
$$

No analogous identity is needed for the diagonal blocks involving $\sinh$.

Combining with the preceding [expectation](../../../probability-theory.md#expected-value) formula and optimality of $X$ gives the [bipartite sign rounding bound](../../../mathematical-optimization.md#bipartite-sign-rounding-bound)

$$
\boxed{c_Kp_{\rm SDP}^*\leq v^*\leq p_{\rm SDP}^*},\qquad
\boxed{c_K=\frac2\pi\log(1+\sqrt2)=0.56109985\ldots}.
$$

At least one feasible rounded outcome attains at least this [expectation](../../../probability-theory.md#expected-value). This is an expectation-based approximation guarantee for the specific bipartite sign problem; no claim is made that $c_K$ is the largest possible constant. The inequalities remain valid when the optimal objective is zero.

## 3

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

On the [unit circle](../../../complex-analysis.md#complex-unit-circle), $z^{-1}=\overline z$, so

$$
p(z)=2+z+\overline z=(1+z)(1+\overline z)=|1+z|^2.
$$

Thus the [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) is nonnegative, with a zero at $z=-1$, and

$$
\boxed{q(z)=1+z,\qquad p(z)=|q(z)|^2\quad(|z|=1)}.
$$

Equivalently, writing $z=e^{i\theta}$ gives $p(z)=2+2\cos\theta=4\cos^2(\theta/2)$. The factor has [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) one as required. Multiplication of $q$ by any constant of modulus one leaves the factorization unchanged; uniqueness of $q$ is not claimed.

This is the simplest instance of the [Fejér–Riesz theorem](../../../fourier-series.md#fejer-riesz-theorem), where nonnegativity of a [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) on the [unit circle](../../../complex-analysis.md#complex-unit-circle) admits a [polynomial](../../../polynomial.md) modulus-square factorization.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Since $p$ is real on the [unit circle](../../../complex-analysis.md#complex-unit-circle),

$$
\sum_{k=-d}^dp_kz^k
=\overline{p(z)}
=\sum_{k=-d}^d\overline{p_k}z^{-k}
=\sum_{k=-d}^d\overline{p_{-k}}z^k.
$$

Multiply the difference by $z^d$. It is an ordinary [polynomial](../../../polynomial.md) of [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) at most $2d$ vanishing at every point of the [unit circle](../../../complex-analysis.md#complex-unit-circle). A nonzero [polynomial](../../../polynomial.md) has only finitely many [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), so all its [coefficients](../../../vector-space.md#coefficient) vanish. This proves the [conjugate symmetry of trigonometric polynomial coefficients](../../../fourier-series.md#conjugate-symmetry-of-trigonometric-polynomial-coefficients):

$$
\boxed{p_{-k}=\overline{p_k}\quad(0\leq k\leq d)}.
$$

For arbitrary nonzero complex $z$, [coefficient](../../../vector-space.md#coefficient) substitution now gives precisely

$$
\boxed{p(z^{-1})=\overline{p(\overline z)}}.
$$

Equivalently $p(1/\overline z)=\overline{p(z)}$. The [complex conjugation](../../../complex-analysis.md#complex-conjugation) on the right applies to the whole value, including the [coefficients](../../../vector-space.md#coefficient); it cannot simply be discarded away from the circle.

The PDF additionally assumes $p_d\ne0$. Then $p_{-d}=\overline{p_d}\ne0$, so the ensuing [polynomial](../../../polynomial.md) $P=z^dp$ has [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) exactly $2d$ and nonzero constant term. These clauses and this subpart are absent from the damaged TeX, but present in the PDF.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For $z\ne0$, the [coefficient](../../../vector-space.md#coefficient) symmetry yields

$$
z^{2d}\overline{P(1/\overline z)}
=z^{2d}\overline{(1/\overline z)^dp(1/\overline z)}
=z^dp(z)=P(z).
$$

Thus $P$ equals its reversed-conjugate [polynomial](../../../polynomial.md). If $\zeta\ne0$ is a [root of a polynomial](../../../polynomial.md#root-of-a-polynomial), with $P(\zeta)=0$, this identity gives $P(1/\overline\zeta)=0$, proving

$$
\boxed{\zeta\text{ a root}\ \Longrightarrow\ 1/\overline\zeta\text{ a root}}.
$$

The [reciprocal-conjugate root pairing](../../../fourier-series.md#reciprocal-conjugate-root-pairing) also preserves the [multiplicity of a root](../../../polynomial.md#multiplicity-of-a-root): reversal and [complex conjugation](../../../complex-analysis.md#complex-conjugation) take each factor associated with $\zeta$ to the corresponding factor associated with $1/\overline\zeta$, with the same exponent.

Since $P(0)=p_{-d}\ne0$, no zero [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) occurs, so the reciprocal operation is always defined on the [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial). Roots off the [unit circle](../../../complex-analysis.md#complex-unit-circle) are paired on opposite sides of it; [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) on the [unit circle](../../../complex-analysis.md#complex-unit-circle) are fixed by this operation. Pairing alone does not force even multiplicity at those fixed [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial); that extra fact uses nonnegativity.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Pair the off-circle [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) using [reciprocal-conjugate root pairing](../../../fourier-series.md#reciprocal-conjugate-root-pairing), and split each unit-circle [root of a polynomial](../../../polynomial.md#root-of-a-polynomial)'s even multiplicity equally between the two members of a pair. The [fundamental theorem of algebra](../../../algebra.md#fundamental-theorem-of-algebra) and the leading [coefficient](../../../vector-space.md#coefficient) $p_d$ give $P(z)=p_d\prod_{i=1}^d(z-\zeta_i)(z-1/\overline{\zeta_i})$. None of the selected $\zeta_i$ is zero.

On the [unit circle](../../../complex-analysis.md#complex-unit-circle), the identity

$$
z-\frac1{\overline{\zeta_i}}
=-\frac z{\overline{\zeta_i}}(\overline z-\overline{\zeta_i})
$$

turns $P(z)/z^d$ into

$$
p(z)=c\prod_{i=1}^d(z-\zeta_i)(\overline z-\overline{\zeta_i})
=c\prod_{i=1}^d|z-\zeta_i|^2,\qquad
c=\frac{(-1)^dp_d}{\prod_i\overline{\zeta_i}}.
$$

At a point of the [unit circle](../../../complex-analysis.md#complex-unit-circle) outside the finite set of [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), the product is positive and $p(z)$ is nonzero and nonnegative. Its ratio to the product is therefore real and strictly positive. This proves $c>0$, even though the algebraic expression initially permits a complex constant. Consequently

$$
\boxed{q(z)=\sqrt c\prod_{i=1}^d(z-\zeta_i),\qquad
p(z)=|q(z)|^2\quad(|z|=1)}.
$$

This proves the [Fejér–Riesz theorem](../../../fourier-series.md#fejer-riesz-theorem) for a nonzero [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) of actual order $d$. A positive constant has a constant square-root factor, and the identically zero [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) has $q=0$; if $p_d=0$ for a specified upper order $d$, reduce to the actual order first.

Although the PDF permits assuming even multiplicity, there is a short proof of [even multiplicity of unit-circle roots of a nonnegative trigonometric polynomial](../../../fourier-series.md#even-multiplicity-of-unit-circle-roots-of-a-nonnegative-trigonometric-polynomial). The [real analytic](../../../analysis.md#real-analytic-function) function $p(e^{i\theta})\geq0$ cannot have a zero of odd order. Near $\zeta=e^{i\theta_0}$, $e^{i\theta}-\zeta$ has a simple zero, and the nonzero factor $e^{-id\theta}$ leaves the zero order of $P(e^{i\theta})$ unchanged. Hence the [multiplicity of a root](../../../polynomial.md#multiplicity-of-a-root) must be even.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Collect the factor's [coefficients](../../../vector-space.md#coefficient) in the column [vector](../../../vector-space.md#vector) $q=(q_0,\ldots,q_d)^T$ and set

$$
\boxed{M=qq^*,\qquad M_{ij}=q_i\overline{q_j}}.
$$

This is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) and a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), because for every complex [vector](../../../vector-space.md#vector) $x$,

$$
x^*Mx=|q^*x|^2\geq0.
$$

On the [unit circle](../../../complex-analysis.md#complex-unit-circle), expanding the modulus square gives

$$
|q(z)|^2=\sum_{i,j=0}^d q_i\overline{q_j}z^{i-j}.
$$

Uniqueness of the finite [Laurent polynomial](../../../polynomial.md#laurent-polynomial) [coefficients](../../../vector-space.md#coefficient), proved as in part (b)(i), therefore gives

$$
\boxed{p_k=\sum_{\substack{0\leq i,j\leq d\\i-j=k}}M_{ij}}.
$$

This is the [rank-one spectral-factor Gram matrix](../../../fourier-series.md#rank-one-spectral-factor-gram-matrix). The [matrix](../../../vector-space.md#matrix) $M$ has [matrix rank](../../../vector-space.md#matrix-rank) one when $q\ne0$ and zero when $q=0$. The orientation $i-j=k$ is the PDF's convention: using $\overline{q_i}q_j$ instead would generally interchange $p_k$ and $p_{-k}$.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

For $z$ on the [unit circle](../../../complex-analysis.md#complex-unit-circle), use the conjugated monomial [vector](../../../vector-space.md#vector)

$$
w(z)=(1,z^{-1},\ldots,z^{-d})^T
=(1,\overline z,\ldots,\overline z^{\,d})^T.
$$

Then the prescribed diagonal sums give

$$
w(z)^*Mw(z)=\sum_{i,j=0}^dM_{ij}z^{i-j}
=\sum_{k=-d}^d p_kz^k=p(z).
$$

[Positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix) proves

$$
\boxed{p(z)=w(z)^*Mw(z)\geq0\quad(|z|=1)}.
$$

This is the [Gram matrix representation of a trigonometric polynomial](../../../fourier-series.md#gram-matrix-representation-of-a-trigonometric-polynomial). The Hermitian condition also implies $p_{-k}=\overline{p_k}$, so its values on the [unit circle](../../../complex-analysis.md#complex-unit-circle) are real. The conjugated monomial [vector](../../../vector-space.md#vector) is required by the source's $i-j=k$ convention; the unconjugated [vector](../../../vector-space.md#vector) would represent $p(z^{-1})$ instead.

In particular $p_0=\operatorname{tr}M\geq0$. If this [matrix trace](../../../linear-algebra.md#matrix-trace) is zero, all nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) vanish and $M=0$, so $p=0$. A general feasible [Gram matrix](../../../linear-algebra.md#gram-matrix) need not have [matrix rank](../../../vector-space.md#matrix-rank) one; the [Fejér–Riesz theorem](../../../fourier-series.md#fejer-riesz-theorem) ensures a rank-one representative exists whenever the nonnegative [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) is nonzero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
