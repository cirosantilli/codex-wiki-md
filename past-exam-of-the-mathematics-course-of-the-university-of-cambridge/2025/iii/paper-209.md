# Paper 209

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_209.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_209.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c1](#1/c1)
    - [Solution](#1/c1/solution)
  - [c2](#1/c2)
    - [Solution](#1/c2/solution)
  - [d1](#1/d1)
    - [Solution](#1/d1/solution)
  - [d2](#1/d2)
    - [Solution](#1/d2/solution)
- [2](#2)
  - [a1](#2/a1)
    - [Solution](#2/a1/solution)
  - [a2](#2/a2)
    - [Solution](#2/a2/solution)
  - [a3](#2/a3)
    - [Solution](#2/a3/solution)
  - [a4](#2/a4)
    - [Solution](#2/a4/solution)
  - [b1](#2/b1)
    - [Solution](#2/b1/solution)
  - [b2](#2/b2)
    - [Solution](#2/b2/solution)
  - [b3](#2/b3)
    - [Solution](#2/b3/solution)
  - [b4](#2/b4)
    - [Solution](#2/b4/solution)
  - [b5](#2/b5)
    - [Solution](#2/b5/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [A1](#5/a1)
    - [Solution](#5/a1/solution)
  - [A2](#5/a2)
    - [Square](#5/a2/square)
      - [Solution](#5/a2/square/solution)
    - [Segment](#5/a2/segment)
      - [Solution](#5/a2/segment/solution)
  - [B1](#5/b1)
    - [Solution](#5/b1/solution)
  - [B2](#5/b2)
    - [Solution](#5/b2/solution)
  - [B3](#5/b3)
    - [Solution](#5/b3/solution)
  - [B4](#5/b4)
    - [Solution](#5/b4/solution)

## 1

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

It suffices to use the two-dimensional coordinate half-plane inside $H$. A [Peierls argument](../../../probability-theory.md#peierls-argument) shows that when $p$ is sufficiently close to one, the probability that a fixed open vertex is separated from distance $n$ by a closed dual contour is summable over contour lengths: the number of length-$m$ contours is at most exponential in $m$, whereas each is closed with probability $(1-p)^m$. Hence the origin has positive probability of belonging to an infinite open cluster. The event that some infinite cluster exists is invariant and therefore has probability zero or one because the boundary translation is an [ergodic transformation](../../../measure-theory.md#ergodicity); its positive probability makes it almost sure. The same cluster is also an infinite cluster of $H$ in every $d\geq2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Translation by $e=(0,1,0,\ldots,0)$ preserves $H$, so $(\omega(x+e):x\in H)$ has the same independent Bernoulli-$p$ law as $\omega$. This shift is ergodic, and the number $N$ of infinite clusters is shift-invariant. Thus $N=k_0$ almost surely for some deterministic $k_0\in\mathbb N\cup\{\infty\}$.

Suppose $2\leq k_0<\infty$. With positive probability a finite box meets all $k_0$ infinite clusters. By the [finite-energy property of Bernoulli percolation](../../../probability-theory.md#finite-energy-property-of-bernoulli-percolation), forcing finitely many sites in the box open has positive conditional probability and joins those clusters without affecting infinity outside the box. The resulting configuration has fewer than $k_0$ infinite clusters on an event of positive probability, contradicting the almost-sure constancy. Hence $k_0\in\{0,1,\infty\}$.

<h3 id="1/c1">c1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c1/solution">Solution</h4>

↑ **Parent:** [C1](#1/c1)

Use independent percolation configurations in $H$ and in its reflected copy $H'=(-\infty,-2]\times\mathbb Z^{d-1}$. Require event $A$ in both copies and close the intervening site $(-1,0,\ldots,0)$. This has probability $(1-p)Q^2$. Because either distinguished infinite cluster meets its boundary hyperplane only at its distinguished origin, the closed intervening site prevents it from leaving its own half-space. The resulting whole-space configuration therefore has two distinct infinite clusters. Whole-space supercritical Bernoulli percolation has an almost surely unique infinite cluster, so $(1-p)Q^2=0$ and hence $Q=0$.

<h3 id="1/c2">c2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c2/solution">Solution</h4>

↑ **Parent:** [C2](#1/c2)

Fix the finite set $S=\{x_1,\ldots,x_n\}\subset B$. If an infinite half-space cluster met $B$ exactly in $S$ with positive probability, take independent reflected occurrences in $H$ and $H'$ and force the finitely many intervening sites adjacent to $S$ closed. The [finite-energy property of Bernoulli percolation](../../../probability-theory.md#finite-energy-property-of-bernoulli-percolation) gives this combined event positive probability, while it creates two distinct whole-space infinite clusters, contradicting uniqueness. Thus the probability is zero for every finite $S$. Since $B$ has only countably many finite subsets, almost surely every infinite cluster that meets $B$ meets it infinitely often.

<h3 id="1/d1">d1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d1/solution">Solution</h4>

↑ **Parent:** [D1](#1/d1)

By part (c2), $C\cap B_{n_0+1}$ is infinite almost surely. For each $x$ in this intersection, its neighbor $x-e_1\in B_{n_0}$ is open independently with probability $p$. The probability that all infinitely many such neighbors are closed is zero. Hence some open site of $B_{n_0}$ is adjacent to $C$, and the open cluster $C'$ containing their union in $H_{n_0}$ is infinite, contains $C$, and intersects $B_{n_0}$.

<h3 id="1/d2">d2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d2/solution">Solution</h4>

↑ **Parent:** [D2](#1/d2)

If an infinite cluster $C$ avoids $B$, the set of first coordinates of its vertices has a least value $n_0\geq1$. Then $C$, viewed in $H_{n_0}$, intersects $B_{n_0}$. Repeated application of part (d1) embeds it in an infinite cluster of $H_{n_0-1}$ meeting $B_{n_0-1}$, eventually producing an infinite cluster of $H$ meeting $B$. Because each enlarged cluster contains $C$, already the first step contradicts the minimality of $n_0$. Thus such a cluster has probability zero.

## 2

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="2/a1">a1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a1/solution">Solution</h4>

↑ **Parent:** [A1](#2/a1)

For each $x\in H_N$, the event that $x$ belongs to an infinite open cluster implies that $x$ has an open path to $h_N$. Translation invariance gives probability $\theta$ for the former event. Therefore

$$
\boxed{\mathbb E\#C_N=\sum_{x\in H_N}\mathbb P(x\in C_N)
\geq\theta\#H_N.}
$$

<h3 id="2/a2">a2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a2/solution">Solution</h4>

↑ **Parent:** [A2](#2/a2)

Write $M=\#H_N$, $X=\#C_N$, and $q=\mathbb P(X\geq\theta M/2)$. Since $0\leq X\leq M$,

$$
\theta M\leq\mathbb EX
\leq\frac{\theta M}{2}(1-q)+Mq.
$$

**Thus $q\geq(\theta/2)/(1-\theta/2)\geq\theta/2$.**

<h3 id="2/a3">a3</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a3/solution">Solution</h4>

↑ **Parent:** [A3](#2/a3)

Both $\{\#C_N\geq\theta\#H_N/2\}$ and $\{0\in C_N\}$ are increasing events. The first has probability at least $\theta/2$ by part (a2), while the second has probability at least $\theta$ because an infinite origin cluster reaches $h_N$. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) gives

$$
\boxed{\mathbb P(A_N)\geq\frac{\theta}{2}\theta=\frac{\theta^2}{2}.}
$$

<h3 id="2/a4">a4</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a4/solution">Solution</h4>

↑ **Parent:** [A4](#2/a4)

On $A_N$, additionally require every site of $h_{N+1}$ to be open and every site of $h_{N+2}$ to be closed. The open ring joins every component of $C_N$ to the origin component, and the closed outer ring makes that component finite. It contains at least $\theta\#H_N/2$ sites. These ring states are independent of $A_N$, and their probability is

$$
p^{\#h_{N+1}}(1-p)^{\#h_{N+2}}.
$$

Since both ring sizes are linear in $N$, this is at least $c(p)e^{-u(p)N}$. Multiplication by $\mathbb P(A_N)\geq\theta^2/2$ proves the claimed lower bound.

<h3 id="2/b1">b1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b1/solution">Solution</h4>

↑ **Parent:** [B1](#2/b1)

The variables $\omega'(x)=1-\omega(x)$ are independent Bernoulli variables with parameter $1-p<1/2$. They therefore form subcritical site percolation on the triangular lattice; their open clusters are precisely the closed-site clusters of the original configuration.

<h3 id="2/b2">b2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b2/solution">Solution</h4>

↑ **Parent:** [B2](#2/b2)

A closed circuit of diameter at least $n$ through a fixed listed point contains a closed path from that point to graph distance at least $n/2$. [Exponential decay of subcritical percolation](../../../probability-theory.md#exponential-decay-of-subcritical-percolation) bounds this probability by $Ce^{-cn}$. A union bound over the $n$ listed points gives

$$
\mathbb P(B_n)\leq Cn e^{-cn}\leq n e^{-u n}
$$

after reducing $u>0$ and adjusting finitely many small $n$.

<h3 id="2/b3">b3</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b3/solution">Solution</h4>

↑ **Parent:** [B3](#2/b3)

A closed circuit surrounding the origin and passing through $(m,0)$ has diameter at least $m$. By the one-point estimate used in part (b2), its probability is at most $Ce^{-cm}$. Therefore

$$
\boxed{\mathbb P(\exists m\geq n\text{ on such a circuit})
\leq\sum_{m\geq n}Ce^{-cm}
\leq C'e^{-c'n}.}
$$

<h3 id="2/b4">b4</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b4/solution">Solution</h4>

↑ **Parent:** [B4](#2/b4)

By planar duality on the triangular lattice, a finite open cluster containing the origin is surrounded by a closed circuit. If its diameter exceeds $n$, an outermost surrounding circuit reaches distance of order $n$ and crosses the positive coordinate ray at some $(m,0)$ with $m\geq c n$. Part (b3), with constants rescaled, therefore gives

$$
\boxed{\mathbb P(0\text{ lies in a finite open cluster of diameter}>n)
\leq Ce^{-cn}.}
$$

<h3 id="2/b5">b5</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b5/solution">Solution</h4>

↑ **Parent:** [B5](#2/b5)

A connected set of at least $m$ triangular-lattice sites has diameter at least $c_0\sqrt m$. Part (b4) gives

$$
\mathbb P(0\text{ lies in a finite cluster with at least }m\text{ sites})
\leq Ce^{-c c_0\sqrt m}
\leq e^{-v\sqrt m}
$$

after reducing $v$ to absorb small $m$. Since $\#H_N$ is of order $N^2$, the lower bound in part (a4) is also of order $e^{-C\sqrt m}$. The upper and lower bounds therefore identify the correct stretched-exponential exponent $\sqrt m$.

## 3

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a finite graph $G=(V,E)$, the $q=2$ [random-cluster model](../../../site-percolation.md#random-cluster-model) is

$$
\phi_{p,2}(\omega)=\frac1Z
p^{o(\omega)}(1-p)^{|E|-o(\omega)}2^{k(\omega)},
$$

where $o(\omega)$ is the number of open edges and $k(\omega)$ the number of open connected components. In the [Edwards-Sokal coupling](../../../site-percolation.md#edwards-sokal-coupling), first sample $\omega$, assign an independent uniform spin $\pm1$ to each open cluster, and give every vertex its cluster's spin. The resulting spin law is the [Ising model](../../../statistical-physics.md#ising-model) with

$$
p=1-e^{-2\beta}.
$$

Conversely, from an Ising configuration, close every edge joining unequal spins and independently open each edge joining equal spins with probability $p$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the single-edge [heat-bath Markov chain](../../../site-percolation.md#heat-bath-markov-chain): choose an edge uniformly and resample it from its conditional random-cluster law. If its endpoints are already connected without that edge, its conditional open probability is $p$; otherwise opening it merges two components and the probability is

$$
\frac p{p+2(1-p)}=\frac p{2-p}.
$$

Detailed balance makes $\phi_{p,2}$ stationary. Driving this chain and Bernoulli heat-bath chains by the same update edges and uniforms gives the stochastic domination

$$
\boxed{\operatorname{Ber}\left(\frac p{2-p}\right)^{\otimes E}
\preceq\phi_{p,2}\preceq
\operatorname{Ber}(p)^{\otimes E}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The conditional open probability in part (b) is increasing in the states of all other edges, because adding edges can only connect the two endpoints. A common-uniform update therefore preserves the coordinatewise order. Start two copies from all closed and use the same updates, with the second copy additionally conditioned through an increasing event $B$ by the corresponding monotone censored heat-bath chain. The monotone grand coupling and convergence to stationarity show that conditioning on $B$ stochastically increases the configuration. Hence for increasing $A$,

$$
\phi_{p,2}(A\mid B)\geq\phi_{p,2}(A),
$$

which is the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) $\phi(A\cap B)\geq\phi(A)\phi(B)$. Applying this to the complement of a decreasing event $B'$ gives

$$
\boxed{\phi(A\cap B')\leq\phi(A)\phi(B').}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Couple the free-boundary random-cluster heat-bath chains in $\Lambda_N$ and $\Lambda_{N+1}$. Restricted to common edges, the larger box has extra possible open paths through its outer annulus. These can only turn a disconnected-endpoint update into a connected-endpoint update and raise its open probability from $p/(2-p)$ to $p$. The monotone coupling therefore gives

$$
P_N\preceq P_{N+1}
$$

on common increasing events. Consequently $P_N(A)$ is nondecreasing and, being bounded by one, has a limit.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The stochastic bounds from part (b) hold uniformly in every box. Passing to the increasing limit for the local increasing event $A$ gives

$$
\mathbb P_{p/(2-p)}^{\mathrm{bond}}(A)
\leq\lim_{N\to\infty}P_N(A)
\leq\mathbb P_p^{\mathrm{bond}}(A).
$$

**Thus the infinite-volume free random-cluster measure lies stochastically between Bernoulli bond percolation at parameters $p/(2-p)$ and $p$.**

## 4

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Root the graph at $x_0$ and let $P^{(0)}$ be the transition matrix of simple random walk killed on hitting $x_0$, indexed by the remaining vertices. Its Green matrix is $G=(I-P^{(0)})^{-1}$. Successively eliminating vertices in an order $x_1,\ldots,x_n$ takes [Schur complements](../../../linear-algebra.md#schur-complement); the corresponding diagonal pivot at step $j$ is exactly $g_{D\setminus\{x_0,\ldots,x_{j-1}\}}(x_j)$. The product of the pivots is therefore

$$
\det G=\frac1{\det(I-P^{(0)})},
$$

which is invariant under the elimination order.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The reduced graph Laplacian is $L^{(0)}=\Delta(I-P^{(0)})$. By the [matrix-tree theorem](../../../combinatorics.md#kirchhoff-s-theorem), the number $\tau(D)$ of spanning trees is

$$
\tau(D)=\det L^{(0)}=\Delta^n\det(I-P^{(0)}).
$$

Combining this with part (a) gives

$$
\prod_{j=1}^n g_{D\setminus\{x_0,\ldots,x_{j-1}\}}(x_j)
=\frac{\Delta^n}{\tau(D)}.
$$

This is also the normalization behind [Wilson algorithm](../../../combinatorics.md#wilson-s-algorithm): loop-erased random walks attach the vertices successively, and the order-independent product ensures that every rooted spanning tree has probability $1/\tau(D)$.

## 5

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="5/a1">A1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a1/solution">Solution</h4>

↑ **Parent:** [A1](#5/a1)

The continuum [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) $\Gamma$ on $\mathbb R^3$ is the centered Gaussian random distribution indexed by smooth compactly supported test functions, with covariance

$$
\mathbb E[\Gamma(f)\Gamma(g)]
=\iint_{\mathbb R^3\times\mathbb R^3}
f(x)G(x,y)g(y)dxdy,
\qquad
G(x,y)=\frac{c_3}{|x-y|},
$$

where $G$ is the Green kernel of $-\Delta$. Equivalently, its covariance operator is $(-\Delta)^{-1}$.

<h3 id="5/a2">A2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a2/square">Square</h4>

↑ **Parent:** [A2](#5/a2)

<h5 id="5/a2/square/solution">Solution</h5>

↑ **Parent:** [Square](#5/a2/square)

A finite measure $\mu$ can index the field when its [Green energy](../../../stochastic-process.md#green-energy)

$$
\iint G(x,y)d\mu(x)d\mu(y)
$$

is finite. On the two-dimensional square, the singularity is locally integrable because polar area contributes $r\,dr$ while $G$ contributes $1/r$. The near-diagonal integral is therefore proportional to $\int_0^\varepsilon dr<\infty$, and the mean $\Gamma(\mu)$ is a well-defined centered Gaussian random variable.

<h4 id="5/a2/segment">Segment</h4>

↑ **Parent:** [A2](#5/a2)

<h5 id="5/a2/segment/solution">Solution</h5>

↑ **Parent:** [Segment](#5/a2/segment)

On the segment the energy contains

$$
c_3\int_0^1\int_0^1\frac{ds\,dt}{|s-t|},
$$

which diverges logarithmically along the diagonal. The uniform segment measure therefore has infinite Green energy, so its mean cannot be defined as an $L^2$ Gaussian-field pairing.

<h3 id="5/b1">B1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b1/solution">Solution</h4>

↑ **Parent:** [B1](#5/b1)

The restriction and normalization make $\mu$ the unique conformal-restriction loop measure surrounding the origin, up to the fixed multiplicative normalization. By the classification of planar conformal restriction measures, it is the image of the rooted [Brownian loop measure](../../../brownian-motion.md#brownian-loop-measure) at the origin under the map taking a Brownian loop to its outer boundary. It is scale invariant and sigma-finite, with finite mass after imposing lower and upper diameter cutoffs.

<h3 id="5/b2">B2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b2/solution">Solution</h4>

↑ **Parent:** [B2](#5/b2)

For every bounded simply connected $D$, translation $z\mapsto z+x$ is a conformal map from $D$ to $D+x$. Conformal restriction says that translating $\rho_D$ gives $\rho_{D+x}$. Exhausting the plane by such domains proves that the whole measure $\rho$ is translation invariant. Consequently

$$
\mu_x=(T_x)_*\mu,
$$

where $T_x(\gamma)=\gamma+x$ and $\mu_x$ restricts $\rho$ to loops surrounding $x$.

<h3 id="5/b3">B3</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b3/solution">Solution</h4>

↑ **Parent:** [B3](#5/b3)

Part (B1) and the stated normalization determine $\mu$, and part (B2) then determines every $\mu_x$. Every self-avoiding loop surrounds some rational point. Since $\mathbb Q^2$ is countable, the restrictions of $\rho$ to loops surrounding rational points determine $\rho$ on the entire loop space, with overlaps already consistent because they arise from the same conformal-restriction law. Hence an existing normalized $\rho$ is unique.

<h3 id="5/b4">B4</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b4/solution">Solution</h4>

↑ **Parent:** [B4](#5/b4)

Restrict $\mu_x$ to outer boundaries that stay in $D$ and surround $y$. By part (B1), this is the image under outer-boundary formation of rooted Brownian loops through $x$ whose outer boundary stays in $D$ and surrounds $y$. But this restriction is exactly the restriction of $\rho_D$ to loops surrounding both $x$ and $y$. Interchanging $x$ and $y$ gives the same intrinsic restriction of $\rho_D$, so it can equally be represented by outer boundaries of Brownian loops rooted at $y$ that surround $x$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
