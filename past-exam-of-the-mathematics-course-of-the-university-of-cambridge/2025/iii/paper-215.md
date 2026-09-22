# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_215.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A randomized stopping time $\tau$ is a [strong stationary time](../../../markov-process.md#strong-stationary-time) when

$$
\mathbb P_x(X_\tau=y,\tau=t)=\pi(y)\mathbb P_x(\tau=t)
$$

for every initial state $x$, state $y$, and time $t$. Equivalently, $X_\tau$ has distribution $\pi$ and is independent of $\tau$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

One shuffle removes the ordered top $k$ cards and inserts them, in a uniformly random person-order, into successively chosen uniform slots. The transition rule depends on a deck only through relabeling of its cards, so its transition matrix on the [symmetric group](../../../finite-group-theory.md#symmetric-group) is doubly stochastic. Hence the uniform distribution on all $n!$ permutations is invariant.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Reverse time under the uniform invariant law. The reverse shuffle selects $k$ cards uniformly without replacement and moves them to the top in random order. Track cards once selected. The forward time $\tau$ at which the initially bottom card first lies among the next top $k$ corresponds in reverse to the first time every card has been selected. At that [coupon-collector](../../../discrete-probability-distribution.md#coupon-collector-problem) time, the order of all marked cards is uniform and independent of the marking time, by induction over the random insertions. Reversing again shows that $X_\tau$ is uniform and independent of $\tau$, so part (a) makes $\tau$ a strong stationary time.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

In the reverse description, a fixed card avoids selection in one shuffle with probability $1-k/n$. After $t$ shuffles, a union bound gives

$$
\mathbb P(\tau>t)
\leq n(1-k/n)^t
\leq ne^{-kt/n}.
$$

For a strong stationary time, the [separation distance](../../../markov-process.md#separation-distance) and hence [total variation distance](../../../probability-and-statistics.md#total-variation-distance) at time $t$ are at most $\mathbb P(\tau>t)$. Taking

$$
t=\frac nk\log n+\frac nk\log(1/\varepsilon)
$$

makes this at most $\varepsilon$. Since $k\geq1$, the second term is at most $C(\varepsilon)n$, proving

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)
\leq\frac nk\log n+C(\varepsilon)n.}
$$

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

