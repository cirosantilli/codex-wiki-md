# Paper 204

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_204.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_204.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
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

## 1

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In [bond percolation](../../../bond-percolation.md) on an [undirected graph](../../../graph-theory.md#undirected-graph) $G=(V,E)$, a configuration is $\omega\in\{0,1\}^E$. The [edge](../../../graph-theory.md#edge-of-a-graph) $e$ is open when $\omega_e=1$ and closed when $\omega_e=0$. Under $\mathbb P_p$, the coordinates are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with the [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) of parameter $p$. For a countable [edge](../../../graph-theory.md#edge-of-a-graph) set, use the [product sigma-algebra](../../../probability-theory.md#product-sigma-algebra) and the [product measure](../../../probability-theory.md#product-measure)

$$
\mathbb P_p=\bigotimes_{e\in E}\operatorname{Bernoulli}(p).
$$

The open [edges](../../../graph-theory.md#edge-of-a-graph) form a random subgraph with the original [graph vertices](../../../graph.md#vertex-graph-theory). Its [connected components of a graph](../../../graph.md#component-graph-theory) are the [percolation clusters](../../../bond-percolation.md#percolation-cluster). Write $x\leftrightarrow y$ when an open [graph path](../../../graph-theory.md#path-in-a-graph) joins $x$ to $y$; a zero-length [graph path](../../../graph-theory.md#path-in-a-graph) is allowed, so $x\leftrightarrow x$ always holds. **The randomness is in the independently open bonds; all vertices remain present.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Order configurations coordinatewise: $\omega\leq\omega'$ means $\omega_e\leq\omega'_e$ for every [edge](../../../graph-theory.md#edge-of-a-graph). An [increasing event](../../../probability-inequality.md#increasing-event) $A$ is a measurable [set](../../../set.md) such that $\omega\in A$ and $\omega\leq\omega'$ imply $\omega'\in A$. Opening additional [edges](../../../graph-theory.md#edge-of-a-graph) cannot destroy an [increasing event](../../../probability-inequality.md#increasing-event). The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality), the [product measure](../../../probability-theory.md#product-measure) version of the [FKG inequality](../../../probability-inequality.md#fkg-inequality), states

$$
\boxed{\mathbb P_p(A\cap B)\geq\mathbb P_p(A)\mathbb P_p(B)}
$$

for two [increasing events](../../../probability-inequality.md#increasing-event). Equivalently, bounded coordinatewise increasing [random variables](../../../random-variable.md) $f,g$ satisfy $\mathbb E_p(fg)\geq\mathbb E_p f\,\mathbb E_p g$. The event inequality also holds for two [decreasing events](../../../probability-inequality.md#decreasing-event), by taking complements.

For [disjoint occurrence of increasing events](../../../bond-percolation.md#disjoint-occurrence-of-increasing-events), a finite open [edge](../../../graph-theory.md#edge-of-a-graph) set $K$ witnesses $A$ in $\omega$ if every configuration agreeing with $\omega$ on $K$ belongs to $A$. Since $A$ is an [increasing event](../../../probability-inequality.md#increasing-event) and all [edges](../../../graph-theory.md#edge-of-a-graph) of $K$ are open, this says that the configuration with exactly $K$ open already forces $A$. Define $A\mathbin\square B$ to consist of configurations admitting disjoint finite witnesses $K,L$ for $A,B$. For events depending on finitely many [edges](../../../graph-theory.md#edge-of-a-graph), this is the usual disjoint-occurrence definition; it also applies to finite-connection events on the infinite [graph](../../../graph.md). The [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) states

$$
\boxed{\mathbb P_p(A\mathbin\square B)\leq\mathbb P_p(A)\mathbb P_p(B)}.
$$

On a countable [graph](../../../graph.md), its finite-witness version follows by taking increasing unions over finite [edge](../../../graph-theory.md#edge-of-a-graph) sets. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) concerns simultaneous occurrence, whereas the [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) requires separate certificates using disjoint coordinates.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use integer [graph vertices](../../../graph.md#vertex-graph-theory) in the boxes: $\Lambda_n=[-n,n]^2\cap\mathbb Z^2$, and set $\Lambda_{-1}=\varnothing$. Thus $\partial\Lambda_0=\{0\}$, $g_0=1$, and $|\partial\Lambda_m|=8m$ for $m\geq1$.

If $0\leftrightarrow\partial\Lambda_{m+n}$, erase loops from an open [graph path](../../../graph-theory.md#path-in-a-graph) to obtain a [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk). Let $x$ be its first [graph vertex](../../../graph.md#vertex-graph-theory) on $\partial\Lambda_m$. Split at $x$. The prefix certifies $A_x=\{0\leftrightarrow x\}$, while a segment of the suffix certifies $B_x=\{x\leftrightarrow x+\partial\Lambda_n\}$: the final [graph vertex](../../../graph.md#vertex-graph-theory) is at [supremum norm](../../../functional-analysis.md#supremum-norm) distance at least $n$ from $x$, so the suffix first hits that translated boundary. The two certificates use disjoint [edges](../../../graph-theory.md#edge-of-a-graph). Therefore the [BK boundary-splitting estimate](../../../bond-percolation.md#bk-boundary-splitting-estimate), the [union bound](../../../probability-inequality.md#boole-s-inequality), the [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality), and translation invariance give

$$
\begin{aligned}
g_{m+n}&\leq\sum_{x\in\partial\Lambda_m}\mathbb P_p(A_x\mathbin\square B_x)\\
&\leq\sum_{x\in\partial\Lambda_m}\mathbb P_p(A_x)\mathbb P_p(B_x)\\
&\leq|\partial\Lambda_m|g_mg_n.
\end{aligned}
$$

The cases $m=0$ or $n=0$ follow directly from $g_0=1$, so this proves the bound including the endpoints.

Here is an explicit way to remove the polynomial boundary factor. For $p>0$ put $b_n=32n^2g_n$, $n\geq1$. By symmetry in $m,n$, assume $m\leq n$. Then

$$
\frac{b_{m+n}}{b_mb_n}\leq\frac{(m+n)^2}{4mn^2}\leq\frac1m\leq1.
$$

Consequently $a_n=\log b_n$ is a [subadditive sequence](../../../real-analysis.md#subadditive-sequence). The [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) states that any real [subadditive sequence](../../../real-analysis.md#subadditive-sequence) satisfies $\lim a_n/n=\inf_{n\geq1}a_n/n$, possibly $-\infty$. In this case the direct horizontal open [graph path](../../../graph-theory.md#path-in-a-graph) gives $g_n\geq p^n$, so this [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) is bounded below by $\log p$. Since $g_n\leq1$, its upper bound is zero. Finally,

$$
\frac{\log g_n}{n}=\frac{a_n}{n}-\frac{\log(32n^2)}n
$$

has the same [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence). Thus the [percolation one-arm decay rate](../../../bond-percolation.md#percolation-one-arm-decay-rate) exists and

$$
\boxed{\gamma=\lim_{n\to\infty}g_n^{1/n}\in[p,1]}.
$$

For $p=0$, every $g_n$ with $n\geq1$ is zero and $\gamma=0$. No exponential-decay theorem or assumption that $p$ is below the [percolation critical probability](../../../probability-theory.md#percolation-critical-probability) is needed.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [union bound](../../../probability-inequality.md#boole-s-inequality) gives $g_k\leq\sum_{x\in\partial\Lambda_k}\mathbb P_p(0\leftrightarrow x)$. Hence some boundary [graph vertex](../../../graph.md#vertex-graph-theory) has [percolation two-point connection probability](../../../bond-percolation.md#percolation-two-point-connection-probability) at least $g_k/(8k)$. The rotations and reflections of the [square lattice](../../../graph.md#square-lattice) let us choose such a [graph vertex](../../../graph.md#vertex-graph-theory) as $x=(k,j)$, $-k\leq j\leq k$. Reflection in the vertical line through $x$ sends $0$ to $e_{2k}=(2k,0)$ and fixes $x$. Therefore

$$
\mathbb P_p(x\leftrightarrow e_{2k})=\mathbb P_p(0\leftrightarrow x).
$$

The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) applied to these two [increasing events](../../../probability-inequality.md#increasing-event) proves the [reflection lower bound for two-point percolation](../../../bond-percolation.md#reflection-lower-bound-for-two-point-percolation):

$$
h_{2k}\geq\mathbb P_p(0\leftrightarrow x,\ x\leftrightarrow e_{2k})\geq\left(\frac{g_k}{8k}\right)^2.
$$

Every [graph path](../../../graph-theory.md#path-in-a-graph) from $0$ to $e_{2k}$ reaches $\partial\Lambda_{2k}$, so $h_{2k}\leq g_{2k}$. Taking roots gives

$$
\left(\frac{g_k}{8k}\right)^{1/k}\leq h_{2k}^{1/(2k)}\leq g_{2k}^{1/(2k)}.
$$

Both outside expressions have [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) $\gamma$, proving the even case. For $p>0$, the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) with the last horizontal [edge](../../../graph-theory.md#edge-of-a-graph) gives $h_{2k+1}\geq p h_{2k}$, and also $h_{2k+1}\leq g_{2k+1}$. The lower bound has root

$$
(p h_{2k})^{1/(2k+1)}=p^{1/(2k+1)}\left(h_{2k}^{1/(2k)}\right)^{2k/(2k+1)}\longrightarrow\gamma.
$$

The upper bound has the same [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence). At $p=0$ all positive-distance connection [probabilities](../../../probability-theory.md#probability) vanish. **Thus $\lim_{n\to\infty}h_n^{1/n}=\gamma$ for every $p\in[0,1]$.**

## 2

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An $n$-step [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) on a [graph](../../../graph.md) $G=(V,E)$ is a sequence $(v_0,v_1,\ldots,v_n)$ of $n+1$ distinct [graph vertices](../../../graph.md#vertex-graph-theory) such that $\{v_{i-1},v_i\}\in E$ for $1\leq i\leq n$. **It has $n$ edges and no repeated vertex**, including its starting [graph vertex](../../../graph.md#vertex-graph-theory). The $0$-step [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) consists of its starting [graph vertex](../../../graph.md#vertex-graph-theory) alone.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Represent the [doubly infinite ladder graph](../../../graph.md#doubly-infinite-ladder-graph) by $\mathbb Z\times\{0,1\}$, with horizontal [edges](../../../graph-theory.md#edge-of-a-graph) between successive columns and a vertical rung at each column. An allowed [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) is coded by a word in $R,V$. Two successive $V$ steps revisit the preceding [graph vertex](../../../graph.md#vertex-graph-theory) and are forbidden. Conversely, every word without consecutive $V$ steps is a [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk): horizontal steps strictly increase the column, and a column is visited vertically at most once. This establishes a [bijection](../../../function.md#bijection), not merely an upper bound.

For the [directed ladder self-avoiding walk count](../../../combinatorics.md#directed-ladder-self-avoiding-walk-count), $\sigma_0=1$, $\sigma_1=2$, and for $n\geq2$ a word either ends in $R$, or ends in $RV$. Removing that final block gives

$$
\sigma_n=\sigma_{n-1}+\sigma_{n-2},\qquad\boxed{\sigma_n=F_{n+2}}.
$$

Let $\varphi=(1+\sqrt5)/2$ be the [golden ratio](../../../algebra.md#golden-ratio), and $\psi=(1-\sqrt5)/2$. The [Binet formula](../../../real-analysis.md#binet-formula) for the [Fibonacci number](../../../real-analysis.md#fibonacci-number) yields

$$
\sigma_n=\frac{\varphi^{n+2}-\psi^{n+2}}{\sqrt5}
=\frac{\varphi^{n+2}}{\sqrt5}\left(1-\left(\frac\psi\varphi\right)^{n+2}\right).
$$

Since $|\psi|<\varphi$, taking $n$th roots gives **$\lim_{n\to\infty}\sigma_n^{1/n}=\varphi$**. This use of the golden-ratio symbol is independent of the connection rate in Question 1.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $c_n$ count $n$-step [self-avoiding walks](../../../combinatorics.md#self-avoiding-walk) on the [square lattice](../../../graph.md#square-lattice) from one fixed [graph vertex](../../../graph.md#vertex-graph-theory). Splitting a [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) after $m$ steps and dropping the avoidance constraint on its suffix gives $c_{m+n}\leq c_mc_n$. The [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) therefore gives the [connective constant](../../../combinatorics.md#connective-constant) $\mu=\lim c_n^{1/n}$. The [planar dual graph](../../../graph-theory.md#planar-dual-graph) of the [square lattice](../../../graph.md#square-lattice) is a translated copy of it, so its [connective constant](../../../combinatorics.md#connective-constant) is also $\mu$.

Put $q=1-p$ and assume $q\mu<1$. Choose $a>\mu$ with $qa<1$. The definition of the [connective constant](../../../combinatorics.md#connective-constant) provides a finite $K$ such that $c_j\leq Ka^j$ for every $j\geq0$. A simple dual [graph cycle](../../../graph-theory.md#cycle-in-a-graph) of length $\ell$ surrounding $0$ has a [graph vertex](../../../graph.md#vertex-graph-theory) in a box of radius $\ell+1$: its diameter is at most $\ell$, and its coordinate ranges straddle the origin. Choose such a [graph vertex](../../../graph.md#vertex-graph-theory) as the starting point, orient the [graph cycle](../../../graph-theory.md#cycle-in-a-graph), and omit its closing [edge](../../../graph-theory.md#edge-of-a-graph). The remaining [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) has length $\ell-1$. Consequently the number $N_\ell$ of these [graph cycles](../../../graph-theory.md#cycle-in-a-graph) obeys

$$
N_\ell\leq K_0\ell^2 c_{\ell-1}\leq K_1\ell^2a^{\ell-1}
$$

for fixed finite constants. A specified [graph cycle](../../../graph-theory.md#cycle-in-a-graph) is open in [dual bond percolation](../../../graph-theory.md#dual-bond-percolation), equivalently all its crossed primal [edges](../../../graph-theory.md#edge-of-a-graph) are closed, with [probability](../../../probability-theory.md#probability) $q^\ell$. Hence

$$
\sum_{\ell\geq L}N_\ell q^\ell\longrightarrow0\quad\text{as }L\to\infty.
$$

To make this tail argument valid for every $q\mu<1$, rather than only extremely small $q$, use a [finite modification of Bernoulli percolation](../../../probability-theory.md#finite-modification-of-bernoulli-percolation). Condition all primal [edges](../../../graph-theory.md#edge-of-a-graph) within $\Lambda_N$ to be open. This event has positive [probability](../../../probability-theory.md#probability) for $p>0$. If the resulting [percolation cluster](../../../bond-percolation.md#percolation-cluster) of $0$ is finite, its outer boundary contains a simple closed dual [graph cycle](../../../graph-theory.md#cycle-in-a-graph) surrounding the whole box. Such a [graph cycle](../../../graph-theory.md#cycle-in-a-graph) has length tending to infinity with $N$ and crosses no forced-open [edge](../../../graph-theory.md#edge-of-a-graph). Under the conditioning its remaining [edge](../../../graph-theory.md#edge-of-a-graph) states retain the original independent law, so its [probability](../../../probability-theory.md#probability) is still $q^\ell$. Choose $N$ so that the above tail is less than $1/2$. The conditional [probability](../../../probability-theory.md#probability) that $0$ belongs to an [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) is then at least $1/2$, and thus $\theta(p)>0$.

This [connective-constant Peierls bound](../../../probability-theory.md#connective-constant-peierls-bound) proves that every $p>1-\mu^{-1}$ is above or at the onset of positive [percolation probability](../../../probability-theory.md#percolation-probability). Taking the infimum gives

$$
\boxed{p_c\leq1-\mu^{-1}}.
$$

The case $p=1$ is immediate. This proof uses the [Peierls argument](../../../probability-theory.md#peierls-argument), without assuming the exact [Harris-Kesten theorem](../../../probability-theory.md#harris-kesten-theorem).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $\mathcal W_n$ for the deterministic [set](../../../set.md) of $n$-step [self-avoiding walks](../../../combinatorics.md#self-avoiding-walk) from $0$. Each uses $n$ distinct [edges](../../../graph-theory.md#edge-of-a-graph), so [independence](../../../random-variable.md#independent-random-variables) gives

$$
\kappa_n=\sum_{w\in\mathcal W_n}\mathbf1_{\{w\text{ open}\}},\qquad\mathbb E_p\kappa_n=c_np^n.
$$

For $n\geq1$, the function $t\mapsto t^{1/n}$ on $[0,\infty)$ is a [concave function](../../../real-analysis.md#concave-function). The [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives the [root-moment bound for open self-avoiding walks](../../../combinatorics.md#root-moment-bound-for-open-self-avoiding-walks)

$$
\mathbb E_p(\kappa_n^{1/n})\leq(\mathbb E_p\kappa_n)^{1/n}=p c_n^{1/n}.
$$

Equivalently, the [Lyapunov moment inequality](../../../probability-inequality.md#lyapunov-moment-inequality) compares exponents $1/n$ and $1$, both strictly positive. Taking the [limit superior](../../../real-analysis.md#limit-superior) and the [connective constant](../../../combinatorics.md#connective-constant) limit proves

$$
\boxed{\limsup_{n\to\infty}\mathbb E_p(\kappa_n^{1/n})\leq p\mu}.
$$

This includes $p=0$ and $n=1$. No [independence](../../../random-variable.md#independent-random-variables) between the different [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) indicators is asserted or needed.

## 3

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [cubic lattice](../../../graph.md#cubic-lattice) has [graph vertices](../../../graph.md#vertex-graph-theory) $\mathbb Z^d$ and an [edge](../../../graph-theory.md#edge-of-a-graph) between $x,y$ when $\sum_i|x_i-y_i|=1$. In independent [site percolation](../../../site-percolation.md), every [graph vertex](../../../graph.md#vertex-graph-theory) is open with [probability](../../../probability-theory.md#probability) $p$ and closed with [probability](../../../probability-theory.md#probability) $1-p$, independently. The open subgraph contains only open [graph vertices](../../../graph.md#vertex-graph-theory) and the [edges](../../../graph-theory.md#edge-of-a-graph) between them. Let $C_p(0)$ be the open [connected component of a graph](../../../graph.md#component-graph-theory) containing $0$, with $C_p(0)=\varnothing$ when $0$ is closed. The [percolation probability](../../../probability-theory.md#percolation-probability) is

$$
\boxed{\theta(p)=\mathbb P_p(|C_p(0)|=\infty)=\mathbb P_p(0\leftrightarrow\infty)}.
$$

Since the [cubic lattice](../../../graph.md#cubic-lattice) is a [locally finite graph](../../../graph-theory.md#locally-finite-graph), the [König infinity lemma](../../../combinatorics.md#konig-s-lemma) identifies an infinite open [connected component of a graph](../../../graph.md#component-graph-theory) with the existence of an infinite open [graph ray](../../../graph-theory.md#ray-in-a-graph) from the origin. In particular, the origin itself must be open. The [percolation critical probability](../../../probability-theory.md#percolation-critical-probability) is $p_c=\inf\{p:\theta(p)>0\}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $A_n$ be the event that the origin has an open [graph path](../../../graph-theory.md#path-in-a-graph) to the boundary of $[-n,n]^d\cap\mathbb Z^d$. The [graph path](../../../graph-theory.md#path-in-a-graph) can be stopped on its first boundary visit, so $A_n$ depends on only finitely many sites. Its [probability](../../../probability-theory.md#probability) $f_n(p)=\mathbb P_p(A_n)$ is a finite sum of terms $p^a(1-p)^b$, and is therefore a [continuous function](../../../calculus.md#continuous-function) of $p$. Also $A_{n+1}\subseteq A_n$, and the [König infinity lemma](../../../combinatorics.md#konig-s-lemma) gives $\bigcap_n A_n=\{0\leftrightarrow\infty\}$. By [continuity from above of a measure](../../../measure-theory.md#continuity-from-above-of-a-measure),

$$
\theta(p)=\inf_{n\geq1}f_n(p).
$$

The [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation) described below shows that $\theta$ is nondecreasing. For $p<1$, its right [limit of a function](../../../calculus.md#limit-of-a-function) $\theta(p+)$ exists and is at least $\theta(p)$. For every fixed $n$,

$$
\theta(p+)\leq\lim_{r\downarrow p}f_n(r)=f_n(p).
$$

Taking the infimum in $n$ proves **$\theta(p+)=\theta(p)$**. This proves [right continuity of percolation probability](../../../probability-theory.md#right-continuity-of-percolation-probability) throughout $[0,1)$; at $1$ right continuity is understood relative to the parameter domain. The argument does not interchange two uncontrolled limits.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [probability space](../../../probability-theory.md#probability-space) $([0,1]^{\mathbb Z^d},\mathcal F,\mathbb P)$ with the [product measure](../../../probability-theory.md#product-measure) of the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$. Its coordinate [random variables](../../../random-variable.md) $U_v$ are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables). Define simultaneously for every parameter

$$
\boxed{X_p(v)=\mathbf1_{\{U_v\leq p\}},\qquad p\in[0,1],\ v\in\mathbb Z^d}.
$$

For $r\leq s$, the [indicator function](../../../measure-theory.md#indicator-function) inequality $X_r(v)\leq X_s(v)$ holds pointwise at every [graph vertex](../../../graph.md#vertex-graph-theory). For fixed $p$, each coordinate has the [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with parameter $p$, and the coordinates are independent because they are functions of distinct independent $U_v$. Thus every marginal configuration is exactly the required [site percolation](../../../site-percolation.md) model. This is a continuum-indexed family of processes, all on one [probability space](../../../probability-theory.md#probability-space), and is the standard [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Work on the common [probability space](../../../probability-theory.md#probability-space) from part (c). For a configuration of all the uniforms, the [set](../../../set.md) $S=\{r\in[0,1]:I_r\text{ occurs}\}$ is an upper interval, possibly with or without its lower endpoint. It is nonempty because $I_1$ occurs, and the [coupled onset parameter for origin percolation](../../../probability-theory.md#coupled-onset-parameter-for-origin-percolation) is $M=\inf S$. For $0<p\leq1$,

$$
\bigcup_{\substack{r<p\\r\in\mathbb Q\cap[0,1]}} I_r=\{M<p\}.
$$

Indeed, occurrence at some $r<p$ implies $M<p$. Conversely, if $M<p$, the definition of infimum yields occurrence at some $s<p$, and a rational $r$ between $s$ and $p$ also satisfies $I_r$. This also proves measurability of $M$ through its strict sublevel [sets](../../../set.md).

Choose a rational sequence increasing to $p$. By [continuity from below of a measure](../../../measure-theory.md#continuity-from-below-of-a-measure) and the [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation),

$$
\lim_{r\uparrow p}\theta(r)=\mathbb P(M<p).
$$

Moreover, $\{M<p\}\subseteq I_p\subseteq\{M\leq p\}$. Hence $I_p$ is the disjoint union of $\{M<p\}$ and $I_p\cap\{M=p\}$, giving

$$
\boxed{\lim_{r\uparrow p}\theta(r)=\theta(p)-\mathbb P(I_p\cap\{M=p\})}.
$$

It is important to retain the intersection with $I_p$: occurrence at the infimum is not automatic. At $p=0$ there is no left limit within the parameter domain, so the displayed left-limit assertion is for $p>0$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Use the following general result, including its site version: independent [site percolation](../../../site-percolation.md) on $\mathbb Z^d$ has [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) at most one [infinite percolation cluster](../../../bond-percolation.md#infinite-percolation-cluster) at each fixed parameter; for every fixed $r>p_c$ it has exactly one [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). This is the [uniqueness of the infinite percolation cluster](../../../bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster), also called the [Burton-Keane theorem](../../../bond-percolation.md#uniqueness-of-the-infinite-percolation-cluster). For $d\geq2$, the additional general fact $p_c<1$ ensures a choice of a parameter strictly between $p_c$ and $1$. In dimension one, $p_c=1$ and the asserted interval is empty.

Fix $p\in(p_c,1]$ and choose $q\in(p_c,p)$. Let $\mathcal C_q$ be the unique infinite open [connected component of a graph](../../../graph.md#component-graph-theory) at $q$. Under the [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation), it is contained in the unique infinite open [connected component of a graph](../../../graph.md#component-graph-theory) at $p$. On $I_p$, the origin and $\mathcal C_q$ therefore lie in that same [connected component of a graph](../../../graph.md#component-graph-theory), and a finite $p$-open [graph path](../../../graph-theory.md#path-in-a-graph) connects $0$ to some [graph vertex](../../../graph.md#vertex-graph-theory) of $\mathcal C_q$.

For this fixed deterministic $p$, the countable [set](../../../set.md) of uniforms satisfies $U_v\ne p$ at every [graph vertex](../../../graph.md#vertex-graph-theory) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Thus all uniforms on that finite [graph path](../../../graph-theory.md#path-in-a-graph) are strictly less than $p$, including its endpoints. If $t$ is their maximum, choose $r$ with $\max(q,t)<r<p$. The [graph path](../../../graph-theory.md#path-in-a-graph) is then $r$-open, and its endpoint remains connected to infinity through $\mathcal C_q$. Consequently $I_r$ occurs and $M<p$. We have proved

$$
\mathbb P(I_p\cap\{M=p\})=0.
$$

Part (d) gives left continuity at this $p$; part (b) supplies right continuity when $p<1$. The same finite-path proof gives left continuity at $p=1$, since all uniforms are strictly less than $1$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). **Thus $\theta$ is continuous on $(p_c,1]$**, without asserting continuity at $p_c$. This is [supercritical continuity of percolation probability](../../../probability-theory.md#supercritical-continuity-of-percolation-probability).

## 4

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $H(R)$ and $V(R)$ for the horizontal and vertical open-crossing [increasing events](../../../probability-inequality.md#increasing-event) of a rectangle in the rotated [square lattice](../../../graph.md#square-lattice). At parameter $1/2$, [planar duality for rectangle crossings](../../../graph-theory.md#planar-duality-for-rectangle-crossings) says that failure of $H$ is exactly a closed dual vertical crossing. Quarter-turn symmetry and the boundary convention of the rotated rectangles identify the two alternatives on a square. Thus its crossing [probability](../../../probability-theory.md#probability) is $1/2$; a rectangle obtained by a harmless one-step boundary adjustment has crossing [probability](../../../probability-theory.md#probability) at least $1/2$. This is the finite-domain [exact self-dual rectangle crossing probability](../../../graph-theory.md#exact-self-dual-rectangle-crossing-probability), not an assumption about infinite [percolation clusters](../../../bond-percolation.md#percolation-cluster).

We first prove a [RSW reflection extension lemma](../../../bond-percolation.md#rsw-reflection-extension-lemma). In coordinate units adapted to the rotated drawing, take $S=[0,n]^2$, $T=[-n,n]^2$, and $R=[-n,2n]\times[-n,n]$. Reveal the rightmost open vertical crossing $\Gamma$ of $S$, when one exists, using only its [edges](../../../graph-theory.md#edge-of-a-graph) and the region to its right. Reflect $\Gamma$ across the horizontal axis. The part $D$ of $T$ to the left of these two paths remains unexposed and has the independent parameter-$1/2$ law. A horizontal crossing of $T$ must reach their union. Its [probability](../../../probability-theory.md#probability) is at least $1/2$. Reflection symmetry and the [union bound](../../../probability-inequality.md#boole-s-inequality) give a [probability](../../../probability-theory.md#probability) at least $1/4$ of reaching the upper path $\Gamma$ through $D$. Conditional opening of the [edges](../../../graph-theory.md#edge-of-a-graph) on $\Gamma$ can only help. Since $V(S)$ has [probability](../../../probability-theory.md#probability) at least $1/2$, the [increasing event](../../../probability-inequality.md#increasing-event) $B$ that a vertical crossing of $S$ is connected inside $T$ to its left side has [probability](../../../probability-theory.md#probability) at least $1/8$.

Reflect this construction in the vertical midline of $S$ to obtain an [increasing event](../../../probability-inequality.md#increasing-event) $B'$ of the same [probability](../../../probability-theory.md#probability), connecting a vertical crossing of $S$ to the right side of $[0,2n]\times[-n,n]$. On $H(S)\cap B\cap B'$, the horizontal crossing of $S$ meets both vertical crossings, so all three [graph paths](../../../graph-theory.md#path-in-a-graph) join and give $H(R)$. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) now yields

$$
\mathbb P_{1/2}(H(R))\geq\frac12\left(\frac18\right)^2=\frac1{128}.
$$

The exploration only conditions the exposed side of the extremal [graph path](../../../graph-theory.md#path-in-a-graph); reflecting a drawn path does not assert that its reflected [edges](../../../graph-theory.md#edge-of-a-graph) are open. This distinction is what makes the extension argument valid.

To pass from aspect ratio $3/2$ to $3$, put four rectangles of width $3h/2$ and height $h$ next to each other, with successive left boundaries separated by $h/2$. Adjacent rectangles overlap in a square of side $h$. Require horizontal crossings of the four rectangles and vertical crossings of the three overlap squares. Every consecutive pair of horizontal crossings meets the vertical crossing in its overlap; together they form a horizontal crossing of width $3h$. The [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) gives a strictly positive bound, for these compatible scales, of

$$
c_*=(1/128)^4(1/2)^3.
$$

The construction works on the rotated [square lattice](../../../graph.md#square-lattice) with the boundary sites used in the source drawing. Integer roundings do not create a scale restriction: for an odd height use the largest smaller compatible even height, and use eight horizontal rectangles and seven overlap squares, whose union has auxiliary aspect ratio $5$, so that its width exceeds the desired $3m$ width for all sufficiently large $m$. Truncate its horizontal crossing on first reaching the desired right side. The number of extra rectangles and overlap-square crossings is bounded independently of $m$, and every factor is bounded below by the same positive constants. The finitely many smallest rectangles each have positive crossing [probability](../../../probability-theory.md#probability), since a specified finite open [graph path](../../../graph-theory.md#path-in-a-graph) suffices. Therefore a constant $c>0$ works at every integer scale. Taking $\tau=c/2$ ensures the requested strict inequality:

$$
\boxed{\inf_{m\geq1}\mathbb P_{1/2}(C_{3m,m})\geq c>\tau>0}.
$$

This proves the required instance of the [Russo-Seymour-Welsh theorem](../../../bond-percolation.md#russo-seymour-welsh-theorem) through reflection, exploration and gluing. The parameter in this calculation is $1/2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

First obtain a [polynomial critical one-arm upper bound](../../../bond-percolation.md#polynomial-critical-one-arm-upper-bound) from part (a). Fix a sufficiently large integer radius $r$. Use rotated-coordinate boxes $B_r=[-r,r]^2$ for this geometric construction, in the axes of part (a). Surround $B_r$ by a square ring inside $B_{3r}$. It can be assembled from the four strips

$$
[-3r,3r]\times[r,3r],\quad[-3r,3r]\times[-3r,-r],\quad[-3r,-r]\times[-3r,3r],\quad[r,3r]\times[-3r,3r].
$$

The first two require horizontal dual crossings; the last two require vertical dual crossings. Their corner overlaps are squares, so the adjacent long crossings intersect there and their union contains a dual [graph cycle](../../../graph-theory.md#cycle-in-a-graph) surrounding the inner box. Translate the strips by the half-lattice displacement of the [planar dual graph](../../../graph-theory.md#planar-dual-graph) and adjust the endpoints by one lattice unit if needed. All aspect ratios remain bounded. Part (a) and the same overlap gluing give a uniform lower bound $c_1>0$ for each dual crossing at $1/2$. Applying the [Harris-FKG inequality](../../../probability-inequality.md#harris-fkg-inequality) to these [decreasing events](../../../probability-inequality.md#decreasing-event) in the primal configuration gives a closed dual circuit with [probability](../../../probability-theory.md#probability) at least $\delta=c_1^4>0$. We may replace $\delta$ by a smaller number in $(0,1)$.

Use the [independent annular barriers for percolation](../../../bond-percolation.md#independent-annular-barriers-for-percolation) at radii $r_j=r_0 10^j$. Their supporting [edge](../../../graph-theory.md#edge-of-a-graph) sets are disjoint, so the circuit events are independent. In the original unrotated coordinates, $B_{3r}$ lies inside $\Lambda_{5r}$ and the ring still separates the origin from infinity. These fixed geometric comparisons let us bound the original $g_N$. An open [graph path](../../../graph-theory.md#path-in-a-graph) from $0$ to distance $N$ must avoid every such closed dual circuit inside $\Lambda_N$. Thus, for some constants $C<\infty$ and $\alpha>0$,

$$
g_N(1/2)\leq(1-\delta)^{\lfloor\log_{10}(N/(5r_0))\rfloor+1}\leq C N^{-\alpha},\qquad
\alpha=\frac{-\log(1-\delta)}{\log10}>0,
$$

where the first bound is used only when at least one of the indicated rings fits; increasing $C$ handles smaller $N$.

Now let $\varepsilon=p-1/2>0$ and use the [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation) on [edges](../../../graph-theory.md#edge-of-a-graph). The event $\{0\leftrightarrow\partial\Lambda_N\}$ only needs [edges](../../../graph-theory.md#edge-of-a-graph) whose endpoints lie in $\Lambda_N$, because a first boundary hit gives an internal [graph path](../../../graph-theory.md#path-in-a-graph). There are exactly $4N(2N+1)$ such [edges](../../../graph-theory.md#edge-of-a-graph). Each changes state between parameters $1/2$ and $p$ with [probability](../../../probability-theory.md#probability) $\varepsilon$. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore gives the [finite-box comparison for percolation parameters](../../../probability-theory.md#finite-box-comparison-for-percolation-parameters)

$$
\theta(p)\leq g_N(p)\leq g_N(1/2)+4N(2N+1)\varepsilon\leq C N^{-\alpha}+12N^2\varepsilon.
$$

For sufficiently small $\varepsilon$, choose $N=\lfloor\varepsilon^{-1/(\alpha+2)}\rfloor$, so that $N$ is at least half the unrounded value. Both terms then have order $\varepsilon^{\alpha/(\alpha+2)}$. In particular,

$$
\boxed{\theta(p)\leq A(p-1/2)^\beta,\qquad\beta=\frac\alpha{\alpha+2}>0}
$$

for a finite $A$. Increase $A$ to cover the remaining compact range of parameters by $\theta(p)\leq1$. This [near-critical percolation power upper bound](../../../probability-theory.md#near-critical-percolation-power-upper-bound) requires only a positive crossing constant, not the exact value of a critical exponent. It also implies $\theta(1/2)=0$ through the critical [one-arm probability](../../../bond-percolation.md#one-arm-probability) bound.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
