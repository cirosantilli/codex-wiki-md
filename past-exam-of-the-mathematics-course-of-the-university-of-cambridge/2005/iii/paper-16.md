# Paper 16

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper16.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper16.pdf)

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
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)

## 1

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [fixed point](../../../function.md#fixed-point) of the [left shift](../../../dynamical-systems.md#left-shift) satisfies $x_{k+1}=x_k$ for every $k\in\mathbb Z$, so its entire two-sided [sequence](../../../real-analysis.md#sequence) is constant. The constant [sequence](../../../real-analysis.md#sequence) with value $i$ belongs to the [subshift of finite type](../../../dynamical-systems.md#subshift-of-finite-type) precisely when $A_{ii}=1$: this is exactly the requirement that its repeated transition be allowed by the [symbolic transition matrix](../../../dynamical-systems.md#transition-matrix-for-a-subshift). There is one such [fixed point](../../../function.md#fixed-point) for each diagonal entry equal to one. Thus

$$
\boxed{\#\operatorname{Fix}(\sigma)=\sum_{i=1}^m A_{ii}=\operatorname{tr}A.}
$$

This also covers an empty [subshift of finite type](../../../dynamical-systems.md#subshift-of-finite-type), for then no permitted constant [sequence](../../../real-analysis.md#sequence) exists.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $W_n(i,j)$ for the number of [locally admissible words](../../../dynamical-systems.md#locally-admissible-word-for-a-transition-matrix) $(x_0,\ldots,x_n)$ with $x_0=i$ and $x_n=j$. Here local admissibility means $A_{x_rx_{r+1}}=1$ for each consecutive pair; length counts symbols, so there are $n$ transitions. For $n=0$, the single-symbol word gives $W_0(i,j)=\delta_{ij}=(A^0)_{ij}$, and for $n=1$ we have $W_1(i,j)=A_{ij}$.

To append the last symbol $j$, choose the penultimate symbol $k$. Every choice gives a [locally admissible word](../../../dynamical-systems.md#locally-admissible-word-for-a-transition-matrix) exactly when its length-$n$ prefix is locally admissible and $A_{kj}=1$. Different prefixes or penultimate symbols give different words, and every admissible word is obtained once. Therefore

$$
W_{n+1}(i,j)=\sum_{k=1}^m W_n(i,k)A_{kj}.
$$

This is precisely the rule for [matrix multiplication](../../../vector-space.md#matrix-multiplication). [Mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) consequently gives

$$
\boxed{W_n(i,j)=(A^n)_{ij}.}
$$

Equivalently, expanding the [matrix](../../../vector-space.md#matrix) entry sums the products $A_{ix_1}A_{x_1x_2}\cdots A_{x_{n-1}j}$ over all intermediate symbols; each product is the [indicator function](../../../measure-theory.md#indicator-function) of one allowed transition chain.

**The intended meaning of “allowed” here is local admissibility.** If instead it means a word that actually occurs in some two-sided [sequence](../../../real-analysis.md#sequence) in $\Sigma_A$, the assertion needs an additional extension assumption. For example, $A=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ permits the word $(1,2)$ and has $(A)_{12}=1$, but $\Sigma_A$ is empty because no symbol can continue after $2$. Having a nonzero entry in every row and every column is sufficient: one can successively choose a predecessor and a successor to extend every [locally admissible word](../../../dynamical-systems.md#locally-admissible-word-for-a-transition-matrix) indefinitely in both directions. No such assumption is needed for the local counting formula.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The equation $\sigma^n x=x$ says $x_{r+n}=x_r$ for every $r\in\mathbb Z$. Thus a solution is determined uniquely by the block $(x_0,\ldots,x_{n-1})$, repeated in both directions. It belongs to the [subshift of finite type](../../../dynamical-systems.md#subshift-of-finite-type) exactly when all transitions inside the block, and the closing transition from $x_{n-1}$ to $x_0$, are allowed. Hence these [fixed points](../../../function.md#fixed-point) of the $n$th [iteration of a map](../../../dynamical-systems.md#iterated-function) are in [bijection](../../../function.md#bijection) with the closed transition chains of $n$ steps with a specified symbol at time zero. By the counting argument in part (b), the number starting at $i$ is $(A^n)_{ii}$. Summing over $i$ proves the [trace formula for periodic points of a subshift](../../../dynamical-systems.md#trace-formula-for-periodic-points-of-a-subshift):

$$
\boxed{\#\operatorname{Fix}(\sigma^n)=\operatorname{tr}(A^n).}
$$

Every closed transition chain extends by periodic repetition, so the extension issue in part (b) does not affect this formula. We count points, not [periodic orbits](../../../dynamical-systems.md#periodic-orbit): a least-period-$d$ [periodic orbit](../../../dynamical-systems.md#periodic-orbit) contributes its $d$ distinct points.

**Here period $n$ means fixed by $\sigma^n$, so the least period may divide $n$.** If $P_d$ denotes the number of points of least period exactly $d$, division with remainder shows that a point is fixed by $\sigma^n$ exactly when its least period divides $n$. Consequently

$$
\operatorname{tr}(A^n)=\sum_{d\mid n}P_d,qquad
P_n=\sum_{d\mid n}\mu_{\mathrm M}(n/d)\operatorname{tr}(A^d),
$$

where $\mu_{\mathrm M}$ is the [Möbius function](../../../number-theory.md#mobius-function) and the second equality is [Möbius inversion](../../../number-theory.md#mobius-inversion-formula). For example, $A=(1)$ has one point fixed by every power but no point of least period two; interpreting the printed formula as an exact-period count would therefore be false.

## 2

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The convention intended by this question is **existence of a dense forward orbit**, also called [point transitivity](../../../dynamical-systems.md#point-transitivity). On a nonempty [compact metric space](../../../topological-analysis.md#compact-metric-space), this means that some $x\in X$ satisfies

$$
\boxed{\overline{\{f^n(x):n\geq0\}}=X.}
$$

Equivalently, that forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) visits every nonempty [open set](../../../topology.md#open-set).

The other common definition of [topological transitivity](../../../dynamical-systems.md#topological-transitivity) uses intersections of iterated [open sets](../../../topology.md#open-set), as in part (b). The distinction matters on spaces with [isolated points](../../../topological-analysis.md#isolated-point): parts (b) and (c) ask precisely how the two conventions are related. We use [point transitivity](../../../dynamical-systems.md#point-transitivity) for the dense-orbit convention throughout this solution. As usual for this definition, the [state space](../../../dynamical-systems.md#state-space) is assumed nonempty; on an empty space the open-set condition is vacuous and there is no point with a forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A [compact metric space](../../../topological-analysis.md#compact-metric-space) is [second countable](../../../topology.md#second-countable-space). To see this concretely, for each positive integer $r$ choose a finite cover by balls of radius $1/r$. Their centres, over all $r$, form a countable [dense subset](../../../topology.md#dense-set); balls centred there with positive rational radii form a countable [basis of a topology](../../../topology.md#basis-of-a-topology). Enumerate its nonempty members as $(V_j)_{j\geq1}$, repeating members if the basis is finite.

For each $j$, put

$$
G_j=\bigcup_{n\geq1}f^{-n}(V_j).
$$

Each $G_j$ is an [open set](../../../topology.md#open-set), because all [iterations of a map](../../../dynamical-systems.md#iterated-function) $f^n$ are [continuous](../../../calculus.md#continuous-function). It is [dense](../../../topology.md#dense-set): if $U$ is any nonempty [open set](../../../topology.md#open-set), the hypothesis supplies $n\geq1$ and $u\in U$ with $f^n(u)\in V_j$, so $u\in U\cap G_j$.

A [compact metric space](../../../topological-analysis.md#compact-metric-space) is a [complete metric space](../../../topological-analysis.md#complete-metric-space), hence a [Baire space](../../../topological-analysis.md#baire-space). The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) implies that $G=\bigcap_{j\geq1}G_j$ is [dense](../../../topology.md#dense-set), and in particular nonempty. For any $x\in G$, the forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) of $x$ meets every $V_j$, and therefore every nonempty [open set](../../../topology.md#open-set). Its [orbit closure](../../../dynamical-systems.md#orbit-closure) is $X$. Thus **the open-set intersection hypothesis implies point transitivity**, and in fact the set of points with a dense forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) contains the dense intersection $G$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $x$ have a dense forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) $O=\{f^j(x):j\geq0\}$, and suppose that $f$ is [surjective](../../../algebra.md#surjective-function). Every tail $O_k=\{f^j(x):j\geq k\}$ is then [dense](../../../topology.md#dense-set). Indeed, [continuity](../../../calculus.md#continuous-function) gives

$$
f^k(\overline O)\subseteq\overline{f^k(O)}=\overline{O_k},
$$

and the left side equals $f^k(X)=X$ by [surjectivity](../../../algebra.md#surjective-function).

Given nonempty [open sets](../../../topology.md#open-set) $U,V$, choose $k\geq0$ with $f^k(x)\in U$. The dense tail $O_{k+1}$ supplies $j\geq k+1$ with $f^j(x)\in V$. Taking $n=j-k\geq1$ gives $f^j(x)\in f^n(U)\cap V$. This proves the required positive-time intersection property.

**The result can fail without [surjectivity](../../../algebra.md#surjective-function).** Take the [compact metric space](../../../topological-analysis.md#compact-metric-space)

$$
X=\{0\}\cup\{1/j:j\geq1\},qquad
f(0)=0,qquad f(1/j)=1/(j+1),
$$

with the [metric](../../../topological-analysis.md#metric) induced from the [real line](../../../real-analysis.md#real-line). All nonzero points are [isolated](../../../topological-analysis.md#isolated-point), so [continuity](../../../calculus.md#continuous-function) there is automatic; at zero, $f(1/j)\to0=f(0)$ proves [continuity](../../../calculus.md#continuous-function). The forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) of $1$ is $\{1,1/2,1/3,\ldots\}$, whose [closure](../../../topology.md#closure-topology) is $X$, so this is [point transitivity](../../../dynamical-systems.md#point-transitivity). But $f(X)=X\setminus\{1\}$. The singletons $U=\{1/2\}$ and $V=\{1\}$ are nonempty [open sets](../../../topology.md#open-set), and for every $n\geq1$,

$$
f^n(U)=\{1/(n+2)\},qquad f^n(U)\cap V=\varnothing.
$$

The isolated initial point can be visited only at the start of the dense forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system); deleting that initial segment destroys density.

## 3

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the separated-set definition of [topological entropy](../../../dynamical-systems.md#topological-entropy). For a [compatible metric](../../../topological-analysis.md#compatible-metric) $d$ and $n\geq1$, define the [Bowen metric](../../../dynamical-systems.md#bowen-metric) and separated-set count by

$$
d_n(x,y)=\max_{0\leq k<n}d(f^kx,f^ky),\qquad
s_n(d,\epsilon)=\max\{|E|:d_n(x,y)\geq\epsilon\text{ for distinct }x,y\in E\}.
$$

For fixed $n$, the [metric](../../../topological-analysis.md#metric) $d_n$ generates the original [topology](../../../topology.md): it includes the $k=0$ term and all finitely many [iterations of a map](../../../dynamical-systems.md#iterated-function) are [continuous](../../../calculus.md#continuous-function). Thus its space is compact and $s_n(d,\epsilon)$ is finite. With natural logarithms, set

$$
h_d(f,\epsilon)=\limsup_{n\to\infty}\frac{\log s_n(d,\epsilon)}n,qquad
h_d(f)=\lim_{\epsilon\downarrow0}h_d(f,\epsilon).
$$

The last limit exists, possibly with value infinity, because decreasing $\epsilon$ can only increase separated-set counts.

Let $d'$ be another [compatible metric](../../../topological-analysis.md#compatible-metric). The identity $(X,d)\to(X,d')$ is a [continuous function](../../../calculus.md#continuous-function) on a compact domain, hence [uniformly continuous](../../../topological-analysis.md#uniform-continuity). For every $\epsilon>0$, choose $\delta>0$ such that $d(x,y)<\delta$ implies $d'(x,y)<\epsilon$. The same implication at every iterate gives

$$
d_n(x,y)<\delta\ \Longrightarrow\ d'_n(x,y)<\epsilon.
$$

By its contrapositive, every $\epsilon$-[separated set](../../../topological-analysis.md#separated-subset-of-a-metric-space) for $d'_n$ is $\delta$-separated for $d_n$. Consequently $s_n(d',\epsilon)\leq s_n(d,\delta)$ for every $n$, and

$$
h_{d'}(f,\epsilon)\leq h_d(f,\delta)\leq h_d(f).
$$

Taking $\epsilon\downarrow0$ gives $h_{d'}(f)\leq h_d(f)$. Interchanging the two [compatible metrics](../../../topological-analysis.md#compatible-metric) gives the reverse inequality. Therefore

$$
\boxed{h_{d'}(f)=h_d(f)=h_{\mathrm{top}}(f).}
$$

[Compactness](../../../topology.md#compact-space) is used for [uniform continuity](../../../topological-analysis.md#uniform-continuity), not merely for pointwise equivalence of the two [metrics](../../../topological-analysis.md#metric).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $H:X\to Y$ be a [homeomorphism](../../../topology.md#homeomorphism) with $H\circ f=g\circ H$. This is [topological conjugacy](../../../dynamical-systems.md#topological-conjugacy). Choose a [compatible metric](../../../topological-analysis.md#compatible-metric) $e$ on $Y$ and pull it back to $X$:

$$
d_H(x,x')=e(Hx,Hx').
$$

Because $H$ is a [homeomorphism](../../../topology.md#homeomorphism), $d_H$ is a [compatible metric](../../../topological-analysis.md#compatible-metric). The conjugacy identity implies $Hf^k=g^kH$ for every $k\geq0$, so the corresponding [Bowen metrics](../../../dynamical-systems.md#bowen-metric) satisfy

$$
(d_H)_n(x,x')=\max_{0\leq k<n}e(g^kHx,g^kHx')=e_n(Hx,Hx').
$$

The [bijection](../../../function.md#bijection) $H$ therefore transports [separated sets](../../../topological-analysis.md#separated-subset-of-a-metric-space) in either direction without changing their separation, and $s_n(d_H,\epsilon)=s_n(e,\epsilon)$. Their exponential growth rates, and then their limits as $\epsilon\downarrow0$, agree. Part (a) lets us replace $d_H$ by any [compatible metric](../../../topological-analysis.md#compatible-metric) on $X$. Hence

$$
\boxed{h_{\mathrm{top}}(f)=h_{\mathrm{top}}(g).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write the [hyperbolic toral automorphism](../../../dynamical-systems.md#hyperbolic-toral-automorphism) as $T_A([v])=[Av]$ on $\mathbb T^2=\mathbb R^2/\mathbb Z^2$, where $A\in\mathrm{GL}(2,\mathbb Z)$. Its [determinant](../../../linear-algebra.md#determinant) is $\pm1$. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) cannot be a nonreal conjugate pair: their product would have [absolute value](../../../real-analysis.md#absolute-value) one, forcing each to have [absolute value](../../../real-analysis.md#absolute-value) one, contrary to hyperbolicity. The same product condition and hyperbolicity imply two distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue), labelled so that

$$
0<|\lambda_s|<1<|\lambda_u|,qquad |\lambda_s\lambda_u|=1.
$$

We will prove

$$
\boxed{h_{\mathrm{top}}(T_A)=\log|\lambda_u|.}
$$

This is the [entropy of a hyperbolic toral automorphism](../../../dynamical-systems.md#entropy-of-a-hyperbolic-toral-automorphism); the [absolute value](../../../real-analysis.md#absolute-value) is important when the expanding [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is negative.

Choose real [eigenvectors](../../../linear-operator-theory.md#eigenvector) $v_s,v_u$ and the adapted [norm](../../../functional-analysis.md#norm) $\|a v_s+b v_u\|_*=\max(|a|,|b|)$. Its quotient [metric](../../../topological-analysis.md#metric) on the [torus](../../../topology.md#torus) is

$$
d([v],[w])=\min_{\ell\in\mathbb Z^2}\|v-w-\ell\|_*.
$$

It is a [compatible metric](../../../topological-analysis.md#compatible-metric), so part (a) allows its use. Let $\rho=\min_{0\ne\ell\in\mathbb Z^2}\|\ell\|_*>0$ and $D=\|A\|_*=|\lambda_u|$. Fix $\epsilon>0$ small enough that $2\epsilon<\rho$ and $(D+1)\epsilon<\rho$.

If $[v]$ lies in the [Bowen ball](../../../dynamical-systems.md#bowen-ball) $B_n(0,\epsilon)$, each $T_A^k[v]$ has a unique lift $z_k$ with $\|z_k\|_*<\epsilon$. Uniqueness follows because two such lifts differ by a lattice vector of [norm](../../../functional-analysis.md#norm) less than $2\epsilon<\rho$. Moreover, $z_{k+1}-Az_k$ is a lattice vector, and

$$
\|z_{k+1}-Az_k\|_*<(D+1)\epsilon<\rho.
$$

It must be zero. Thus $z_k=A^kz_0$: there is no hidden lattice jump between successive lifted iterates.

Write $z_0=a v_s+b v_u$. The simultaneous bounds $\|A^kz_0\|_*<\epsilon$ for $0\leq k<n$ are exactly

$$
|a|<\epsilon,qquad |b|<\epsilon|\lambda_u|^{-(n-1)}.
$$

The stable coordinate is largest at time zero and the unstable coordinate at time $n-1$. Conversely, every vector in this rectangle satisfies all the [Bowen ball](../../../dynamical-systems.md#bowen-ball) bounds. The quotient is injective on this rectangle by $2\epsilon<\rho$. If $J=|\det(v_s,v_u)|$, its normalized [Haar measure](../../../measure-theory.md#haar-measure) is therefore

$$
\nu(B_n(0,\epsilon))=4J\epsilon^2|\lambda_u|^{-(n-1)}.
$$

The quotient [metric](../../../topological-analysis.md#metric) is translation invariant and $T_A$ is linear, so $d_n(x,y)=d_n(0,y-x)$; every [Bowen ball](../../../dynamical-systems.md#bowen-ball) has this same [measure](../../../measure-theory.md#measure), independently of its centre.

Take an $\epsilon$-[separated set](../../../topological-analysis.md#separated-subset-of-a-metric-space) of largest cardinality $s_n(d,\epsilon)$. It is maximal under inclusion, so its radius-$\epsilon$ [Bowen balls](../../../dynamical-systems.md#bowen-ball) cover the [torus](../../../topology.md#torus): a point outside all these balls could be added. The covering bound gives

$$
s_n(d,\epsilon)\geq\frac1{4J\epsilon^2}|\lambda_u|^{n-1}.
$$

Its radius-$\epsilon/2$ [Bowen balls](../../../dynamical-systems.md#bowen-ball) are disjoint, by the [triangle inequality](../../../topological-analysis.md#triangle-inequality) for $d_n$. Their measures sum to at most one, giving

$$
s_n(d,\epsilon)\leq\frac1{J\epsilon^2}|\lambda_u|^{n-1}.
$$

Taking logarithms, dividing by $n$, and letting $n\to\infty$ yields $h_d(T_A,\epsilon)=\log|\lambda_u|$ for every sufficiently small $\epsilon$. The limit as $\epsilon\downarrow0$ proves the answer. Contraction in the stable direction contributes no exponential growth; only expansion in the unstable direction does.

## 4

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $(X,\mathcal B,\mu)$ be a [probability space](../../../probability-theory.md#probability-space), let $T$ be a [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation), and let $g\in L^1(\mu)$. The [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem) asserts that

$$
A_ng(x)=\frac1n\sum_{k=0}^{n-1}g(T^kx)
\longrightarrow g^*(x)=\mathbb E_\mu[g\mid\mathcal I](x)
$$

for almost every $x$, where $\mathcal I=\{B\in\mathcal B:\mu(T^{-1}B\mathbin{\triangle}B)=0\}$ is the [invariant sigma-algebra](../../../measure-theory.md#invariant-sigma-algebra). The limit is integrable, satisfies $g^*\circ T=g^*$ almost everywhere, and has $\int g^*\,d\mu=\int g\,d\mu$. On a [probability space](../../../probability-theory.md#probability-space) the convergence also holds in $L^1$. No invertibility of $T$ is required.

If $T$ is [ergodic](../../../measure-theory.md#ergodicity), its [invariant sigma-algebra](../../../measure-theory.md#invariant-sigma-algebra) is trivial modulo null sets, so its [conditional expectation](../../../measure-theory.md#conditional-expectation) is constant. In that case the concise form is

$$
\boxed{A_ng(x)\longrightarrow\int_Xg\,d\mu\quad\text{for almost every }x.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Identify the [circle group](../../../lie-theory.md#circle-group) with $[0,1)$ modulo its endpoints, and let $\lambda$ be normalized [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). We first check invariance. On the $r$th inverse branch, $x=(y+r)/m$ for $0\leq r<m$. For an integrable [function](../../../function.md) $g$, substitution gives

$$
\int_0^1g(E_mx)\,dx
=\sum_{r=0}^{m-1}\frac1m\int_0^1g(y)\,dy
=\int_0^1g(y)\,dy.
$$

In particular, testing [indicator functions](../../../measure-theory.md#indicator-function) shows that the [integer multiplication map on the circle](../../../measure-theory.md#integer-multiplication-map-on-the-circle) preserves $\lambda$.

To prove [ergodicity](../../../measure-theory.md#ergodicity), let $B$ be a measurable set with $\lambda(E_m^{-1}B\mathbin{\triangle}B)=0$ and put $h=\mathbf1_B$. Then $h(E_mx)=h(x)$ almost everywhere. Its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are

$$
c_k=\int_0^1h(x)e^{-2\pi ikx}\,dx\qquad(k\in\mathbb Z).
$$

Using invariance of $h$ and substituting separately on the same $m$ branches gives

$$
\begin{aligned}
c_k
&=\int_0^1h(E_mx)e^{-2\pi ikx}\,dx\\
&=\frac1m\sum_{r=0}^{m-1}e^{-2\pi ikr/m}
  \int_0^1h(y)e^{-2\pi i(k/m)y}\,dy\\
&=\begin{cases}0,&m\nmid k,\\c_{k/m},&m\mid k.\end{cases}
\end{aligned}
$$

In the last line, the finite [geometric series](../../../real-analysis.md#geometric-series) of $m$th [roots of unity](../../../algebra.md#root-of-unity) is zero unless $m$ divides $k$, when it equals $m$. For any nonzero integer $k$, divide repeatedly by $m$ until the resulting integer is no longer divisible by $m$. The recurrence then implies $c_k=0$.

Since the [Fourier basis](../../../fourier-series.md#fourier-basis) is a complete [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $L^2([0,1),\lambda)$, the absence of every nonconstant [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) implies $h=c_0=\lambda(B)$ almost everywhere. An [indicator function](../../../measure-theory.md#indicator-function) takes only the values zero and one, so $\lambda(B)$ must be zero or one. This proves

$$
\boxed{E_m\text{ is ergodic for Lebesgue measure for every integer }m\geq2.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Outside the [countable set](../../../set-theory.md#countable-set) of dyadic rational numbers, the [binary expansion](../../../arithmetic.md#binary-expansion) $x=\sum_{j\geq1}\epsilon_j(x)2^{-j}$ is unique. Multiplication by two modulo one deletes the first binary digit, so

$$
\epsilon_j(x)=\mathbf1_{[1/2,1)}(E_2^{j-1}x).
$$

Let $g=\mathbf1_{[1/2,1)}$. By part (b), the [doubling map](../../../dynamical-systems.md#dyadic-transformation) is a [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation) and is [ergodic](../../../measure-theory.md#ergodicity) for [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Applying the [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem) to this [indicator function](../../../measure-theory.md#indicator-function) gives

$$
\frac1n\#\{1\leq j\leq n:\epsilon_j(x)=1\}
=\frac1n\sum_{k=0}^{n-1}g(E_2^kx)
\longrightarrow\int_0^1g(x)\,dx=\frac12
$$

for almost every $x$. The dyadic rationals have [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) zero, so the choice of their two possible [binary expansions](../../../arithmetic.md#binary-expansion) does not affect the conclusion. Thus **the limiting frequency of the digit one is $1/2$ almost everywhere**.

## 5

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

We first prove invariance, before using any assertion that requires it. Write $A_n\varphi(x)=n^{-1}\sum_{k=0}^{n-1}\varphi(f^kx)$. Choose a point whose forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) has the prescribed convergence against every [continuous function](../../../calculus.md#continuous-function); the hypothesis gives a set of such points of full [measure](../../../measure-theory.md#measure). For each [continuous function](../../../calculus.md#continuous-function) $\varphi$, telescoping gives

$$
A_n(\varphi\circ f)(x)-A_n\varphi(x)
=\frac{\varphi(f^nx)-\varphi(x)}n\longrightarrow0,
$$

because a [continuous function](../../../calculus.md#continuous-function) on a [compact metric space](../../../topological-analysis.md#compact-metric-space) is bounded. Both test functions are continuous, so their averages converge to their prescribed integrals. Hence

$$
\int_X\varphi\circ f\,d\mu=\int_X\varphi\,d\mu
$$

for every [continuous function](../../../calculus.md#continuous-function) $\varphi$. The continuous-test criterion for an [invariant measure](../../../measure-theory.md#invariant-measure) therefore gives **$f_*\mu=\mu$**. The points in the hypothesis can now be called [generic points for an invariant measure](../../../measure-theory.md#generic-point-for-an-invariant-measure).

For [ergodicity](../../../measure-theory.md#ergodicity), let $B$ be a [Borel set](../../../measure-theory.md#borel-set) invariant modulo null sets, and set $h=\mathbf1_B$, $p=\mu(B)$. Then $h\circ f=h$ almost everywhere. Since invariance preserves null preimages, deleting the union of all iterated preimages of the exceptional [null set](../../../measure-theory.md#null-set) gives $h(f^kx)=h(x)$ for every $k\geq0$ on one full-measure set. Thus $A_nh=h$ almost everywhere for every $n$.

Given $\epsilon>0$, the [continuous approximation of Borel indicators on a compact metric space](../../../measure-theory.md#continuous-approximation-of-borel-indicators-on-a-compact-metric-space), proved in the supporting steps below, supplies $\varphi\in C(X)$ with $0\leq\varphi\leq1$ and $\|h-\varphi\|_{L^1(\mu)}<\epsilon$. By the hypothesis, $A_n\varphi\to\int\varphi\,d\mu$ almost everywhere. Since $0\leq A_n\varphi\leq1$, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) also gives convergence in $L^1(\mu)$. Invariance and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) give the uniform estimate

$$
\|A_n(h-\varphi)\|_{L^1(\mu)}
\leq\frac1n\sum_{k=0}^{n-1}\int_X|h-\varphi|\circ f^k\,d\mu
=\|h-\varphi\|_{L^1(\mu)}<\epsilon.
$$

Consequently,

$$
\begin{aligned}
\|h-p\|_{L^1(\mu)}
&\leq\|A_nh-A_n\varphi\|_{L^1(\mu)}
 +\left\|A_n\varphi-\int\varphi\,d\mu\right\|_{L^1(\mu)}
 +\left|\int\varphi\,d\mu-p\right|\\
&<2\epsilon+\left\|A_n\varphi-\int\varphi\,d\mu\right\|_{L^1(\mu)}.
\end{aligned}
$$

Letting $n\to\infty$ and then $\epsilon\downarrow0$ proves $\|h-p\|_1=0$. Explicitly,

$$
\|\mathbf1_B-p\|_1=p(1-p)+(1-p)p=2p(1-p),
$$

so $p\in\{0,1\}$. Every invariant [Borel set](../../../measure-theory.md#borel-set) has [measure](../../../measure-theory.md#measure) zero or one, which proves

$$
\boxed{\mu\text{ is invariant and ergodic}.}
$$

This proof controls measurable-set averages through a uniform $L^1$ estimate; convergence only against continuous test functions is not silently assumed to include [indicator functions](../../../measure-theory.md#indicator-function).

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Here is an alternative route for the ergodicity step using the [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem). After invariance has been proved, the theorem identifies the almost-everywhere limit of $A_n\varphi$ with $\mathbb E_\mu[\varphi\mid\mathcal I]$. The hypothesis therefore gives

$$
\mathbb E_\mu[\varphi\mid\mathcal I]=\int\varphi\,d\mu
$$

for every [continuous function](../../../calculus.md#continuous-function) $\varphi$. For an invariant [Borel set](../../../measure-theory.md#borel-set) $B$, approximate $h=\mathbf1_B$ in $L^1$ by such a $\varphi$. Since $h$ is measurable with respect to the [invariant sigma-algebra](../../../measure-theory.md#invariant-sigma-algebra), its [conditional expectation](../../../measure-theory.md#conditional-expectation) is $h$ itself. The [L1 contraction of conditional expectation](../../../measure-theory.md#l1-contraction-of-conditional-expectation) gives

$$
\left\|h-\mu(B)\right\|_1
\leq\left\|\mathbb E_\mu[h-\varphi\mid\mathcal I]\right\|_1
 +\left|\int(\varphi-h)\,d\mu\right|
\leq2\|h-\varphi\|_1.
$$

Arbitrarily accurate continuous approximation forces $h=\mu(B)$ almost everywhere. Thus this use of the theorem reaches the same zero-or-one criterion as the direct averaging proof above, without assuming in advance that $\mu$ is [ergodic](../../../measure-theory.md#ergodicity).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

For a [Borel set](../../../measure-theory.md#borel-set) $B$ and $\epsilon>0$, [inner regularity](../../../measure-theory.md#inner-regular-measure) supplies a [compact set](../../../topology.md#compact-space) $K\subseteq B$ with $\mu(B)-\mu(K)<\epsilon/2$. Independently, [outer regularity](../../../measure-theory.md#outer-regular-measure) supplies an [open set](../../../topology.md#open-set) $U\supseteq B$ with $\mu(U)-\mu(B)<\epsilon/2$. Because $K\subseteq U$ and the [measure](../../../measure-theory.md#measure) is finite,

$$
\mu(U\setminus K)=\mu(U)-\mu(K)<\epsilon.
$$

This creates an arbitrarily small measurable transition region between a compact inner approximation and an open outer approximation. The cutoff in the next step then approximates $\mathbf1_B$, rather than merely approximating the number $\mu(B)$.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

For the [compact set](../../../topology.md#compact-space) $K\subseteq B\subseteq U$ chosen in the preceding step, the [Urysohn lemma](../../../topology.md#urysohn-s-lemma) gives a [continuous function](../../../calculus.md#continuous-function) $0\leq\varphi\leq1$ equal to one on $K$ and zero on $X\setminus U$. In a [metric space](../../../topological-analysis.md#metric-space) this cutoff can also be written explicitly, when $K$ and $X\setminus U$ are both nonempty:

$$
\varphi(x)=\frac{d(x,X\setminus U)}{d(x,K)+d(x,X\setminus U)}.
$$

The two sets are disjoint and closed, so the denominator never vanishes, and their distance functions are [continuous](../../../calculus.md#continuous-function). If $K$ is empty, take $\varphi=0$; if $U=X$ and $K$ is nonempty, take $\varphi=1$. These choices satisfy the required boundary conditions in the exceptional cases.

The difference $\varphi-\mathbf1_B$ vanishes on $K$ and outside $U$, and its [absolute value](../../../real-analysis.md#absolute-value) is at most one everywhere. Therefore

$$
\boxed{\|\varphi-\mathbf1_B\|_{L^1(\mu)}\leq\mu(U\setminus K)<\epsilon.}
$$

This is the precise continuous approximation required by both proofs of [ergodicity](../../../measure-theory.md#ergodicity), and also gives $|\int\varphi\,d\mu-\mu(B)|<\epsilon$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