With stationary flow $Q(x,y)=\pi(x)P(x,y)$, the [conductance of a Markov chain](../../../markov-process.md#conductance-of-a-markov-chain) is $\Phi(A)=Q(A,A^c)/\pi(A)$. The bottleneck ratio and isoperimetric profile are

$$
\boxed{\Phi_*=\inf_{0<\pi(A)\leq1/2}\Phi(A),
\qquad
\Phi_*(r)=\inf_{0<\pi(A)\leq r}\Phi(A),
\quad0<r\leq\frac12.}
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

No transition joins distinct $A_i$, so

$$
Q(A,A^c)=\sum_iQ(A_i,A_i^c).
$$

Consequently

$$
\boxed{\Phi(A)=\sum_i\frac{\pi(A_i)}{\pi(A)}\Phi(A_i)
\geq\inf_i\Phi(A_i).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The graph has $\asymp n^4$ vertices, bounded degrees, and stationary masses $\asymp n^{-4}$. Split any set into components that do not communicate in one step and use part (a)(ii). A connected component of stationary mass $r\leq1/2$ has $O(rn^4)$ vertices. The planar grid isoperimetric bound supplies at least $c\sqrt{rn^4}$ boundary edges unless the component fills most of one layer; in that case the $\asymp n^2$ interlayer edges give the same order. Thus

$$
\Phi_*(r)\gtrsim\frac1{n^2\sqrt r}.
$$

The conductance-profile mixing bound for a lazy chain now gives

$$
t_{\mathrm{mix}}
\lesssim\int_{4\pi_{\min}}^{1/2}
\frac{du}{u\Phi_*(u)^2}+t_{\mathrm{rel}}
\lesssim n^4.
$$

Here $\Phi_*\gtrsim n^{-2}$ also gives $t_{\mathrm{rel}}\lesssim n^4$ by [Cheeger inequality](../../../markov-process.md#cheeger-inequality). Hence $t_{\mathrm{mix}}\lesssim n^4$.

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose a shortest path $x=x_0,\ldots,x_m=y$. Glue the prescribed one-step edge couplings successively. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the Wasserstein transportation metric gives

$$
\rho_K(P(x,\cdot),P(y,\cdot))
\leq\sum_{j=1}^me^{-\alpha}\rho(x_{j-1},x_j)
=e^{-\alpha}\rho(x,y).
$$

Now couple initial states $(U,V)$ optimally for $\mu,\nu$ and conditionally use these one-step couplings. Taking expectations and then the infimum gives

$$
\rho_K(\mu P,\nu P)\leq e^{-\alpha}\rho_K(\mu,\nu).
$$

Iteration with $\nu=\pi$ yields $\rho_K(P^t(x,\cdot),\pi)\leq e^{-\alpha t}\operatorname{diam}(V)$. Since this metric dominates total variation, it is at most $\varepsilon$ once

$$
\boxed{t\geq\frac1\alpha\left(\log\operatorname{diam}(V)+\log(1/\varepsilon)\right).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Writing $a=|A\setminus B|$ and $b=|B\setminus A|$ gives

$$
\rho(A,B)=\frac{a+b+|a-b|}{2}=\max(a,b).
$$

Make two states adjacent when one can pair every disagreement except at most one, equivalently when $\rho=1$, and give every such edge length one. Pairing a deletion with an insertion as a swap and then handling the excess disagreements constructs a path of length $\max(a,b)$; every edge changes $\rho$ by at most one, so this is the corresponding path metric.

For adjacent states, couple the lazy coin and coordinate choices so that a distinguished disagreement is removed whenever its coordinate is selected, matching a compensating coordinate in the swap case. A direct check of the nested and equal-cardinality cases gives

$$
\mathbb E_{A,B}\rho(X_1,Y_1)
\leq\left(1-\frac1{2n}\right)\rho(A,B).
$$

The [Path coupling theorem](../../../markov-process.md#path-coupling-theorem) extends this to all pairs. Since $\operatorname{diam}(V)=k$, part (a), with $\alpha\geq1/(2n)$ up to an absolute constant, gives

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)\lesssim
n\bigl(\log k+\log(1/\varepsilon)\bigr)
\lesssim n\log(k/\varepsilon).}
$$

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $0<\alpha,\varepsilon<1$, define

$$
\operatorname{hit}_\alpha(\varepsilon)
=\inf\left\{t:\max_x\max_{A:\pi(A)\geq\alpha}
\mathbb P_x(T_A>t)\leq\varepsilon\right\}.
$$

A hit$_\alpha$ cutoff means that for every fixed $0<\varepsilon<1/2$,

$$
\frac{\operatorname{hit}_\alpha(\varepsilon)}
{\operatorname{hit}_\alpha(1-\varepsilon)}\to1.
$$

For finite reversible chains, mixing-time cutoff implies hit$_{1/2}$ cutoff; this is the hitting-time characterization of cutoff.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Both chains are reversible. Since $G$ is $d$-regular, simple random walk $X$ is reversible with uniform invariant distribution. In the weighted graph every vertex has total incident weight $d+\theta$, so $Y$ is also reversible with the same uniform invariant distribution.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Write

$$
\widetilde P=(1-q)P+qM,
\qquad q=\frac\theta{d+\theta}\asymp\frac1{t_{\mathrm{mix}}},
$$

where $M$ traverses the added perfect matching. The standard rare-transition robustness theorem for reversible chains says that when $t_{\mathrm{rel}}=o(t_{\mathrm{mix}})$, adding a bounded-degree kernel at rate $q\asymp1/t_{\mathrm{mix}}$ cannot create cutoff: if the original chain's mixing window is a nonvanishing fraction of its mixing time, the perturbed chain retains such a window. The proof couples the chains between matching jumps; the geometric waiting time for those jumps has mean $\asymp t_{\mathrm{mix}}$ and nonconcentrated fluctuations, while the $X$ segments retain the original noncutoff profile. Therefore cutoff of $Y$ would imply cutoff of $X$, contrary to hypothesis. Hence $Y$ does not exhibit cutoff.

## 5

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

[Thomson principle](../../../markov-process.md#thomson-principle) states that the effective resistance is the minimum energy of a unit flow from $a$ to $z$:

$$
R_{\mathrm{eff}}(a,z)=\inf_\theta
\sum_e\frac{\theta(e)^2}{c(e)}.
$$

An edge cutset separating $a$ and $z$ is a set of edges whose removal disconnects them. Every unit flow has net flux one across each such cutset $\Pi_k$. By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
1=\left(\sum_{e\in\Pi_k}\theta(e)\right)^2
\leq\left(\sum_{e\in\Pi_k}\frac{\theta(e)^2}{c(e)}\right)
\left(\sum_{e\in\Pi_k}c(e)\right).
$$

For disjoint cutsets, summing these energy lower bounds and applying Thomson's principle gives the [Nash-Williams inequality](../../../markov-process.md#nash-williams-inequality)

$$
R_{\mathrm{eff}}(a,z)
\geq\sum_{k=1}^m\left(\sum_{e\in\Pi_k}c(e)\right)^{-1}.
$$

The [commute time identity](../../../markov-process.md#commute-time-identity) is

$$
\boxed{\mathbb E_aT_z+\mathbb E_zT_a
=2\left(\sum_{e\in E}c(e)\right)R_{\mathrm{eff}}(a,z).}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

There are $\asymp n^3$ edges. The $n^2$ horizontal cutsets between successive rows perpendicular to the long direction are disjoint and each contains $\asymp n$ unit-conductance edges. [Nash-Williams inequality](../../../markov-process.md#nash-williams-inequality) gives

$$
R_{\mathrm{eff}}((0,0),(n,n^2))\gtrsim n^2/n=n.
$$

Conversely, spread a unit flow nearly uniformly across the width $n$ while moving it through the $n^2$ long-direction layers, with bounded extra energy to fan out from and collect at the two corner vertices. Its energy is $O(n^2/n)+O(\log n)=O(n)$, so Thomson's principle gives the matching upper bound $R_{\mathrm{eff}}\asymp n$.

The graph is invariant under a half-turn exchanging the two corners, so the two directional hitting-time expectations are equal. The [commute time identity](../../../markov-process.md#commute-time-identity) therefore yields

$$
\boxed{\mathbb E_{(0,0)}T_{(n,n^2)}
\asymp |E|R_{\mathrm{eff}}\asymp n^3n=n^4.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
