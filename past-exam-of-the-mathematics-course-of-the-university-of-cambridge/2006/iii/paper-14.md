# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper14.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Expose the vertices in order, revealing at step $i$ every [edge](../../../graph-theory.md#edge-of-a-graph) from vertex $i$ to an earlier vertex. With the resulting [filtration](../../../stochastic-process.md#filtration-probability-theory) $\mathcal F_i$, put

$$
M_i=\mathbb E[\chi(G)\mid\mathcal F_i],\qquad M_0=\mu,\quad M_n=\chi(G).
$$

This is the [vertex exposure for chromatic number](../../../graph-theory.md#vertex-exposure-for-chromatic-number) [martingale](../../../martingale.md). Its increments $D_i=M_i-M_{i-1}$ have [conditional mean](../../../measure-theory.md#conditional-expectation) zero and satisfy $|D_i|\leq1$, by the permitted [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity).

Here is the required exponential-moment proof of the [Azuma-Hoeffding inequality](../../../martingale.md#azuma-s-inequality). More generally, suppose $|D_i|\leq c_i$ for deterministic $c_i$. [Convexity](../../../real-analysis.md#convex-function) of the [exponential function](../../../calculus.md#exponential-function) gives, for $-c_i\leq d\leq c_i$,

$$
e^{td}\leq\frac{c_i+d}{2c_i}e^{tc_i}+\frac{c_i-d}{2c_i}e^{-tc_i}.
$$

Taking [conditional expectation](../../../measure-theory.md#conditional-expectation) and using the zero [conditional mean](../../../measure-theory.md#conditional-expectation) yields

$$
\mathbb E[e^{tD_i}\mid\mathcal F_{i-1}]\leq\cosh(tc_i)\leq e^{t^2c_i^2/2}.
$$

For the last inequality, integrate $(\log\cosh u)'=\tanh u\leq u$ for $u\geq0$, and use evenness. A zero $c_i$ simply means a zero increment. Iterated [conditional expectation](../../../measure-theory.md#conditional-expectation) now gives

$$
\mathbb E e^{t(M_n-M_0)}\leq\exp\left(\frac{t^2}{2}\sum_i c_i^2\right).
$$

For $s,t>0$, the strict Markov bound on the event $M_n-M_0>s$ gives

$$
\mathbb P(M_n-M_0>s)<\exp\left(-ts+\frac{t^2}{2}\sum_i c_i^2\right).
$$

The strict inequality follows directly by integrating $e^{t(M_n-M_0)}>e^{ts}$ on that event; it is also immediate if the event is empty. Optimize at $t=s/\sum_i c_i^2$ and apply the same argument to the negative increments. For $c_i=1$ and $s=\lambda\sqrt n$, the [union bound](../../../probability-inequality.md#boole-s-inequality) proves, for every $\lambda>0$,

$$
\boxed{\mathbb P(|\chi(G)-\mu|>\lambda\sqrt n)<2e^{-\lambda^2/2}.}
$$

At $\lambda=0$ the displayed strict bound is trivial.

For the second conclusion write $a_n=n/\log n$ and choose a fixed $C>\sqrt{2\log10}$. If $\mu\geq a_n+C\sqrt n$, then $\{\chi(G)<a_n\}\subseteq\{\chi(G)-\mu<-C\sqrt n\}$, whose [probability](../../../probability-theory.md#probability) is less than $e^{-C^2/2}<1/10$. Thus the given positive [probability](../../../probability-theory.md#probability) forces $\mu<a_n+C\sqrt n$. For sufficiently large $n$,

$$
\mathbb P\bigl(\chi(G)\geq a_n+(\log n)\sqrt n\bigr)
\leq\exp\left(-\frac{(\log n-C)^2}{2}\right)\longrightarrow0.
$$

Here the non-strict one-sided bound follows by the usual non-strict [Markov inequality](../../../probability-inequality.md#markov-inequality). Consequently **the asserted upper bound holds [with high probability](../../../probabilistic-combinatorics.md#with-high-probability)**, uniformly over any sequence $p=p(n)$ satisfying the stated assumption.

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

We use the [random alteration method](../../../probabilistic-combinatorics.md#random-alteration-method), controlling large [hypergraph independent sets](../../../hypergraph.md#hypergraph-independent-set) and then removing the few forbidden overlaps. Fix $k=2005$, let $n$ tend to infinity, and independently include each three-element subset of an $n$-vertex set as an [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) with [probability](../../../probability-theory.md#probability) $p=n^{-7/4}$. Call the resulting three-[uniform hypergraph](../../../hypergraph.md#uniform-hypergraph) $H_0$, and let $s=\lceil n/(2k)\rceil$.

For any prescribed $s$-vertex set, the [probability](../../../probability-theory.md#probability) that it is a [hypergraph independent set](../../../hypergraph.md#hypergraph-independent-set) is $(1-p)^{\binom s3}$. Hence the [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P\bigl(H_0\text{ has an independent set of size }s\bigr)
\leq\binom ns(1-p)^{\binom s3}
\leq\exp\bigl(n\log2-p\tbinom s3\bigr)\longrightarrow0,
$$

because $p\binom s3$ has order $n^{5/4}$, with a positive constant depending only on $k$.

Let $Y$ count [unordered pairs](../../../set.md#unordered-pair) of distinct [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) meeting in two vertices. Each potential pair consists of its common pair and two distinct additional vertices, so

$$
\mathbb E Y=\binom n2\binom{n-2}2p^2=O(n^{1/2}).
$$

The [Markov inequality](../../../probability-inequality.md#markov-inequality) implies $\mathbb P(Y\geq n/2)=O(n^{-1/2})$. We may therefore fix one realization for which $Y<n/2$ and no $s$-vertex [hypergraph independent set](../../../hypergraph.md#hypergraph-independent-set) exists. For each offending [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) pair choose one vertex from its union, and let $D$ be the set of all chosen vertices. Delete $D$, together with all incident [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph), and call the induced [hypergraph](../../../hypergraph.md) $H$. Then $|D|\leq Y<n/2$, so $N=|V(H)|>n/2$. The next two parts verify both desired properties of this same $H$.

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Every [hypergraph independent set](../../../hypergraph.md#hypergraph-independent-set) in the induced [hypergraph](../../../hypergraph.md) $H$ is also a [hypergraph independent set](../../../hypergraph.md#hypergraph-independent-set) in $H_0$. Thus its maximum independent-set size is at most $s-1<n/(2k)<N/k$. In any proper [hypergraph colouring](../../../hypergraph.md#hypergraph-colouring) with at most $k$ colours, one [colour class](../../../ramsey-theory.md#colour-class) would have at least $N/k$ vertices, contradicting that bound. Therefore

$$
\boxed{\chi(H)>2005,\quad\text{hence}\quad\chi(H)\geq2006.}
$$

This is the weak [hypergraph colouring](../../../hypergraph.md#hypergraph-colouring) convention: an [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) may use two colours, but it may not be [monochromatic](../../../ramsey-theory.md#monochromatic-set).

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

If two distinct [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) survived in $H$ and shared two vertices, they were an offending pair in $H_0$. The deletion set $D$ contains a chosen vertex from their union, so at least one of those [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) could not have survived. This contradiction proves that **$H$ is a [linear hypergraph](../../../hypergraph.md#linear-hypergraph)**. Deleting vertices leaves every surviving [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) of size three, so the construction meets the uniformity requirement as well as the chromatic-number requirement.

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Colour every vertex independently red or blue, each with [probability](../../../probability-theory.md#probability) $1/2$. A fixed $r$-element [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) is [monochromatic](../../../ramsey-theory.md#monochromatic-set) with [probability](../../../probability-theory.md#probability) $2^{1-r}$. If there are $m<2^{r-1}$ [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph), the expected number of [monochromatic](../../../ramsey-theory.md#monochromatic-set) [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) is $m2^{1-r}<1$. Equivalently, the [union bound](../../../probability-inequality.md#boole-s-inequality) says that the [probability](../../../probability-theory.md#probability) of even one [monochromatic](../../../ramsey-theory.md#monochromatic-set) [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) is less than one. **A proper two-colouring therefore exists.**

For the converse, suppose $r\geq2$, put $N=2r^2$, and sample $m$ [independent](../../../random-variable.md#independent-random-variables) uniformly random $r$-subsets of an $N$-vertex set. Initially this is a [multihypergraph](../../../hypergraph.md#multihypergraph). For a fixed two-colouring with $a$ red vertices, a sampled [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) is [monochromatic](../../../ramsey-theory.md#monochromatic-set) with [probability](../../../probability-theory.md#probability)

$$
q(a)=\frac{\binom ar+\binom{N-a}r}{\binom Nr}.
$$

The numerator is minimized by $a=N/2=r^2$. To see this discretely, use $\binom{a+1}r-\binom ar=\binom a{r-1}$: the successive difference of the numerator is $\binom a{r-1}-\binom{N-a-1}{r-1}$, negative up to the middle and positive afterwards. [Binomial coefficients](../../../combinatorics.md#binomial-coefficient) with an upper index below $r$ are understood as zero.

For this balanced colouring,

$$
q(a)\geq2\frac{\binom{r^2}r}{\binom{2r^2}r}
=2^{1-r}\prod_{j=0}^{r-1}\frac{1-j/r^2}{1-j/(2r^2)}
\geq2^{1-r}\prod_{j=0}^{r-1}(1-j/r^2).
$$

The elementary inequality $\prod_j(1-u_j)\geq1-\sum_j u_j$, valid for $0\leq u_j\leq1$, gives

$$
q(a)\geq2^{1-r}\left(1-\frac{r(r-1)}{2r^2}\right)>2^{-r}.
$$

Thus any fixed colouring is proper for all the sampled [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) with [probability](../../../probability-theory.md#probability) at most $e^{-m2^{-r}}$. There are $2^N$ colourings, so choose

$$
m=\left\lceil(N\log2+1)2^r\right\rceil.
$$

A [union bound](../../../probability-inequality.md#boole-s-inequality) makes the [probability](../../../probability-theory.md#probability) that any proper colouring exists at most $2^Ne^{-m2^{-r}}\leq e^{-1}<1$. Some sampled [multihypergraph](../../../hypergraph.md#multihypergraph) is consequently not two-colourable. Remove repeated copies of its [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph): this changes neither which colourings are proper nor non-two-colourability, and leaves at most $m$ distinct [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph). We have proved

$$
\boxed{\text{There is an }r\text{-uniform hypergraph without Property B with }O(r^22^r)\text{ edges}.}
$$

For $r=1$, one singleton [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) is already not two-colourable, so that endpoint causes no exception.

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $Y$ be the number of [isolated vertices](../../../graph-theory.md#isolated-vertex) and set $\lambda=e^{-c}$. For fixed $k\geq1$, the [falling factorial](../../../combinatorics.md#falling-factorial) $(Y)_k$ counts ordered $k$-tuples of distinct [isolated vertices](../../../graph-theory.md#isolated-vertex). A specified tuple is isolated exactly when all [edges](../../../graph-theory.md#edge-of-a-graph) incident to its vertices are absent. There are $k(n-k)+\binom k2$ such [edges](../../../graph-theory.md#edge-of-a-graph), so

$$
\mathbb E(Y)_k=(n)_k(1-p)^{k(n-k)+\binom k2}.
$$

Since $np=\log n+c$ and $np^2=o(1)$, taking [logarithms](../../../calculus.md#logarithm) gives

$$
\log\mathbb E(Y)_k=k\log n-k(\log n+c)+o(1)=-kc+o(1).
$$

Thus every fixed [factorial moment](../../../markov-process.md#factorial-moment) tends to $\lambda^k$. We use the standard [factorial-moment criterion for Poisson convergence](../../../markov-process.md#factorial-moment-criterion-for-poisson-convergence): nonnegative integer-valued [random variables](../../../random-variable.md) whose [factorial moments](../../../markov-process.md#factorial-moment) converge, for every fixed order, to $\lambda^k$ converge in distribution to $\operatorname{Poisson}(\lambda)$. Consequently $Y$ has that limiting distribution, and its mass at each fixed integer converges. In particular,

$$
\boxed{\mathbb P(Y\geq1)\longrightarrow1-e^{-e^{-c}}.}
$$

This establishes the limiting [probability](../../../probability-theory.md#probability) of at least one [isolated vertex](../../../graph-theory.md#isolated-vertex), rather than merely a bound based on its [expectation](../../../probability-theory.md#expected-value).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The factorial-moment argument above gives $Y\Rightarrow\operatorname{Poisson}(\lambda)$ with $\lambda=e^{-c}$. Because $Y$ is integer-valued, apply [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) at the continuity points $3/2$ and $5/2$ and subtract. This proves

$$
\boxed{\mathbb P(Y=2)\longrightarrow e^{-e^{-c}}\frac{e^{-2c}}2.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A [connected graph](../../../graph.md#connected-graph) with $n>1$ has no [isolated vertices](../../../graph-theory.md#isolated-vertex). Conversely, a disconnected [graph](../../../graph.md) with no [isolated vertices](../../../graph-theory.md#isolated-vertex) has a [connected component](../../../geometry-and-topology.md#connected-component) with size between $2$ and $n/2$. We must show that this latter event has [probability](../../../probability-theory.md#probability) tending to zero.

The permitted component-size estimate excludes sizes between $\log\log n$ and $n/2$ [with high probability](../../../probabilistic-combinatorics.md#with-high-probability). For the remaining small sizes, let $C_k$ count components with $k$ vertices. A [connected graph](../../../graph.md#connected-graph) on a fixed $k$-vertex set contains a [spanning tree](../../../combinatorics.md#spanning-tree). By the [Cayley formula](../../../combinatorics.md#cayley-s-formula), there are $k^{k-2}$ labelled [trees](../../../combinatorics.md#tree-graph-theory), as follows from the [Prüfer code](../../../combinatorics.md#prufer-sequence) [bijection](../../../function.md#bijection) between labelled [trees](../../../combinatorics.md#tree-graph-theory) and sequences of $k-2$ labels. A [union bound](../../../probability-inequality.md#boole-s-inequality) over the [trees](../../../combinatorics.md#tree-graph-theory), together with the absence of every [edge](../../../graph-theory.md#edge-of-a-graph) to the complementary [vertex set](../../../graph.md#vertex-set), gives

$$
\mathbb E C_k\leq\binom nk k^{k-2}p^{k-1}(1-p)^{k(n-k)}.
$$

Put $a=np=\log n+c$ and $L=\lceil\log\log n\rceil$. Using $\binom nk\leq(en/k)^k$ and $1-p\leq e^{-p}$, uniformly for $2\leq k\leq L$ we obtain

$$
\mathbb E C_k\leq\frac{n}{a k^2}\left(\frac{e^{1-c}a}{n}\right)^k e^{pk^2}.
$$

Here $pL^2\to0$. Therefore, with $\rho_n=e^{1-c}a/n\to0$,

$$
\sum_{k=2}^L\mathbb E C_k
\leq\frac{2n}{a}\sum_{k=2}^{\infty}\rho_n^k
=O(a/n)\longrightarrow0.
$$

The [Markov inequality](../../../probability-inequality.md#markov-inequality) excludes all these small components [with high probability](../../../probabilistic-combinatorics.md#with-high-probability). Together with the permitted estimate, this proves that the difference between the [probability](../../../probability-theory.md#probability) of connectivity and the [probability](../../../probability-theory.md#probability) of no [isolated vertices](../../../graph-theory.md#isolated-vertex) tends to zero. Hence

$$
\boxed{\mathbb P(G\text{ is connected})\longrightarrow e^{-e^{-c}}.}
$$

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the unheaded degree-one continuation, write $X=\sum_{v=1}^n I_v$, where $I_v$ indicates that vertex $v$ has degree one. With

$$
q=\mathbb P(I_v=1)=(n-1)p(1-p)^{n-2},
$$

we have

$$
\mathbb E X=nq\sim e^{-c}(\log n+c)\longrightarrow\infty.
$$

For distinct vertices $u,v$, separate the cases where their connecting [edge](../../../graph-theory.md#edge-of-a-graph) is present or absent. If it is present, all their other incident [edges](../../../graph-theory.md#edge-of-a-graph) must be absent. If it is absent, each vertex chooses its unique neighbour among the other $n-2$ vertices; those two neighbours may coincide. The respective [edge](../../../graph-theory.md#edge-of-a-graph) constraints are [independent](../../../random-variable.md#independent-random-variables) even in that case. Thus

$$
\mathbb E(I_uI_v)=p(1-p)^{2n-4}+(n-2)^2p^2(1-p)^{2n-5}.
$$

Dividing by $q^2$ gives the exact ratio

$$
R_n=\frac{1}{(n-1)^2p}+\left(\frac{n-2}{n-1}\right)^2\frac{1}{1-p}\longrightarrow1.
$$

The first term tends to zero because $(n-1)^2p$ has order $n\log n$; the second tends to one. Consequently its [variance](../../../variance.md) satisfies

$$
\frac{\operatorname{Var}X}{(\mathbb EX)^2}
=\frac{1}{nq}+\left(1-\frac1n\right)R_n-1\longrightarrow0.
$$

The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) now yields $\mathbb P(X=0)\leq\operatorname{Var}X/(\mathbb EX)^2\to0$. **A vertex of degree one exists [with high probability](../../../probabilistic-combinatorics.md#with-high-probability)**, even though the limiting [probability](../../../probability-theory.md#probability) of having an [isolated vertex](../../../graph-theory.md#isolated-vertex) is strictly between zero and one.

## 5

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The general, or [asymmetric Lovász local lemma](../../../probabilistic-combinatorics.md#asymmetric-lovasz-local-lemma), is as follows. Let $E_1,\ldots,E_m$ be events, with a [dependency graph of events](../../../probabilistic-combinatorics.md#dependency-graph-of-events) having neighbour sets $N(i)$. Each $E_i$ must be [independent](../../../random-variable.md#independent-random-variables) of the sigma-algebra generated by all the events indexed by its nonneighbours. If numbers $0\leq x_i<1$ satisfy

$$
\mathbb P(E_i)\leq x_i\prod_{j\in N(i)}(1-x_j),
$$

then

$$
\mathbb P\left(\bigcap_{i=1}^m E_i^c\right)\geq\prod_{i=1}^m(1-x_i)>0.
$$

For completeness, the key inductive bound is $\mathbb P(E_i\mid\bigcap_{j\in S}E_j^c)\leq x_i$ whenever $i\notin S$. Split $S$ into neighbours $S_1$ of $i$ and nonneighbours $S_2$. If $S_1$ is empty, the dependency condition gives the bound directly. Otherwise,

$$
\mathbb P\left(E_i\mid\bigcap_{j\in S}E_j^c\right)
\leq\frac{\mathbb P(E_i\mid\bigcap_{j\in S_2}E_j^c)}{\mathbb P(\bigcap_{j\in S_1}E_j^c\mid\bigcap_{j\in S_2}E_j^c)}
\leq\frac{\mathbb P(E_i)}{\prod_{j\in S_1}(1-x_j)}\leq x_i.
$$

The denominator bound follows by exposing the exclusions in $S_1$ one at a time and using the induction hypothesis with strictly fewer conditioning events. The same induction ensures that all conditioning events have positive [probability](../../../probability-theory.md#probability). Finally multiply the successive [conditional probabilities](../../../probability-theory.md#conditional-probability) of avoiding $E_1,\ldots,E_m$ to obtain the stated lower bound.

For the symmetric form, suppose each event has [probability](../../../probability-theory.md#probability) at most $q$ and the dependency [graph](../../../graph.md) has maximum degree $D\geq1$. Choose $x_i=1/(D+1)$. Then

$$
x_i\prod_{j\in N(i)}(1-x_j)
\geq\frac{1}{D+1}\left(\frac{D}{D+1}\right)^D
\geq\frac{1}{e(D+1)}.
$$

The final inequality follows from $(1+1/D)^D\leq e$. Thus **$eq(D+1)\leq1$ suffices for positive [probability](../../../probability-theory.md#probability) that no bad event occurs**. If $D=0$, the dependency condition gives joint [independence](../../../random-variable.md#independent-random-variables) and the same criterion implies $q<1$, so the conclusion follows directly.

Apply this to a fair [independent](../../../random-variable.md#independent-random-variables) two-colouring of the [hypergraph](../../../hypergraph.md) vertices, with $E_W$ the event that [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) $W$ is [monochromatic](../../../ramsey-theory.md#monochromatic-set). Its [probability](../../../probability-theory.md#probability) is $q=2^{1-r}$. Events on disjoint [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) use disjoint [independent](../../../random-variable.md#independent-random-variables) variables, giving a dependency [graph](../../../graph.md) by joining intersecting [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph). Each [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) meets at most

$$
D\leq\sum_{v\in W}(d_H(v)-1)\leq r(\Delta-1)
$$

other [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph); repeated counting only enlarges this upper bound. The slightly looser bound $D+1\leq r(\Delta+1)$ is enough for the printed condition. Indeed,

$$
\Delta<\frac{2^r}{2re}-1
\quad\Longrightarrow\quad
 e,2^{1-r}(D+1)\leq e,2^{1-r}r(\Delta+1)<1.
$$

The symmetric [Lovász local lemma](../../../probabilistic-combinatorics.md#lovasz-local-lemma) therefore gives **a proper two-colouring**. A [hypergraph](../../../hypergraph.md) with no [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) is trivially colourable and needs no dependency calculation.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $S$ be the number of red vertices in $W$. It has a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $r$ and $1/2$, so [independence](../../../random-variable.md#independent-random-variables) gives

$$
\mathbb E e^{t(S-r/2)}=\left(\cosh(t/2)\right)^r.
$$

For $t=1$, the strict inequality $\log\cosh(1/2)<1/8$ follows by integrating $\tanh u<u$ for $u>0$. Hence the [exponential Markov bound](../../../probability-inequality.md#exponential-markov-bound) yields

$$
\mathbb P(S>3r/4)
\leq e^{-r/4}\left(\cosh(1/2)\right)^r
<e^{-r/4+r/8}.
$$

Therefore

$$
\boxed{\mathbb P(S>3r/4)<e^{-r/8}.}
$$

This supplies the tail estimate directly, including the strict constant in the requested bound.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

For each [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) $W$, let $B_W$ be the event that one of its two colours occupies more than $3r/4$ vertices. By colour symmetry and the [union bound](../../../probability-inequality.md#boole-s-inequality), the preceding calculation gives

$$
\mathbb P(B_W)<2e^{-r/8}.
$$

Again the dependency [graph](../../../graph.md) joins intersecting [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) and has $D+1\leq r(\Delta+1)$. The assumed degree bound implies

$$
 e\,(2e^{-r/8})(D+1)
\leq2er e^{-r/8}(\Delta+1)<1.
$$

The symmetric [Lovász local lemma](../../../probabilistic-combinatorics.md#lovasz-local-lemma) gives positive [probability](../../../probability-theory.md#probability) that no $B_W$ occurs. Thus **there is a two-colouring in which each colour occupies at most $3r/4$ vertices of every [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph)**. Equivalently, both colour counts in every [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) lie between $r/4$ and $3r/4$; no rounding difficulty arises because the counts are integers and the bad events use strict inequalities.

## 6

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

We prove both inequalities, including the [BK inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality), for the inhomogeneous [product measure](../../../probability-theory.md#product-measure) in the question. Identify a configuration with its set of coordinates equal to one. An up-set is then an [increasing event](../../../probability-inequality.md#increasing-event). For an [increasing event](../../../probability-inequality.md#increasing-event) $A$, a set $S$ of open coordinates is a witness if the configuration with precisely $S$ open belongs to $A$: upward closure ensures that those coordinates alone force $A$, whatever the remaining coordinates do. The event $A\square B$ means that there are disjoint open witnesses $S,T$ for $A,B$ respectively.

First prove the [Harris' inequality](../../../probability-inequality.md#harris-inequality) by induction on the number of coordinates. For the last coordinate, of parameter $p$, write $A_0\subseteq A_1$ and $B_0\subseteq B_1$ for the two sections in the remaining coordinates, and put $a_i=\mathbb P(A_i)$, $b_i=\mathbb P(B_i)$. Induction applied to each section gives

$$
\mathbb P(A\cap B)\geq(1-p)a_0b_0+p a_1b_1.
$$

Subtract the product of the marginal [probabilities](../../../probability-theory.md#probability) from the right-hand side:

$$
(1-p)a_0b_0+p a_1b_1-\bigl((1-p)a_0+p a_1\bigr)\bigl((1-p)b_0+p b_1\bigr)
=p(1-p)(a_1-a_0)(b_1-b_0)\geq0.
$$

The base case of zero coordinates is immediate. Thus

$$
\boxed{\mathbb P(A\cap B)\geq\mathbb P(A)\mathbb P(B).}
$$

For disjoint occurrence, first assume every coordinate parameter is at most $1/2$, and again use induction. Put $c_{ij}=\mathbb P(A_i\square B_j)$ on the remaining coordinates. The zero-section of $A\square B$ is exactly $A_0\square B_0$. The one-section is exactly

$$
(A_1\square B_0)\cup(A_0\square B_1).
$$

Indeed, the last open coordinate can belong to at most one of two disjoint witnesses. Assigning it to the $A$ witness leaves a witness for $A_1$ and a witness for $B_0$; assigning it to the $B$ witness gives the other event. If neither witness uses it, both descriptions still hold. Conversely, witnesses for either displayed event lift to disjoint witnesses by adding the last coordinate only to the appropriate one.

The intersection of the two displayed events contains $A_0\square B_0$, because the sections are increasing. Therefore

$$
\mathbb P(A\square B)\leq(1-p)c_{00}+p(c_{10}+c_{01}-c_{00})
=(1-2p)c_{00}+p c_{10}+p c_{01}.
$$

The coefficient $1-2p$ is nonnegative. Applying the induction hypothesis to each term gives

$$
\mathbb P(A\square B)\leq(1-2p)a_0b_0+p a_1b_0+p a_0b_1.
$$

The product of the marginal [probabilities](../../../probability-theory.md#probability) is exactly this last expression plus

$$
p^2(a_1-a_0)(b_1-b_0)\geq0.
$$

This proves the desired inequality whenever every parameter is at most $1/2$.

To remove that restriction, suppose first $p_i<1$ for every coordinate. Replace coordinate $i$ by the [logical disjunction](../../../mathematical-logic.md#logical-disjunction) of $m_i$ [independent](../../../random-variable.md#independent-random-variables) [Bernoulli](../../../discrete-probability-distribution.md#bernoulli-distribution) bits, each with parameter

$$
q_i=1-(1-p_i)^{1/m_i}.
$$

Choose $m_i$ large enough that $q_i\leq1/2$. Different blocks are [independent](../../../random-variable.md#independent-random-variables), and their OR values have exactly the original distribution. Let $\widetilde A,\widetilde B$ be the inverse images of $A,B$ under this block-OR map; they are [increasing events](../../../probability-inequality.md#increasing-event). If the OR configuration has disjoint witnesses $S,T$, choose one open bit from each block indexed by $S$ or $T$. The bits chosen for $S$ force $\widetilde A$, those for $T$ force $\widetilde B$, and the two bit sets are disjoint. Thus the inverse image of $A\square B$ is contained in $\widetilde A\square\widetilde B$. The small-parameter result proves

$$
\mathbb P(A\square B)
\leq\mathbb P(\widetilde A\square\widetilde B)
\leq\mathbb P(\widetilde A)\mathbb P(\widetilde B)
=\mathbb P(A)\mathbb P(B).
$$

Parameters equal to one follow by a [limit](../../../calculus.md#limit-of-a-function): [probabilities](../../../probability-theory.md#probability) of any fixed event on a finite cube are [polynomials](../../../polynomial.md) in the coordinate parameters, hence continuous. Zero parameters already cause no difficulty. We have obtained

$$
\boxed{\mathbb P(A\square B)\leq\mathbb P(A)\mathbb P(B).}
$$

For the [graph](../../../graph.md) application, take coordinates to be the [edges](../../../graph-theory.md#edge-of-a-graph) of the [complete graph](../../../graph-theory.md#complete-graph). Let $A$ be the [increasing event](../../../probability-inequality.md#increasing-event) that $x$ is connected by a [graph path](../../../graph-theory.md#path-in-a-graph) to $U$, and $B$ the corresponding event for $W$. Their [probabilities](../../../probability-theory.md#probability) are $\alpha,\beta$. A simple [graph path](../../../graph-theory.md#path-in-a-graph) from $U$ to $W$ through $x$ splits at $x$ into two [graph paths](../../../graph-theory.md#path-in-a-graph) with disjoint [edge](../../../graph-theory.md#edge-of-a-graph) sets. Those sets witness $A$ and $B$, so this [graph path](../../../graph-theory.md#path-in-a-graph) event is contained in $A\square B$. The [BK inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) gives

$$
\boxed{\mathbb P(\text{a }U\text{--}W\text{ path through }x)\leq\alpha\beta.}
$$

On the other hand, if both $A$ and $B$ occur, concatenate an $x$-to-$U$ [graph path](../../../graph-theory.md#path-in-a-graph) and an $x$-to-$W$ [graph path](../../../graph-theory.md#path-in-a-graph) to obtain a walk from $U$ to $W$. Removing loops yields a simple [graph path](../../../graph-theory.md#path-in-a-graph), although it need not pass through $x$. Thus $A\cap B$ is contained in the unrestricted connection event, and the [Harris' inequality](../../../probability-inequality.md#harris-inequality) gives

$$
\boxed{\mathbb P(\text{a }U\text{--}W\text{ path})\geq\mathbb P(A\cap B)\geq\alpha\beta.}
$$

The distinction between a simple [graph path](../../../graph-theory.md#path-in-a-graph) through $x$ and an unrestricted connection is essential: a walk may revisit an [edge](../../../graph-theory.md#edge-of-a-graph), so a through-$x$ walk would not in general provide disjoint witnesses.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
