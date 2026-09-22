# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper30.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Orient each [edge](../../../graph-theory.md#edge-of-a-graph) both ways. A [unit flow](../../../graph-theory.md#unit-flow) $j$ from $x$ to $y$ is antisymmetric, $j(u,v)=-j(v,u)$, with [divergence of a flow](../../../graph-theory.md#divergence-of-a-flow) equal to $+1$ at $x$, $-1$ at $y$ and zero elsewhere. Its energy is

$$
\mathcal E_r(j)=\sum_{e\in E}r_ej(e)^2,
$$

where each unoriented [edge](../../../graph-theory.md#edge-of-a-graph) is counted once. Put $c_e=1/r_e$. The electrical unit current is $i(u,v)=c_{uv}(V(u)-V(v))$, where the potential $V$ solves the [Kirchhoff node law](../../../markov-process.md#kirchhoff-node-law) with those source and sink divergences. Because $G$ is a [connected graph](../../../graph.md#connected-graph), this potential is unique up to an additive constant. The [effective resistance](../../../markov-process.md#effective-resistance) is the [electric potential difference](../../../electromagnetism.md#electric-potential-difference) needed for unit current,

$$
R(x,y)=V(x)-V(y).
$$

Discrete summation by parts gives $\mathcal E_r(i)=\sum_uV(u)\operatorname{div}i(u)=R(x,y)$.

The [Thomson principle](../../../markov-process.md#thomson-principle) says that this current minimizes energy among all [unit flows](../../../graph-theory.md#unit-flow). Indeed write any other [unit flow](../../../graph-theory.md#unit-flow) as $j=i+k$, where $\operatorname{div}k=0$. Then

$$
\sum_er_ei(e)k(e)=\sum_{e=(u,v)}(V(u)-V(v))k(u,v)=\sum_uV(u)\operatorname{div}k(u)=0.
$$

Consequently

$$
\mathcal E_r(j)=R(x,y)+\mathcal E_r(k)\ge R(x,y),\qquad
\boxed{R(x,y)=\min_{j\text{ unit flow }x\to y}\mathcal E_r(j).}
$$

This also proves uniqueness of the minimizing current.

If $r'_e\ge r_e$ for every [edge](../../../graph-theory.md#edge-of-a-graph), then $\mathcal E_{r'}(j)\ge\mathcal E_r(j)$ for every admissible [flow](../../../graph-theory.md#flow). The admissible set is unchanged, so taking its minimum proves the [Rayleigh monotonicity principle](../../../markov-process.md#rayleigh-monotonicity-principle):

$$
\boxed{R_{r'}(x,y)\ge R_r(x,y).}
$$

Deletion is the limiting operation $r_e\to\infty$: finite-energy [flows](../../../graph-theory.md#flow) must then carry zero current on that [edge](../../../graph-theory.md#edge-of-a-graph). If the terminals become disconnected, the [effective resistance](../../../markov-process.md#effective-resistance) is infinite.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use $T_y=\inf\{n\ge0:X_n=y\}$ and the positive return time $T_x^+=\inf\{n\ge1:X_n=x\}$. The walk has transitions $p_{uv}=c_{uv}/d(u)$, $d(u)=\sum_vc_{uv}$; its transition matrix defines a [reversible Markov chain](../../../markov-process.md#reversible-markov-chain), although the [transition probabilities](../../../markov-process.md#transition-probability) need not be symmetric.

The voltage $h(u)=P_u(T_x<T_y)$ equals one at $x$, zero at $y$, and is a [harmonic function on a graph](../../../partial-differential-equation.md#discrete-harmonic-function) away from the terminals: $h(u)=\sum_vp_{uv}h(v)$. For this unit [electric potential difference](../../../electromagnetism.md#electric-potential-difference) the [electric current](../../../electromagnetism.md#electric-current) is

$$
I=\sum_vc_{xv}(1-h(v))=\frac1{R(x,y)}.
$$

The [first-step analysis](../../../analysis.md#first-step-analysis) therefore proves the [return probability from effective resistance](../../../markov-process.md#return-probability-from-effective-resistance) identity:

$$
P_x(T_x^+<T_y)=\sum_vp_{xv}h(v)
=1-\frac{I}{d(x)}
=\boxed{1-\frac1{d(x)R(x,y)}}.
$$

Finite irreducibility ensures eventual hitting of one of the terminals, so no missing escape event appears in this finite-network calculation.

For an infinite locally finite [connected graph](../../../graph.md#connected-graph), exhaust it by finite sets and wire their exteriors to one sink. The event of exiting before the first return decreases to the event of never returning. Thus

$$
P_o(T_o^+=\infty)=\frac1{d(o)R(o,\infty)},
$$

with $1/\infty=0$. In particular [recurrence](../../../markov-process.md#recurrent-markov-chain) is equivalent to infinite [effective resistance to infinity](../../../markov-process.md#effective-resistance-to-infinity).

After deleting an [edge](../../../graph-theory.md#edge-of-a-graph), consider any infinite component and choose a root $o$ away from that [edge](../../../graph-theory.md#edge-of-a-graph)'s endpoints. Its [vertex degree](../../../graph-theory.md#degree-graph-theory) $d(o)$ is unchanged. On every finite wired exhaustion the [Rayleigh monotonicity principle](../../../markov-process.md#rayleigh-monotonicity-principle) makes the resistance no smaller; the [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) does too. A [recurrent](../../../markov-process.md#recurrent-markov-chain) original network consequently leaves a [recurrent](../../../markov-process.md#recurrent-markov-chain) component. Finite components give [recurrent](../../../markov-process.md#recurrent-markov-chain) walks as well, with an isolated [graph vertex](../../../graph.md#vertex-graph-theory) viewed as an [absorbing state](../../../markov-process.md#absorbing-state). This proves that [edge deletion preserves recurrence](../../../markov-process.md#edge-deletion-preserves-recurrence). The phrase “no less [recurrent](../../../markov-process.md#recurrent-markov-chain)” refers to this [recurrence](../../../markov-process.md#recurrent-markov-chain) comparison: at a deleted-edge endpoint the [vertex degree](../../../graph-theory.md#degree-graph-theory) factor also changes, so monotonicity of its first-return [probability](../../../probability-theory.md#probability) alone should not be inferred.

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) of length $n$ is a sequence of $n+1$ distinct [graph vertices](../../../graph.md#vertex-graph-theory) joined consecutively by [edges](../../../graph-theory.md#edge-of-a-graph). Split a rooted [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) of length $m+n$ after $m$ steps. There are $\kappa_m$ possible prefixes; each remaining segment is a self-avoiding $n$-step walk from its current [graph vertex](../../../graph.md#vertex-graph-theory), and forbidding intersections with the prefix can only reduce its count below $\kappa_n$. [Translation invariance](../../../physics.md#translation-invariance) therefore gives

$$
\kappa_{m+n}\le\kappa_m\kappa_n.
$$

Apply the [Fekete lemma](../../../real-analysis.md#fekete-s-lemma), proved in Question 4(a), to $\log\kappa_n$. It gives $\log\mu=\inf_n n^{-1}\log\kappa_n$ and hence existence of the [connective constant](../../../combinatorics.md#connective-constant). Walks using only the $d$ positive coordinate directions never revisit a [graph vertex](../../../graph.md#vertex-graph-theory), so there are at least $d^n$. A walk has $2d$ choices for its first step and at most $2d-1$ subsequently because immediate reversal is forbidden. Thus

$$
d^n\le\kappa_n\le2d(2d-1)^{n-1},\qquad\boxed{d\le\mu\le2d-1.}
$$

For independent [bond percolation](../../../bond-percolation.md), let $C(0)$ be the [percolation cluster](../../../bond-percolation.md#percolation-cluster) of the origin, $\theta(p)=P_p(|C(0)|=\infty)$, and $p_c=\inf\{p:\theta(p)>0\}$. An [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) in a locally finite [graph](../../../graph.md) contains an open self-avoiding path of every length. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\theta(p)\le\kappa_np^n.
$$

When $p\mu<1$, the right-hand side tends to zero, since its $n$th root tends to $p\mu$. Hence the [connective-constant lower bound for percolation](../../../probability-theory.md#connective-constant-lower-bound-for-percolation) is

$$
\boxed{p_c\ge\mu^{-1}.}
$$

For the upper bound in two dimensions, use the square [planar dual graph](../../../graph-theory.md#planar-dual-graph). Call a dual [edge](../../../graph-theory.md#edge-of-a-graph) available when its crossing primal [edge](../../../graph-theory.md#edge-of-a-graph) is closed. Each dual [edge](../../../graph-theory.md#edge-of-a-graph) is available with [probability](../../../probability-theory.md#probability) $q=1-p$, independently. The [planar graph](../../../graph-theory.md#planar-graph) boundary lemma says that a finite primal [percolation cluster](../../../bond-percolation.md#percolation-cluster) is enclosed by a [graph cycle](../../../graph-theory.md#cycle-in-a-graph) consisting of such [edges](../../../graph-theory.md#edge-of-a-graph): its external [edge](../../../graph-theory.md#edge-of-a-graph) boundary gives this [graph cycle](../../../graph-theory.md#cycle-in-a-graph). We show that $q\mu<1$ guarantees positive percolation [probability](../../../probability-theory.md#probability).

Let $N_n$ count enclosing [graph cycles](../../../graph-theory.md#cycle-in-a-graph) of length $n$. Because the origin lies inside their coordinate bounding box and their diameter is at most $n$, every such [graph cycle](../../../graph-theory.md#cycle-in-a-graph) has a [graph vertex](../../../graph.md#vertex-graph-theory) within a box of side $2n+3$. From each possible root, the first $n-1$ [edges](../../../graph-theory.md#edge-of-a-graph) give a [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk); the final closing [edge](../../../graph-theory.md#edge-of-a-graph) is then determined. Dropping the closure restriction gives the convenient bound

$$
N_n\le(2n+3)^2\kappa_{n-1}.
$$

Choose $\rho$ with $q\mu<\rho<1$. The connective-constant [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) implies $\kappa_{n-1}q^n\le C\rho^n$. Consequently the large-circuit tail

$$
\sum_{n\ge L}N_nq^n\longrightarrow0\qquad(L\to\infty)
$$

is summable.

Condition all primal [edges](../../../graph-theory.md#edge-of-a-graph) inside a large square $[-L,L]^2$ to be open; this event has positive [probability](../../../probability-theory.md#probability). The origin [percolation cluster](../../../bond-percolation.md#percolation-cluster) then contains that square. If it is finite, its enclosing [graph cycle](../../../graph-theory.md#cycle-in-a-graph) has length at least $L$. A proposed [graph cycle](../../../graph-theory.md#cycle-in-a-graph) using a pinned-open [edge](../../../graph-theory.md#edge-of-a-graph) now has [conditional probability](../../../probability-theory.md#conditional-probability) zero; every other proposed [graph cycle](../../../graph-theory.md#cycle-in-a-graph) still has [probability](../../../probability-theory.md#probability) $q^n$ by [independence of random variables](../../../random-variable.md#independent-random-variables). For $L$ large enough the [union bound](../../../probability-inequality.md#boole-s-inequality) for the remaining [graph cycles](../../../graph-theory.md#cycle-in-a-graph) is less than one. There is therefore positive [conditional probability](../../../probability-theory.md#conditional-probability) that the origin [percolation cluster](../../../bond-percolation.md#percolation-cluster) is infinite. This proves the [connective-constant Peierls bound](../../../probability-theory.md#connective-constant-peierls-bound) without needing the exact value of $p_c$:

$$
\boxed{p_c\le1-\mu^{-1}\quad(d=2).}
$$

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Order configurations coordinatewise: $\omega\le\eta$ when $\omega(e)\le\eta(e)$ for every coordinate. An [increasing event](../../../probability-inequality.md#increasing-event) $A$ is an upward-closed set: $\omega\in A$ and $\omega\le\eta$ imply $\eta\in A$.

The finite-lattice [FKG inequality](../../../probability-inequality.md#fkg-inequality) states that a [probability](../../../probability-theory.md#probability) mass function satisfying the [FKG lattice condition](../../../probability-inequality.md#fkg-lattice-condition)

$$
\mu(\omega\vee\eta)\mu(\omega\wedge\eta)\ge\mu(\omega)\mu(\eta)
\quad\text{for every }\omega,\eta
$$

is [positively associated](../../../probability-theory.md#positive-association-of-random-variables). Here [meet in a lattice](../../../mathematical-logic.md#meet-in-a-lattice) and [join in a lattice](../../../mathematical-logic.md#join-in-a-lattice) are coordinatewise minimum and maximum. Thus for [increasing observables](../../../set.md#increasing-function-on-a-partially-ordered-set) $f,g$,

$$
E_\mu[fg]\ge E_\mu[f]E_\mu[g].
$$

Taking [indicator functions](../../../measure-theory.md#indicator-function) gives **$\mu(A\cap B)\ge\mu(A)\mu(B)$ for all [increasing events](../../../probability-inequality.md#increasing-event)**. The strictly positive version suffices for the Ising weights here; the theorem also holds for nonnegative log-supermodular weights of positive total mass.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Work [edge](../../../graph-theory.md#edge-of-a-graph) by [edge](../../../graph-theory.md#edge-of-a-graph). Let $\omega,\eta$ have two-bit restrictions to an [edge](../../../graph-theory.md#edge-of-a-graph). If these restrictions are comparable, taking their [meet in a lattice](../../../mathematical-logic.md#meet-in-a-lattice) and [join in a lattice](../../../mathematical-logic.md#join-in-a-lattice) only reorders the two pairs, so their total equality indicators do not change. If they are incomparable, they are $01$ and $10$, while their [meet in a lattice](../../../mathematical-logic.md#meet-in-a-lattice) and [join in a lattice](../../../mathematical-logic.md#join-in-a-lattice) are $00$ and $11$. In that case the sum of equality indicators increases from zero to two. Consequently

$$
\Delta_e=\delta_{(\omega\vee\eta)(x),(\omega\vee\eta)(y)}
+\delta_{(\omega\wedge\eta)(x),(\omega\wedge\eta)(y)}
-\delta_{\omega(x),\omega(y)}-\delta_{\eta(x),\eta(y)}\ge0.
$$

The [partition functions](../../../statistical-physics.md#canonical-partition-function) cancel from the required ratio, leaving

$$
\frac{\mu_\Lambda(\omega\vee\eta)\mu_\Lambda(\omega\wedge\eta)}
{\mu_\Lambda(\omega)\mu_\Lambda(\eta)}
=\exp\left(\beta\sum_e\Delta_e\right)\ge1.
$$

This is the [ferromagnetic Ising lattice inequality](../../../statistical-physics.md#ferromagnetic-ising-lattice-inequality) in binary-spin normalization, so **the measure satisfies the [FKG lattice condition](../../../probability-inequality.md#fkg-lattice-condition) and is [positively associated](../../../probability-theory.md#positive-association-of-random-variables)**. If $\sigma(x)=2\omega(x)-1$, then $\delta_{\omega(x),\omega(y)}=(1+\sigma(x)\sigma(y))/2$: the conventional $\{-1,1\}$ coupling is $\beta/2$, which explains the factor two in the [edge](../../../graph-theory.md#edge-of-a-graph) calculation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With the inner boundary specified in the PDF, the [Ising boundary condition](../../../statistical-physics.md#ising-boundary-condition) pins $\omega|_{\partial\Lambda}=\zeta$. Explicitly $\mu_\Lambda^\zeta$ is $\mu_\Lambda$ conditioned on those [Ising spins](../../../statistical-physics.md#ising-spin-variable). Its [partition function](../../../statistical-physics.md#canonical-partition-function) sums over unpinned interior [Ising spins](../../../statistical-physics.md#ising-spin-variable) only; [edges](../../../graph-theory.md#edge-of-a-graph) between two pinned sites contribute a constant that cancels on normalization.

Pinning coordinates preserves the [FKG lattice condition](../../../probability-inequality.md#fkg-lattice-condition), since [meet in a lattice](../../../mathematical-logic.md#meet-in-a-lattice) and [join in a lattice](../../../mathematical-logic.md#join-in-a-lattice) still have the same pinned values. It also gives monotonicity in the pins. For any [increasing observable](../../../set.md#increasing-function-on-a-partially-ordered-set) $f$, [positive association of random variables](../../../probability-theory.md#positive-association-of-random-variables) with an unpinned [Ising spin](../../../statistical-physics.md#ising-spin-variable) $\omega(z)$ gives

$$
E[f\mid\omega(z)=1]\ge E[f\mid\omega(z)=0].
$$

Both [conditional probabilities](../../../probability-theory.md#conditional-probability) are positive. The same inequality holds after other [Ising spins](../../../statistical-physics.md#ising-spin-variable) have been pinned. Changing pins one at a time proves [stochastic domination](../../../probability-and-statistics.md#stochastic-domination-of-probability-measures) of the measures as $\zeta$ increases.

Now let $\Lambda\subset\Lambda'$ and take an [increasing observable](../../../set.md#increasing-function-on-a-partially-ordered-set) depending on a fixed set inside the smaller box. Given the [Ising spins](../../../statistical-physics.md#ising-spin-variable) on $\partial\Lambda$, the larger-box measure induces precisely the smaller-box interior law with those boundary values: nearest-neighbor interactions cannot see farther once this boundary is fixed. Its conditional law is therefore between the all-zero and all-one smaller-box laws. Averaging yields

$$
\mu_\Lambda^0(f)\le\mu_{\Lambda'}^0(f),\qquad
\mu_{\Lambda'}^1(f)\le\mu_\Lambda^1(f).
$$

These are bounded monotone sequences along any increasing box exhaustion.

For every finite set $S$, the event that all [Ising spins](../../../statistical-physics.md#ising-spin-variable) in $S$ are one is increasing, so its [probability](../../../probability-theory.md#probability) converges in both boundary sequences. [Probabilities](../../../probability-theory.md#probability) of arbitrary finite zero/one patterns are finite [inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle) combinations of these all-one [probabilities](../../../probability-theory.md#probability), and hence converge too. The limits are consistent [finite-dimensional distributions](../../../stochastic-process.md#finite-dimensional-distribution); they define measures on $\{0,1\}^{\mathbb Z^d}$ and give [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) in the [product topology](../../../geometry-and-topology.md#product-topology). Thus **both [extremal infinite-volume Ising measures](../../../statistical-physics.md#extremal-infinite-volume-ising-measures) $\mu^0,\mu^1$ exist**, with $\mu^0$ below $\mu^1$ in [stochastic domination](../../../probability-and-statistics.md#stochastic-domination-of-probability-measures). This argument proves existence even when the two limits are different.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Set $L=\inf_{k\ge1}x_k/k$. It may be $-\infty$, but cannot be $+\infty$ because $x_1$ is finite. Fix $k$ and write $n=qk+r$, $0\le r<k$. Repeated use of the [subadditive sequence](../../../real-analysis.md#subadditive-sequence) inequality gives

$$
x_n\le qx_k+C_k,\qquad C_k=\max(0,x_1,\ldots,x_{k-1}),
$$

where $C_1=0$. Dividing by $n$ and letting $n\to\infty$ gives $\limsup x_n/n\le x_k/k$. Since this holds for every $k$, the upper [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) is at most $L$, while every ratio is at least $L$. If $L$ is finite these bounds agree. If $L=-\infty$, choose $k$ with $x_k/k$ below any prescribed real number; the same upper-limit bound proves convergence to $-\infty$. This establishes the [extended-real Fekete lemma](../../../real-analysis.md#fekete-s-lemma):

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\ge1}\frac{x_k}{k}\in[-\infty,\infty).}
$$

A finite real [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) requires a lower linear bound. For example $x_n=-n^2$ satisfies the premise but has normalized [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) $-\infty$, so that qualification cannot be dropped.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $\phi=\phi^1_{p,q}$ and $C_n=\phi(0\leftrightarrow e_n)$. We use these standard facts about the [infinite-volume wired random-cluster measure](../../../site-percolation.md#infinite-volume-wired-random-cluster-measure) for $q\ge1$: it is translation invariant and invariant under coordinate reflections/permutations; it has [positive association of the random-cluster model](../../../site-percolation.md#positive-association-of-the-random-cluster-model); and every conditional edge-open [probability](../../../probability-theory.md#probability) is at least

$$
r=\frac{p}{p+q(1-p)}>0.
$$

The last bound follows because an [edge](../../../graph-theory.md#edge-of-a-graph) either leaves its component count unchanged on opening, giving [probability](../../../probability-theory.md#probability) $p$, or merges two components, giving $p/(p+q(1-p))$. These are standard infinite-volume properties of the limit obtained from the finite wired laws by [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures). [Positive association of random variables](../../../probability-theory.md#positive-association-of-random-variables) applies to connection events by increasing approximation with finite-path events.

Opening the $n$ [edges](../../../graph-theory.md#edge-of-a-graph) of the straight segment gives $C_n\ge r^n$, so its logarithm is finite. The events $A=\{0\leftrightarrow e_m\}$ and $B=\{e_m\leftrightarrow e_{m+n}\}$ are increasing, and their intersection implies connection to $e_{m+n}$. Thus

$$
C_{m+n}\ge\phi(A\cap B)\ge\phi(A)\phi(B)=C_mC_n.
$$

The sequence $a_n=-\log C_n$ is a [subadditive sequence](../../../real-analysis.md#subadditive-sequence), with $0\le a_n\le-n\log r$. Part (a) proves the [random-cluster inverse correlation length](../../../site-percolation.md#random-cluster-inverse-correlation-length) exists and is finite:

$$
\boxed{\alpha(p,q)=\lim_n\frac{a_n}{n}=\inf_n\frac{a_n}{n}\in[0,-\log r].}
$$

Since $a_n/n\ge\alpha$ for every $n$, exponentiating yields the requested bound

$$
\boxed{\phi^1_{p,q}(0\leftrightarrow e_n)\le e^{-n\alpha(p,q)}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $B_n=\phi(0\leftrightarrow\partial\Lambda_n)$ and $s_n=|\partial\Lambda_n|$. This connection event is the union over $x\in\partial\Lambda_n$ of $\{0\leftrightarrow x\}$. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore supplies a [graph vertex](../../../graph.md#vertex-graph-theory) with connection [probability](../../../probability-theory.md#probability) at least $B_n/s_n$.

Every boundary [graph vertex](../../../graph.md#vertex-graph-theory) has some coordinate equal to $n$ or $-n$. By applying a [permutation](../../../combinatorics.md#permutation) and a [graph automorphisms](../../../graph.md#graph-automorphism), which preserve both the law and the boundary, choose such a [graph vertex](../../../graph.md#vertex-graph-theory) in the form $x=(n,x_2,\ldots,x_d)$ while retaining its [probability](../../../probability-theory.md#probability) bound. Now $e_{2n}-x=(n,-x_2,\ldots,-x_d)$ is a reflection of $x$. Translation and reflection invariance give

$$
\phi(x\leftrightarrow e_{2n})=\phi(0\leftrightarrow e_{2n}-x)=\phi(0\leftrightarrow x).
$$

[Positive association of random variables](../../../probability-theory.md#positive-association-of-random-variables) applied to the two connection events, whose intersection implies $0\leftrightarrow e_{2n}$, proves the [reflection comparison of random-cluster connections](../../../site-percolation.md#reflection-comparison-of-random-cluster-connections):

$$
\boxed{C_{2n}\ge\phi(0\leftrightarrow x)^2,\qquad
\phi(0\leftrightarrow x)\ge B_n/s_n.}
$$

Also $C_n\le B_n$, since any path to $e_n$ meets the box boundary. Consequently

$$
C_n\le B_n\le s_n\sqrt{C_{2n}},
$$

and hence

$$
-\frac1{2n}\log C_{2n}-\frac{\log s_n}{n}
\le-\frac1n\log B_n
\le-\frac1n\log C_n.
$$

Here $s_n=(2n+1)^d-(2n-1)^d=O(n^{d-1})$, so $\log s_n/n\to0$. Both outside logarithmic connection rates converge to $\alpha(p,q)$ by part (b). Squeezing gives the rate for every box size, and therefore for the requested even subsequence:

$$
\boxed{-\frac1{2n}\log\phi^1_{p,q}(0\leftrightarrow\partial\Lambda_{2n})\longrightarrow\alpha(p,q).}
$$

## 5

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

In [bond percolation](../../../bond-percolation.md) on $\mathbb Z^d$, [edges](../../../graph-theory.md#edge-of-a-graph) are independently open with [probability](../../../probability-theory.md#probability) $p$ and closed otherwise. An open [percolation cluster](../../../bond-percolation.md#percolation-cluster) is a connected component using only open [edges](../../../graph-theory.md#edge-of-a-graph). In [site percolation](../../../site-percolation.md) it is the [graph vertices](../../../graph.md#vertex-graph-theory) that are independently declared open. The [percolation probability](../../../probability-theory.md#percolation-probability) $\theta(p)=P_p(0\leftrightarrow\infty)$ measures the chance that the origin lies in an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster), and the [percolation critical probability](../../../probability-theory.md#percolation-critical-probability) is $p_c=\inf\{p:\theta(p)>0\}$. [Monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation) by independent [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) makes $\theta$ nondecreasing.

The [sharpness of the percolation transition](../../../probability-theory.md#sharpness-of-the-percolation-transition) says that below $p_c$ connection [probabilities](../../../probability-theory.md#probability) on $\mathbb Z^d$ decay exponentially with distance, while above $p_c$ the percolation [probability](../../../probability-theory.md#probability) is positive. There is almost surely a unique [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) in the supercritical regime. On the [square lattice](../../../graph.md#square-lattice), the [Harris-Kesten theorem](../../../probability-theory.md#harris-kesten-theorem) gives bond threshold $1/2$, and there is no [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) at [percolation critical probability](../../../probability-theory.md#percolation-critical-probability). The emergence of connections on arbitrarily large scales is the geometric meaning of the [phase transition](../../../critical-phenomenon.md#phase-transition).

Several observables describe this singular behavior. The [percolation susceptibility](../../../bond-percolation.md#percolation-susceptibility) is $\chi(p)=E_p|C(0)|$ for $p<p_c$. A directional [correlation length](../../../critical-phenomenon.md#correlation-length) can be defined through exponential two-point decay, $\xi(p)^{-1}=-\lim_n n^{-1}\log P_p(0\leftrightarrow ne_1)$. [Percolation critical exponents](../../../critical-phenomenon.md#percolation-critical-exponents) describe leading powers, conveniently defined logarithmically rather than requiring exact asymptotic amplitudes:

$$
\theta(p)=(p-p_c)^{\beta+o(1)},\quad
\chi(p)=(p_c-p)^{-\gamma+o(1)},\quad
\xi(p)=(p_c-p)^{-\nu+o(1)}.
$$

The first [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) approaches from above, the other two from below. At [percolation critical probability](../../../probability-theory.md#percolation-critical-probability), [percolation two-point connection probability](../../../bond-percolation.md#percolation-two-point-connection-probability) is expected to have leading power $|x|^{-(d-2+\eta)}$, and the number per site of [percolation clusters](../../../bond-percolation.md#percolation-cluster) of size $s$ has leading power $s^{-\tau}$. This cluster-count [probability distribution](../../../probability-theory.md#probability-distribution) differs from the size-biased [probability distribution](../../../probability-theory.md#probability-distribution) seen by choosing a site. [Scaling relations for critical exponents](../../../critical-phenomenon.md#scaling-relation-for-critical-exponents) such as $\gamma=(2-\eta)\nu$ and $2\beta+\gamma=d\nu$ connect the exponents in their applicable scaling regime; [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation) is not valid above the [upper critical dimension of percolation](../../../critical-phenomenon.md#upper-critical-dimension-of-percolation) in ordinary mean-field regimes.

The [percolation universality hypothesis](../../../critical-phenomenon.md#percolation-universality-hypothesis) predicts that dimension and large-scale symmetry, rather than microscopic [graph](../../../graph.md) details, determine these exponents and scaling functions. Thus square-lattice bond and triangular-lattice site models are expected to share the [planar graph](../../../graph-theory.md#planar-graph) [universality class](../../../critical-phenomenon.md#universality-class) despite different microscopic definitions. Universality does not mean identical critical [probabilities](../../../probability-theory.md#probability), amplitudes or finite-lattice distributions. Exact values and existence of exponents require model-specific theorems, not merely this prediction.

Two dimensions have an additional structure: [conformal maps](../../../geometry-and-topology.md#conformal-map) preserve angles, and critical crossing [probabilities](../../../probability-theory.md#probability) are expected to be unchanged under conformal transport of the domain and its marked boundary arcs. A crossing [probability](../../../probability-theory.md#probability) then depends only on the conformal shape of that marked quadrilateral. The [Cardy boundary crossing formula](../../../stochastic-process.md#cardy-boundary-crossing-formula) gives this dependence in terms of its boundary cross ratio. For critical triangular-lattice site percolation, conformal invariance and the resulting exponents are established; examples are $\beta=5/36$, $\gamma=43/18$, $\nu=4/3$, with the rigorous statements in leading-power form. These values are summarized in [Smirnov and Werner's original paper](https://www.unige.ch/~smirnov/papers/smw-j.pdf). Their universality extension to arbitrary planar lattices should not be presented as the same theorem.

An exploration path separating the two colors, with opposite boundary colors on two arcs, has a [domain Markov property of a percolation exploration](../../../site-percolation.md#domain-markov-property-of-a-percolation-exploration): conditional on the explored portion, the unexplored colors retain their independent laws with the newly exposed boundary colors. Conformal invariance, this domain Markov property and suitable regularity lead to [Schramm–Loewner evolution](../../../stochastic-process.md#schramm-loewner-evolution). In the upper half-plane its chordal equation is

$$
\partial_tg_t(z)=\frac2{g_t(z)-U_t},\qquad U_t=\sqrt\kappa\,B_t,
$$

where $B_t$ is standard [Brownian motion](../../../brownian-motion.md) and time is normalized by half-plane capacity. Critical percolation corresponds to $\kappa=6$. Thus the complicated discrete interface becomes a conformally natural random curve driven by one real [Brownian motion](../../../brownian-motion.md). Its crossing and arm [probabilities](../../../probability-theory.md#probability) supply critical exponents and, through [scaling relations for critical exponents](../../../critical-phenomenon.md#scaling-relation-for-critical-exponents), near-critical singularities. This makes conformal methods predictive tools for the transition, rather than only descriptions of an interface's appearance.

## 6

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

In the [voter model](../../../stochastic-process.md#voter-model) on $\mathbb Z^2$, each site has a rate-one [Poisson process](../../../probability-theory.md#poisson-process) clock; when it rings, that site copies one of its four neighbors, chosen uniformly. States are zero or one. For a [cylinder function](../../../geometry-and-topology.md#cylinder-function-on-a-product-space) $f$, the local [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) is

$$
Lf(\eta)=\sum_x\frac14\sum_{y\sim x}\bigl[f(\eta^{x\leftarrow y})-f(\eta)\bigr],
$$

where $\eta^{x\leftarrow y}$ agrees with $\eta$ except that the [voter model](../../../stochastic-process.md#voter-model) opinion at $x$ is replaced by the [voter model](../../../stochastic-process.md#voter-model) opinion at $y$. Only sites in the support of $f$ contribute, so this [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) sum is finite.

The [voter-model duality](../../../stochastic-process.md#voter-model-duality) comes from independent [Poisson processes](../../../probability-theory.md#poisson-process) of copying arrows of rate $1/4$ on each ordered neighboring pair. Trace the ancestors of specified sites backwards from time $t$: each ancestral line is a rate-one [continuous-time random walk](../../../markov-process.md#continuous-time-random-walk) with uniform nearest-neighbor steps, and lines coalesce when they meet. The [voter model](../../../stochastic-process.md#voter-model) opinions at time $t$ are the initial [voter model](../../../stochastic-process.md#voter-model) opinions at those ancestral locations. This construction also explains the general duality theorem being used.

Two ancestral walks on $\mathbb Z^2$ meet almost surely. Until their meeting, their difference is a rate-two symmetric nearest-neighbor walk, and [simple random walk in two dimensions is recurrent](../../../markov-process.md#simple-random-walk-in-two-dimensions-is-recurrent). If $\tau_{xy}$ is their meeting time, this gives

$$
P_\nu(\xi_t(x)\ne\xi_t(y))\le P(\tau_{xy}>t)\longrightarrow0
$$

for every initial law $\nu$. If $\nu$ is invariant, the left side is the fixed [probability](../../../probability-theory.md#probability) $\nu(\eta(x)\ne\eta(y))$, so it is zero. This holds for every pair. Countability then implies that $\nu$ is concentrated on configurations with all [voter model](../../../stochastic-process.md#voter-model) opinions equal. Both constant configurations are [absorbing state](../../../markov-process.md#absorbing-state). Thus the [invariant measures of the two-dimensional voter model](../../../stochastic-process.md#invariant-measures-of-the-two-dimensional-voter-model) are exactly

$$
\boxed{\nu=\alpha\delta_0+(1-\alpha)\delta_1,\qquad0\le\alpha\le1.}
$$

No translation-invariance assumption on $\nu$ was used.

For the last assertion, let the initial set of one-valued opinions $F$ be finite. Single-line duality gives

$$
P(\xi_t(x)=1)=P_x(X_t\in F)=\sum_{z\in F}p_t(x,z).
$$

Each [transition probability](../../../markov-process.md#transition-probability) tends to zero. One direct verification is the [Fourier transform](../../../analysis.md#fourier-transform) for the rate-one walk:

$$
p_t(x,z)=\frac1{(2\pi)^2}\int_{[-\pi,\pi]^2}
 e^{-ik\cdot(z-x)}\exp\left[-t\left(1-\tfrac12(\cos k_1+\cos k_2)\right)\right]dk.
$$

The integrand has modulus at most one and tends to zero except at the single point $k=0$; [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) proves the claim. For any finite observation set $K$, the [union bound](../../../probability-inequality.md#boole-s-inequality) now gives

$$
P(\xi_t\text{ has a one somewhere in }K)
\le\sum_{x\in K}\sum_{z\in F}p_t(x,z)\longrightarrow0.
$$

Therefore every finite [voter model](../../../stochastic-process.md#voter-model) opinion pattern converges in law to the all-zero pattern. These cylinder distributions determine [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) in the compact [product topology](../../../geometry-and-topology.md#product-topology), proving **finite-seed local extinction in the [voter model](../../../stochastic-process.md#voter-model)** and

$$
\boxed{\mathcal L(\xi_t)\Longrightarrow\delta_0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
