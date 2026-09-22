# Paper 220

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_220.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_220.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
    - [iii](#3/d/iii)
      - [Solution](#3/d/iii/solution)
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

## 1

↑ **Parent:** [Paper 220](paper-220.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A compact [real tree](../../../topological-analysis.md#real-tree) is a compact [metric space](../../../topological-analysis.md#metric-space) $(T,d)$ such that any $x,y\in T$ are joined by a unique arc, and that arc is [isometric](../../../riemannian-geometry.md#isometry) to $[0,d(x,y)]$. The [multiplicity of a point in a real tree](../../../topological-analysis.md#multiplicity-of-a-point-in-a-real-tree) $a\in T$ is the number of [connected components](../../../geometry-and-topology.md#connected-component) of $T\setminus\{a\}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $s,t\in[0,1]$, define

$$
m_g(s,t)=\inf_{r\in[s\wedge t,s\vee t]}g(r),
\qquad
d_g(s,t)=g(s)+g(t)-2m_g(s,t).
$$

The function $d_g$ is a [pseudometric](../../../topological-analysis.md#pseudometric). Declare $s\sim t$ when $d_g(s,t)=0$, and give the [quotient set](../../../set-theory.md#quotient-set) $T_g=[0,1]/\!\sim$ the induced metric, again denoted $d_g$. This is the [real tree encoded by an excursion](../../../topological-analysis.md#real-tree-encoded-by-an-excursion) $g$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**False.** Join, at one common endpoint $o$, a [line segment](../../../mathematical-optimization.md#line-segment) of length $1/n$ for every positive [integer](../../../number-theory.md#integer) $n$, and use the intrinsic [path metric](../../../graph-theory.md#path-metric). This is a [real tree](../../../topological-analysis.md#real-tree). It is [totally bounded](../../../topological-analysis.md#totally-bounded-space), because outside the first finitely many arms every point lies arbitrarily close to $o$, and it is [complete](../../../topological-analysis.md#completeness); hence it is [compact](../../../topology.md#compact-space). Removing $o$ leaves one [connected component](../../../geometry-and-topology.md#connected-component) for every arm, so $o$ has countably infinite [multiplicity of a point in a real tree](../../../topological-analysis.md#multiplicity-of-a-point-in-a-real-tree).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**False.** Excursion coding does not remember the speed of traversal. Let $f$ be any nonzero coding function and let $\phi:[0,1]\to[0,1]$ be a nonidentity increasing [homeomorphism](../../../topology.md#homeomorphism). Set $g=f\circ\phi$. Then

$$
m_g(s,t)=m_f(\phi(s),\phi(t)),
\qquad
d_g(s,t)=d_f(\phi(s),\phi(t)).
$$

**Thus $[s]\mapsto[\phi(s)]$ induces an [isometry](../../../riemannian-geometry.md#isometry) $T_g\to T_f$, although generally $g\ne f$.**

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For nonempty compact subsets $A,B$ of a [metric space](../../../topological-analysis.md#metric-space) $(Z,d)$, the [Hausdorff distance](../../../topological-analysis.md#hausdorff-distance) is

$$
d_H^Z(A,B)=\max\left\{\sup_{a\in A}\inf_{b\in B}d(a,b),
\sup_{b\in B}\inf_{a\in A}d(a,b)\right\}.
$$

For compact [metric spaces](../../../topological-analysis.md#metric-space) $X,Y$, the [Gromov-Hausdorff distance](../../../topological-analysis.md#gromov-hausdorff-distance) is

$$
d_{GH}(X,Y)=\inf_{Z,\varphi,\psi}d_H^Z(\varphi(X),\psi(Y)),
$$

where $\varphi$ and $\psi$ range over [isometric embeddings](../../../riemannian-geometry.md#isometric-embedding) into a common [metric space](../../../topological-analysis.md#metric-space) $Z$.

The collection of compact [real trees](../../../topological-analysis.md#real-tree) is not compact in the [Gromov-Hausdorff topology](../../../topological-analysis.md#gromov-hausdorff-topology). Indeed, the intervals $T_n=[0,n]$ are compact real trees and

$$
|\operatorname{diam}(X)-\operatorname{diam}(Y)|\leq2d_{GH}(X,Y).
$$

Their diameters are unbounded, so $(T_n)$ has no convergent subsequence in the [Gromov-Hausdorff topology](../../../topological-analysis.md#gromov-hausdorff-topology).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Choose a root $o\in T$ and finite sets $F_n\subset T$ whose union is dense, arranging that $F_n$ is a $2^{-n}$-net and $F_n\subset F_{n+1}$. Let $T_n$ be the finite subtree spanned by $o$ and $F_n$. A depth-first contour traversal of $T_n$, recording distance from $o$, gives a continuous excursion $g_n$ whose [real tree encoded by an excursion](../../../topological-analysis.md#real-tree-encoded-by-an-excursion) is $T_n$.

The traversals may be chosen compatibly: when passing from $T_n$ to $T_{n+1}$, insert the new branch traversals into small time intervals at their attachment points. Since every new component has height at most $2^{-n+1}$, choose the time changes so that

$$
\lVert g_{n+1}-g_n\rVert_\infty\leq 2^{-n+2}.
$$

After harmlessly taking a faster sequence of nets, these errors are [summable](../../../real-analysis.md#summable-sequence). Hence $(g_n)$ is [Uniformly Cauchy](../../../real-analysis.md#uniformly-cauchy-sequence) and converges uniformly to a continuous $g:[0,1]\to\mathbb R_+$ with $g(0)=g(1)=0$.

The net property gives $d_{GH}(T_n,T)\to0$. By the stated continuity of excursion coding, $d_{GH}(T_{g_n},T_g)\to0$. Since $T_{g_n}$ is [isometric](../../../riemannian-geometry.md#isometry) to $T_n$, uniqueness of limits in the [Gromov-Hausdorff distance](../../../topological-analysis.md#gromov-hausdorff-distance) implies that $T_g$ is [isometric](../../../riemannian-geometry.md#isometry) to $T$. This proves the [excursion coding theorem for compact real trees](../../../topological-analysis.md#excursion-coding-theorem-for-compact-real-trees).

## 2

↑ **Parent:** [Paper 220](paper-220.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For $u\geq0$, let $\mathcal C_u$ be the collection of interval components of the [superlevel set](../../../topology.md#superlevel-set) $\{r:g(r)\geq u\}$. Two times $s,t$ lie in the same member of $\mathcal C_u$ exactly when $u\leq m_g(s,t)$. Therefore

$$
m_g(s,t)=\int_0^\infty\sum_{C\in\mathcal C_u}
\mathbf1_{\{s\in C\}}\mathbf1_{\{t\in C\}}\,du.
$$

For arbitrary real $\lambda_1,\ldots,\lambda_n$, the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) now gives

$$
\sum_{i,j}\lambda_i\lambda_jm_g(s_i,s_j)
=\int_0^\infty\sum_{C\in\mathcal C_u}
\left(\sum_{i:s_i\in C}\lambda_i\right)^2du\geq0.
$$

**Thus $(m_g(s_i,s_j))_{i,j}$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix).**

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The head of the [Brownian snake](../../../stochastic-process.md#brownian-snake) driven by $g$ is the centered [Gaussian process](../../../stochastic-process.md#gaussian-process) $(Z_t)_{0\leq t\leq1}$ with [covariance function](../../../stochastic-process.md#covariance-function) $\mathbb E[Z_sZ_t]=m_g(s,t)$. Part i shows that these [finite-dimensional distributions](../../../stochastic-process.md#finite-dimensional-distribution) exist consistently. Moreover,

$$
\mathbb E[(Z_t-Z_s)^2]
=g(s)+g(t)-2m_g(s,t)=d_g(s,t).
$$

If $g$ has Hölder constant $L$, then $d_g(s,t)\leq2L|t-s|^\alpha$. The [absolute moment](../../../probability-theory.md#absolute-moment) formula for a centered [normal distribution](../../../probability-theory.md#normal-distribution) consequently gives, for every $p\geq2$,

$$
\mathbb E|Z_t-Z_s|^p\leq C_{p,L}|t-s|^{\alpha p/2}.
$$

The [Kolmogorov continuity theorem](../../../stochastic-process.md#kolmogorov-continuity-theorem), with $p$ arbitrarily large, produces a modification that is $\gamma$-Hölder continuous for every $\gamma<\alpha/2$. Taking $\gamma=\alpha/2-\varepsilon$ proves the claim whenever $0<\varepsilon<\alpha/2$; for larger $\varepsilon$ the assertion is vacuous.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The set $\mathcal Q_n$ consists of [rooted planar maps](../../../graph-theory.md#rooted-planar-map) with $n$ faces, every face having degree four. The set $\mathcal Q_n^\bullet$ consists of these [quadrangulations](../../../graph-theory.md#planar-quadrangulation) with an additional distinguished vertex.

For the [trivial bijection between planar maps and quadrangulations](../../../graph-theory.md#trivial-bijection-between-planar-maps-and-quadrangulations), start from a rooted [planar map](../../../graph-theory.md#planar-map) with $n$ edges. Put a new vertex in every face and join it to the original vertex at every incident corner. Delete the original edges. The two endpoints of each deleted edge and the new vertices in its two adjacent faces bound a quadrangular face, so the result lies in $\mathcal Q_n$. Its bipartition distinguishes old from new vertices and reconstructs the original map. With the standard root convention this is a bijection, and hence

$$
\boxed{\#\mathcal Q_n=\#\mathcal M_n.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Consider an occurrence counted by $G_m$. Before the next counted occurrence, the exploration must first take a downward step of the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk), which has probability $1/2$, and then choose the decrement $-1$ among the three equally likely values of $\xi$, which has probability $1/3$. Thus it terminates the visits to the current record value with probability

$$
p=\frac12\frac13=\frac16.
$$

The [Strong Markov property](../../../markov-process.md#strong-markov-property) at successive counted occurrences makes these trials independent. Therefore $G_m$ has the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $\{1,2,\ldots\}$ with parameter $1/6$, and

$$
\boxed{\mathbb P(G_m\geq j)=\left(1-\frac16\right)^{j-1}}
$$

for every $j\geq1$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

In the standard labelled encoding of a pointed [planar quadrangulation](../../../graph-theory.md#planar-quadrangulation), incidences at the distinguished vertex are represented by visits counted by the record variables $G_m$. Consequently its [degree of a vertex](../../../graph-theory.md#degree-graph-theory) is bounded by the largest such count encountered before the coding walk first reaches $-1$.

Before time $2n+1$ there are at most $2n+1$ possible record levels. The [union bound](../../../probability-inequality.md#boole-s-inequality) and part i therefore imply

$$
\mathbb P\left(\max_mG_m\geq r,\ \sigma=2n+1\right)
\leq(2n+1)\left(\frac56\right)^{r-1}.
$$

Conditioning on $\sigma=2n+1$ and using the supplied lower bound gives

$$
\mathbb P\left(\deg(v^*)\geq r\mid\sigma=2n+1\right)
\leq C_0n^{5/2}\left(\frac56\right)^{r-1}.
$$

Set $r=C\log n$. If $C>5/(2\log(6/5))$, the right-hand side tends to zero. Hence for some constant $C>0$,

$$
\boxed{\mathbb P(\deg(v^*)\leq C\log n)\longrightarrow1}.
$$

## 3

↑ **Parent:** [Paper 220](paper-220.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded relatively closed set $A\subset\mathbb H$ for which $\mathbb H\setminus A$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique [conformal map](../../../geometry-and-topology.md#conformal-map) $g_A:\mathbb H\setminus A\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity)

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

Its [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is $\operatorname{hcap}(A)=a$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Set $h_A(z)=\operatorname{Im}(z-g_A(z))$. This is a nonnegative [harmonic function](../../../partial-differential-equation.md#harmonic-function) on $\mathbb H\setminus A$, has boundary value $\operatorname{Im}z$ on the hull boundary, and tends to zero on the real boundary. If $\tau$ is the first exit time of planar [Brownian motion](../../../brownian-motion.md) from $\mathbb H\setminus A$, the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
h_A(iy)=\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

The hydrodynamic expansion yields $h_A(iy)=\operatorname{hcap}(A)/y+O(y^{-2})$, and therefore the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity)

$$
\boxed{\operatorname{hcap}(A)=\lim_{y\to\infty}y\mathbb E_{iy}[\operatorname{Im}B_\tau]}.
$$

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

If $A\subseteq C$, Brownian motion exits $\mathbb H\setminus C$ no later than it exits $\mathbb H\setminus A$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) and the nonnegative harmonic function $h_A$ show that the expected exit height for $C$ is at least that for $A$. Taking the limits in the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) proves the [monotonicity of half-plane capacity](../../../stochastic-process.md#monotonicity-of-half-plane-capacity)

$$
\boxed{\operatorname{hcap}(A)\leq\operatorname{hcap}(C).}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

On $\mathbb H\setminus(A\cup C)$, the nonnegative [harmonic function](../../../partial-differential-equation.md#harmonic-function) $h_A+h_C$ dominates the boundary data $\operatorname{Im}z$ on $A\cup C$: at a point of $A$, for example, $h_A(z)=\operatorname{Im}z$ and $h_C(z)\geq0$. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions), or equivalently [Brownian motion](../../../brownian-motion.md) stopped on the union, gives

$$
h_{A\cup C}(z)\leq h_A(z)+h_C(z).
$$

Comparing the coefficients at infinity proves

$$
\boxed{\operatorname{hcap}(A\cup C)
\leq\operatorname{hcap}(A)+\operatorname{hcap}(C)}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

**False.** Let

$$
A_n=[-n,n]\times(0,n^{-2}].
$$

After filling bounded complementary components if necessary, this is a [compact H-hull](../../../stochastic-process.md#compact-h-hull) with diameter asymptotic to $2n$. The [half-plane capacity of a low rectangle](../../../stochastic-process.md#half-plane-capacity-of-a-low-rectangle) estimate, together with [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity), gives

$$
\operatorname{hcap}(A_n)=O(n^{-1})\longrightarrow0.
$$

**Thus unbounded diameter need not force unbounded capacity.**

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

**True.** The standard estimate [half-plane capacity is bounded by squared diameter](../../../stochastic-process.md#half-plane-capacity-is-bounded-by-squared-diameter) gives

$$
\operatorname{hcap}(A_n)\leq C\operatorname{diam}(A_n)^2.
$$

**Consequently $\operatorname{hcap}(A_n)\to\infty$ forces $\operatorname{diam}(A_n)\to\infty$.**

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Fix $x\in\mathbb R\setminus\{0\}$ and, before $x$ is swallowed, put $X_t=(g_t(x)-U_t)/\sqrt\kappa$. The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) and $U_t=\sqrt\kappa B_t$ show, after changing the sign of the Brownian motion, that

$$
dX_t=dW_t+\frac{2/\kappa}{X_t},dt.
$$

Thus $X$ is a [Bessel process](../../../brownian-motion.md#bessel-process) of dimension

$$
\delta=1+\frac4\kappa.
$$

A Bessel process hits zero exactly when $\delta<2$, which here is equivalent to $\kappa>4$. Hitting zero is precisely the swallowing of a nonzero boundary point by the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) hull. For $\kappa\leq4$ the trace is simple and swallows no such point; for $\kappa>4$ swallowing occurs through a boundary contact. Hence the trace intersects $\partial\mathbb H\setminus\{0\}$ exactly when $\kappa>4$.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

For $\kappa\leq4$, part i gives no nonzero boundary intersection. For $\kappa>4$, part i gives a boundary hit almost surely. After any hit, map out the past hull and recenter at the current tip. The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) says that the future is again an [SLE](../../../stochastic-process.md#schramm-loewner-evolution) in the remaining domain. Applying part i repeatedly and using [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) produces another boundary hit after every finite number of hits. Therefore there are almost surely infinitely many.

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

For $0<\kappa\leq4$, the trace meets the real boundary only at its starting point, so the intersection has zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Suppose $4<\kappa<8$. A boundary point swallowed by an interval need not itself lie on the trace. The stated fact that $\mathbb P(\tau_x=\tau_y)>0$ for $0<x<y$, combined with the [Strong Markov property](../../../markov-process.md#strong-markov-property) and [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) at successively nested swallowed intervals, implies that a fixed deterministic $x\ne0$ is swallowed in an interval rather than hit by the trace with probability one. Equivalently,

$$
\mathbb P\{x\in\gamma([0,\infty))\}=0.
$$

Applying the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) to the random indicator of the boundary trace gives

$$
\mathbb E\,\operatorname{Leb}\{x\in\mathbb R:x\in\gamma([0,\infty))\}
=\int_\mathbb R\mathbb P\{x\in\gamma([0,\infty))\}\,dx=0.
$$

The nonnegative random measure is therefore zero almost surely.

## 4

↑ **Parent:** [Paper 220](paper-220.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) states that, conditional on the hull $K_t$, the image under $g_t-U_t$ of the future hull has the same law as the original hull and is independent of the past.

For a [Loewner chain](../../../stochastic-process.md#loewner-chain) with continuous driver $U$, this property says that $U_{t+s}-U_t$ is independent of the past and has the same distribution as $U_s$. Thus $U$ has [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments). Every continuous process with those properties is a Brownian motion with drift, so $U_t=at+\sigma B_t$. Conformal scale invariance gives

$$
(r^{-1}U_{r^2t})_{t\geq0}\overset d=(U_t)_{t\geq0},
$$

which forces $a=0$. Writing $\kappa=\sigma^2$ yields

$$
\boxed{U_t=\sqrt\kappa B_t}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle) says the following. Let $D\subset\mathbb H$ be simply connected and agree with $\mathbb H$ in a neighborhood of $0$, and let $\psi:D\to\mathbb H$ be conformal with $\psi(0)=0$. The image under $\psi$ of an $\operatorname{SLE}_6$ in $\mathbb H$, stopped when it first leaves $D$, has the law of an $\operatorname{SLE}_6$ in $\mathbb H$, up to the corresponding stopping time and a change of [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

With the notation supplied in the question, $\widetilde U_t=\psi_t(U_t)$ and $dU_t=\sqrt\kappa\,dB_t$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and $\partial_t\psi_t(U_t)=-3\psi_t''(U_t)$ give

$$
d\widetilde U_t
=\sqrt\kappa\,\psi_t'(U_t)dB_t
+\left(\frac\kappa2-3\right)\psi_t''(U_t)dt.
$$

For $\kappa=6$, the [drift](../../../stochastic-calculus.md#drift-coefficient) vanishes. The resulting [continuous local martingale](../../../martingale.md#continuous-local-martingale) has [quadratic variation](../../../stochastic-calculus.md#quadratic-variation)

$$
d\langle\widetilde U\rangle_t
=6\psi_t'(U_t)^2dt
=3\,d\widetilde a(t).
$$

If $s=\widetilde a(t)/2$ is the usual half-plane-capacity time, then $\langle\widetilde U\rangle=6s$. The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) therefore gives

$$
\widetilde U_s=\sqrt6\,\widetilde B_s
$$

for a standard [Brownian motion](../../../brownian-motion.md) $\widetilde B$. The mapped hulls are consequently an $\operatorname{SLE}_6$, which proves locality.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Explore the two stopped curves in the opposite order. Begin with an $\operatorname{SLE}_6$ from $1$ to $\infty$, stopped on leaving $B(1,1)$, and then, in its unbounded complementary component, draw an $\operatorname{SLE}_6$ from $-1$ to $\infty$, stopped on leaving $B(-1,1)$. Before their respective stopping times, each curve is separated from the neighborhood in which the other hull changes the domain. The [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle) therefore says that mapping out the other stopped hull does not change either stopped marginal law.

The two exploration orders consequently define the same joint law for the pair of stopped hulls. Disintegrating this joint law with respect to the second curve shows that, conditional on $\gamma_2|_{[0,\tau_2]}$, the first curve is an $\operatorname{SLE}_6$ in the unbounded component of

$$
\mathbb H\setminus\gamma_2([0,\tau_2])
$$

from $-1$ to $\infty$, stopped when it leaves $B(-1,1)$, as required.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Choose a [Möbius transformation](../../../group-theory.md#mobius-transformation) of $\mathbb H$ that fixes $0$ and exchanges $x$ with $\infty$. By [Conformal invariance of SLE](../../../stochastic-process.md#conformal-invariance-of-sle), it transforms an $\operatorname{SLE}_6$ from $0$ to $x$ into one from $0$ to $\infty$. Until $x$ is disconnected from infinity, the discrepancy between the two target domains lies beyond the component visible from the growing tip. The [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle) therefore makes the two initial curve laws identical up to that disconnection time. Hence an $\operatorname{SLE}_6$ from $0$ to $x$, stopped at $\tau_x$, has the law of an $\operatorname{SLE}_6$ from $0$ to $\infty$ stopped when it disconnects $x$ from infinity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
