<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $R$ interchange the two [complete graphs](../../../../../../complete-graph.md), sending $v_i$ to $v_i'$ and fixing $w$. This [involution](../../../../../../involution.md) preserves the [transition matrix](../../../../../../stochastic-matrix.md) of the [simple random walk](../../../../../../simple-random-walk.md). A [mirror coupling under an involution](../../../../../../mirror-coupling-under-an-involution.md) starts $X$ at $v_i$, keeps $Y_t=R(X_t)$ until the [hitting time](../../../../../../first-passage-time.md) $\tau$ of $w$, and then makes the two walks move identically. Each coordinate has the correct [transition probabilities](../../../../../../transition-probability.md), and they coalesce precisely at $\tau$. The [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md) gives

$$
\boxed{\|P^t(v_i,\cdot)-P^t(v_i',\cdot)\|_{\mathrm{TV}}\leq\mathbb P_{v_i}(\tau>t).}
$$

There is a genuine error in the printed [expected hitting time](../../../../../../expected-hitting-time.md) bound, as well as an unspecified initial law. For $n\geq2$, write $a=\mathbb E_{v_1}\tau$ and $b=\mathbb E_{v_i}\tau$ for $i\ne1$. From every clique vertex there is a positive chance of reaching $w$ within two steps, uniformly over the finite state space for each fixed $n$, so $\tau$ has finite [expected value](../../../../../../expected-value.md). [First-step analysis](../../../../../../first-step-analysis.md), using the [degree of a vertex](../../../../../../degree-graph-theory.md) $n$ at $v_1$ and $n-1$ at the other clique vertices, gives

$$
a=1+\frac{n-1}{n}b,\qquad b=1+\frac{a+(n-2)b}{n-1}.
$$

Solving these [linear equations](../../../../../../linear-equation.md) yields

$$
\boxed{a=n^2-n+1,\qquad b=n^2,\qquad \mathbb E_w\tau=0.}
$$

In particular even the attachment vertex exceeds the printed bound by one. The valid uniform replacement is $\max_x\mathbb E_x\tau\leq n^2$, the [hitting time of the bridge vertex between two cliques](../../../../../../hitting-time-of-the-bridge-vertex-between-two-cliques.md) formula.

We must also handle arbitrary starting states, including $w$, before applying the mirror argument. Identify related vertices and consider the [lumped Markov chain](../../../../../../lumped-markov-chain.md) $Z$ on $\{1,\ldots,n,w\}$. Its [transition matrix](../../../../../../stochastic-matrix.md) $Q$ has $Q(1,j)=1/n$ for $j\ne1$, $Q(1,w)=1/n$, $Q(i,j)=1/(n-1)$ for $i\ne1$ and $j\ne i$, and $Q(w,1)=1$, with all other entries zero. Here the row for $i\ne1$ only ranges over $j\in\{1,\ldots,n\}$.

For $n\geq3$ and $j\in\{2,\ldots,n\}$, direct two-step calculation gives

$$
\begin{aligned}
Q^2(w,j)&=1/n, &Q^2(1,j)&=(n-2)/(n(n-1)),\\
Q^2(i,i)&=(n-2)/(n-1)^2+1/(n(n-1)),\quad&i\geq2,\\
Q^2(i,j)&=(n-3)/(n-1)^2+1/(n(n-1)),\quad&i,j\geq2,\ i\ne j.
\end{aligned}
$$

All these entries are at least $1/(2n)$. Thus $Q^2(z,\cdot)\geq\alpha\nu(\cdot)$ for every $z$, where $\nu$ is the [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md) $\{2,\ldots,n\}$ and $\alpha=(n-1)/(2n)\geq1/3$. This is a [Doeblin condition](../../../../../../doeblin-s-condition.md). At each two-step block couple the two quotient endpoints to the same sample from $\nu$ with probability $\alpha$, using the residual [probability distributions](../../../../../../probability-distribution.md) otherwise. The first successful block has [expected value](../../../../../../expected-value.md) at most $1/\alpha$, so the alignment time $A$ has $\mathbb E A\leq6$. Lift each endpoint [coupling of probability distributions](../../../../../../coupling.md) to the original walks by their conditional two-step path laws; this preserves every marginal path law. The success test uses fresh block randomness and so permits restarting the walks with their original [transition matrix](../../../../../../stochastic-matrix.md) at the aligned endpoints.

At alignment the original walks are equal or related. Use identical transitions in the first case and the [mirror coupling under an involution](../../../../../../mirror-coupling-under-an-involution.md) in the second. The resulting [coalescing coupling](../../../../../../coalescing-coupling.md) has coalescence time $T$ satisfying $\mathbb E T\leq6+n^2$ for every pair of initial states. Therefore [Markov inequality](../../../../../../markov-inequality.md) and the [pairwise mixing diameter](../../../../../../pairwise-mixing-diameter.md) imply

$$
d(t)\leq\bar d(t)\leq\sup_{x,y}\mathbb P_{x,y}(T>t)\leq\frac{n^2+6}{t},\qquad
\boxed{t_{\mathrm{mix}}(1/4)\leq\lceil4(n^2+6)\rceil=O(n^2).}
$$

For the hint's particular starting states, the quotient one-step laws from two different clique indices have a common component of mass at least $1-2/n$: for two ordinary indices it is $(n-2)/(n-1)$; for one attachment index it is $(n-2)/n$. A [maximal coupling](../../../../../../maximal-coupling.md) therefore aligns those indices with probability $1-O(1/n)$, as suggested. The two-step argument above additionally covers $w$.

The nonlazy walk is an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md) for $n\geq3$, because the connected [graph](../../../../../../graph-split.md) contains a [triangle](../../../../../../triangle.md). For $n=1,2$ it is a [periodic Markov chain](../../../../../../periodic-markov-chain.md) on a [bipartite graph](../../../../../../bipartite-graph.md); each bipartition class has stationary mass $1/2$, and the walk stays on a single class at each time. Hence $d(t)\geq1/2$ and the $1/4$ [mixing time](../../../../../../mixing-time-of-a-markov-chain.md) is infinite. The asymptotic conclusion is valid for $n\geq3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
