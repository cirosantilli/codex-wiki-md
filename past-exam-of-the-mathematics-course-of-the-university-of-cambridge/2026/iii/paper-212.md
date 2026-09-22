# Paper 212

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20212.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20212.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 212](paper-212.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In [bond percolation](../../../bond-percolation.md) on the [square lattice](../../../graph.md#square-lattice), exactly one of the following occurs in the rectangle: an open left-to-right primal crossing, or a closed top-to-bottom crossing in the [planar dual graph](../../../graph-theory.md#planar-dual-graph). These alternatives are disjoint and exhaustive by [planar duality for rectangle crossings](../../../graph-theory.md#planar-duality-for-rectangle-crossings).

At $p=1/2$, the closed dual edges have the same law as open primal edges. Rotating the dual rectangle through a right angle identifies its top-to-bottom crossing with the original left-to-right crossing; the slight difference between the side lengths $\ell+1$ and $\ell$ is exactly the boundary shift introduced by dualization. Thus the event and its complement have equal probability, so

$$
\boxed{\mathbb P_{1/2}(\operatorname{LR}(\ell))=\frac12.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write

$$
\pi(r)=\mathbb P_{1/2}(0\longleftrightarrow\partial\Lambda_r).
$$

The [Russo-Seymour-Welsh theorem](../../../bond-percolation.md#russo-seymour-welsh-theorem) and the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) give the standard [one-arm extension estimate](../../../bond-percolation.md#one-arm-extension-estimate): there is $c>0$ such that

$$
\pi(2r)\geq c\pi(r)
$$

uniformly in $r$. Indeed, on the one-arm event to scale $r$, a fixed finite collection of open rectangle crossings in the annulus $\Lambda_{2r}\setminus\Lambda_r$, each having probability bounded below by RSW, joins that arm to $\partial\Lambda_{2r}$; FKG multiplies the lower bounds. Iteration shows that $\pi(ar)$ and $\pi(r)$ are comparable for every fixed $a>0$. This proves the estimate suggested in the hint.

Fix $x\in\partial\Lambda_n$ and choose $r=\lfloor n/4\rfloor$. If $0\longleftrightarrow x$, there is an open arm from $0$ to distance $r$ and another from $x$ to distance $r$. These are [independent events](../../../probability-theory.md#independent-events) because they use disjoint edge sets, so the extension estimate gives

$$
\mathbb P_{1/2}(0\longleftrightarrow x)
\leq\pi(r)^2\leq C\pi(n)^2.
$$

For the reverse inequality, take one-arm events from $0$ and $x$ at scale comparable with $n$, in disjoint boxes. A fixed collection of open crossings of rectangles of bounded aspect ratio joins the two arms. The [Russo-Seymour-Welsh theorem](../../../bond-percolation.md#russo-seymour-welsh-theorem) bounds the probability of every added crossing below uniformly in $n$ and in the position of $x$ along the four sides; the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) and the arm-extension estimate therefore give

$$
\mathbb P_{1/2}(0\longleftrightarrow x)
\geq c\pi(n)^2.
$$

This is the usual [RSW gluing lemma for two one-arm events](../../../bond-percolation.md#rsw-gluing-lemma-for-two-one-arm-events). Enlarging the constants handles the finitely many small $n$, proving the claim with positive constants $c_1,c_2$.

## 2

↑ **Parent:** [Paper 212](paper-212.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For every truncated directed path $\gamma:o\to z_r$, let $j_\gamma$ be its signed unit [flow](../../../graph-theory.md#flow) along its traversed edges. Its [divergence of a flow](../../../graph-theory.md#divergence-of-a-flow) is zero at every vertex other than $o,z_r$, while its strength from $o$ to $z_r$ is one. The displayed expression in the question is

$$
\theta_\omega
=\sum_{\gamma:o\to z_r}
\frac{\mu(\gamma)\mathbf1_{\{\gamma\text{ open}\}}}
{\mathbb P(\gamma\text{ open})},j_\gamma.
$$

It is a nonnegative linear combination of such path flows. Hence it obeys flow conservation at every interior vertex, is antisymmetric on oppositely directed edges, and is supported on open edges. It is therefore a flow from $o$ to $z_r$ for every configuration $\omega$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The strength of the linear combination is the same linear combination of the unit strengths:

$$
X_r(\omega)=\sum_{\gamma:o\to z_r}
\frac{\mu(\gamma)\mathbf1_{\{\gamma\text{ open}\}}}
{\mathbb P(\gamma\text{ open})}.
$$

Taking expectations cancels each denominator. Since the truncated paths partition the path space,

$$
\mathbb EX_r
=\sum_{\gamma:o\to z_r}\mu(\gamma)=1.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Expanding the square and using the independence of the percolation edges gives

$$
\mathbb EX_r^2
=\sum_{\gamma,\gamma'}\mu(\gamma)\mu(\gamma')
\frac{\mathbb P(\gamma,\gamma'\text{ open})}
{\mathbb P(\gamma\text{ open})\mathbb P(\gamma'\text{ open})}.
$$

The ratio equals $p^{-N_r(\gamma,\gamma')}$, where $N_r$ is the number of common edges in the two truncated paths. It is at most $p^{-N}$ for $N=|\xi\cap\xi'|$, under the convention in the hypothesis; in particular $N\geq1$ because both paths contain $o$. For every integer $N\geq1$,

$$
p^{-N}\leq\sum_{n=1}^Np^{-n}.
$$

The [tail-sum formula](../../../probability-theory.md#tail-sum-formula) and the assumed exponential intersection tail therefore yield

$$
\boxed{\mathbb EX_r^2
\leq\sum_{n=1}^\infty p^{-n}(\mu\times\mu)(N\geq n)
\leq C\sum_{n=1}^\infty\left(\frac\zeta p\right)^n
=\frac{C\zeta}{p-\zeta}.}
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Let the [energy of a flow](../../../graph-theory.md#energy-of-a-flow) be $\mathcal E(\theta)=\sum_e\theta(e)^2$, with each unoriented edge counted once. Expanding as in part (i), dropping orientation signs, and summing over common edges gives

$$
\mathbb E\mathcal E(\theta_\omega)
\leq\mathbb E_{\mu\times\mu}[N p^{-N}]
\leq C\sum_{n\geq1}n\left(\frac\zeta p\right)^n<\infty,
$$

uniformly in $r$.

Part (i), $\mathbb EX_r=1$, and the [Paley-Zygmund inequality](../../../probability-and-statistics.md#paley-zygmund-inequality) give a constant $a>0$ such that $\mathbb P(X_r>1/2)\geq a$ for every $r$. The preceding uniform expectation bound and [Markov inequality](../../../probability-inequality.md#markov-inequality) allow a constant $L$ such that

$$
\mathbb P\bigl(X_r>1/2, \mathcal E(\theta_\omega)\leq L\bigr)\geq a/2.
$$

On this event, $\theta_\omega/X_r$ is a unit open flow from $o$ to $z_r$ with energy at most $4L$.

The events that there is such a bounded-energy unit flow from $o$ out of $B(o,r)$ are decreasing in $r$. Their intersection still has probability at least $a/2$. A diagonal compactness argument produces on this intersection a unit flow from $o$ to infinity, supported on its open cluster, with finite energy. The [finite-energy flow criterion for transience](../../../graph-theory.md#finite-energy-flow-criterion-for-transience) makes that open cluster transient.

Thus a transient open cluster exists with positive probability. This existence event is a [tail event](../../../probability-theory.md#tail-event): changing finitely many edges cannot destroy transience in every infinite component, because transience is invariant under finite graph modifications. The [Kolmogorov zero-one law](../../../probability-theory.md#kolmogorov-s-zero-one-law) upgrades its probability to one.

## 3

↑ **Parent:** [Paper 212](paper-212.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Take an increasing exhaustion $G_n$ of $G$ by finite connected vertex sets, identify every vertex outside $G_n$ to one boundary vertex, and choose a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) of the resulting finite wired graph. The weak limit as $n\to\infty$ is the [wired uniform spanning forest](../../../combinatorics.md#wired-uniform-spanning-forest) of $G$.

For [Wilson algorithm rooted at infinity](../../../combinatorics.md#wilson-algorithm-rooted-at-infinity), enumerate $V$ as $v_1,v_2,\ldots$. Run a [simple random walk](../../../markov-process.md#simple-random-walk) from $v_1$ forever and add its chronological [loop erasure](../../../markov-process.md#loop-erasure). Transience makes the infinite loop erasure well-defined. Next, from the first vertex not already in the forest, run an independent random walk until it hits the existing forest; if it never hits, run it forever. Add its loop erasure and continue through the enumeration. Wilson's theorem rooted at infinity says that the resulting forest has the wired uniform spanning forest law.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Run [Wilson algorithm rooted at infinity](../../../combinatorics.md#wilson-algorithm-rooted-at-infinity) with $w_1,\ldots,w_K$ first in the enumeration. Couple its first $K$ walks with the independent walks in the hypothesis. On the positive-probability event that their ranges are pairwise disjoint, no walk from $w_j$ hits any earlier loop-erased range. Wilson's algorithm therefore creates $K$ distinct trees, so

$$
\mathbb P(\text{the wired uniform spanning forest has at least $K$ trees})>0.
$$

The [component-number zero-one law for the wired uniform spanning forest](../../../combinatorics.md#component-number-zero-one-law-for-the-wired-uniform-spanning-forest) says that its number of trees is almost surely constant; it follows from tail triviality of the wired uniform spanning forest and the fact that all its trees are infinite. The displayed positive probability must consequently equal one.

## 4

↑ **Parent:** [Paper 212](paper-212.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $\tau_p(x)=\mathbb P_p(0\longleftrightarrow x)$ and $r=1-\chi(p)^{-1}$. The [percolation susceptibility](../../../bond-percolation.md#percolation-susceptibility) decomposes over the $\ell^1$ spheres as

$$
\chi(p)=\mathbb E_p|C|
=\sum_{n=0}^\infty\mathbb E_pM_n,
\qquad \mathbb E_pM_0=1.
$$

If $\mathbb E_pM_n>r^n$ for every $n\geq1$, then

$$
\chi(p)>1+\sum_{n=1}^\infty r^n
=1+\frac r{1-r}=\chi(p),
$$

a contradiction. Hence some $m\geq1$ satisfies $\mathbb E_pM_m\leq r^m$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set $a=\mathbb E_pM_m=\sum_{|x|=m}\tau_p(x)$. If $|u|\geq m$, an open self-avoiding path from $0$ to $u$ first meets the $\ell^1$ sphere of radius $m$ at some $x$. Its portions from $0$ to $x$ and from $x$ to $u$ use disjoint edge sets. The [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) and translation invariance therefore give

$$
\tau_p(u)
\leq\sum_{|x|=m}\tau_p(x)\tau_p(u-x).
$$

Let $s_k=\sup_{|u|\geq km}\tau_p(u)$. Since $|u-x|\geq|u|-m$, the last inequality gives $s_k\leq a s_{k-1}$ and $s_0\leq1$. Induction yields

$$
\boxed{\mathbb P_p(0\longleftrightarrow u)=\tau_p(u)
\leq a^{\lfloor|u|/m\rfloor}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $j=0,\ldots,k-1$, let $E_j$ be the increasing event that $ju\longleftrightarrow(j+1)u$. Their intersection implies $0\longleftrightarrow ku$. By translation invariance and the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality),

$$
\boxed{\mathbb P_p(0\longleftrightarrow ku)
\geq\mathbb P_p\left(\bigcap_{j=0}^{k-1}E_j\right)
\geq\prod_{j=0}^{k-1}\mathbb P_p(E_j)
=\mathbb P_p(0\longleftrightarrow u)^k.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Combine parts (a)--(c). For every $k\geq1$,

$$
\tau_p(u)^k
\leq\tau_p(ku)
\leq(\mathbb E_pM_m)^{\lfloor k|u|/m\rfloor}
\leq r^{m\lfloor k|u|/m\rfloor}.
$$

Taking $k$th roots and letting $k\to\infty$ gives

$$
\boxed{\mathbb P_p(0\longleftrightarrow u)=\tau_p(u)
\leq r^{|u|}
=\left(1-\chi(p)^{-1}\right)^{|u|}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
