<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $P$ be the transition matrix of a finite [irreducible Markov chain](../../../../../irreducible-markov-chain.md) with at least two states, reversible with [stationary distribution](../../../../../stationary-distribution.md) $\pi$. Its [Dirichlet form of a Markov chain](../../../../../dirichlet-form-of-a-markov-chain.md) is

$$
\mathcal E(f,f)=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2.
$$

The [Discrete Poincare inequality](../../../../../poincare-inequality-for-a-reversible-markov-chain.md) states that $\operatorname{Var}_\pi f\leq C\mathcal E(f,f)$ for every real $f$. Its optimal constant is $C=(1-\lambda_2)^{-1}$, where $\lambda_2$ is the second largest [eigenvalue](../../../../../eigenvalue.md) of $P$. Indeed, [detailed balance](../../../../../detailed-balance.md) makes $P$ [self-adjoint](../../../../../self-adjoint-operator.md) on $L^2(\pi)$. Expand $f-\pi(f)=\sum_{j\geq2}a_jv_j$ in an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md). Then $\operatorname{Var}_\pi f=\sum a_j^2$ and $\mathcal E(f,f)=\sum(1-\lambda_j)a_j^2$, proving the inequality and its sharpness.

The useful constructive version is the [canonical paths Poincare bound](../../../../../canonical-paths-poincare-bound.md). Choose transition [graph paths](../../../../../path-in-a-graph.md) $\gamma_{xy}$ between each ordered pair, write $Q(u,v)=\pi(u)P(u,v)$, and define

$$
\rho=\max_{(u,v):Q(u,v)>0}\frac1{Q(u,v)}
\sum_{x,y}\pi(x)\pi(y)|\gamma_{xy}|N_{uv}(\gamma_{xy}),
$$

where $N_{uv}$ counts occurrences of the directed transition. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) along each [path in a graph](../../../../../path-in-a-graph.md) gives $(f(x)-f(y))^2\leq|\gamma_{xy}|\sum_{\gamma_{xy}}(f(u)-f(v))^2$. Multiply by $\pi(x)\pi(y)/2$ and sum. The identity $\operatorname{Var}_\pi f=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2$ proves $\operatorname{Var}_\pi f\leq\rho\mathcal E(f,f)$.

For a [lazy Markov chain](../../../../../lazy-markov-chain.md) this also proves the [mixing time](../../../../../mixing-time-of-a-markov-chain.md) estimate

$$
\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}
\leq\frac1{2\sqrt{\pi(x)}}e^{-t/\rho}.
$$

To see this, the centred initial density has $L^2(\pi)$ norm at most $\pi(x)^{-1/2}$; laziness puts all nonconstant [eigenvalues](../../../../../eigenvalue.md) between zero and $1-\rho^{-1}$. Their powers contract that norm, and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds [total variation distance](../../../../../total-variation-distance.md) by half the density's $L^2(\pi)$ norm.

Here is a precise sufficient density condition for the permanent application: **every row and every column has more than $n/2$ ones**. Interpret the [permanent of a matrix](../../../../../permanent-mathematics.md) as the number $m_n$ of [perfect matchings](../../../../../perfect-matching.md) in its [bipartite graph](../../../../../bipartite-graph.md), with $n$ [vertices](../../../../../vertex-graph-theory.md) per side. Write $m_k$ for the number of $k$-edge [matchings in a graph](../../../../../matching-graph-theory.md).

First prove the [short augmenting paths in a dense bipartite graph](../../../../../short-augmenting-paths-in-a-dense-bipartite-graph.md) bound. Given a nonperfect [matching in a graph](../../../../../matching-graph-theory.md), choose unmatched $u,v$ on opposite sides. If either has an unmatched [neighbour](../../../../../neighbour-of-a-vertex.md), augment with one [edge](../../../../../edge-of-a-graph.md). Otherwise the matched partners of $N(u)$ and the [neighbours](../../../../../neighbour-of-a-vertex.md) $N(v)$ are subsets of the same $n$-element side whose total size exceeds $n$. Their intersection gives an alternating [path in a graph](../../../../../path-in-a-graph.md) $u,b,a,v$ of length three, with $ab$ a matching [edge](../../../../../edge-of-a-graph.md). Repeating proves $m_n>0$. Choose augmentations by a fixed deterministic rule. A reverse augmentation is specified by at most four [vertices](../../../../../vertex-graph-theory.md), so a next-size [matching in a graph](../../../../../matching-graph-theory.md) has at most $C_0=2n^4$ preimages. Therefore

$$
m_k\leq C_0m_{k+1},\qquad m_{n-j}\leq C_0^jm_n.
$$

Use the [matching generating function](../../../../../matching-generating-function.md) $Z(\lambda)=\sum_{k=0}^nm_k\lambda^k$ and the [weighted matching Markov chain](../../../../../weighted-matching-markov-chain.md) on all [matchings in a graph](../../../../../matching-graph-theory.md), with stationary weights $\pi_\lambda(M)=\lambda^{|M|}/Z(\lambda)$. It stays put with probability $1/2$; otherwise it chooses a [graph](../../../../../graph-split.md) [edge](../../../../../edge-of-a-graph.md) uniformly and proposes its deletion, its addition if both endpoints are unmatched, or its exchange for the unique incident matching [edge](../../../../../edge-of-a-graph.md) if precisely one endpoint is matched. Other proposals stay put. Accept with probability $\min(1,\lambda^{|M'|-|M|})$. Reverse proposals use the opposite exchanged [edge](../../../../../edge-of-a-graph.md), so [detailed balance](../../../../../detailed-balance.md) holds. Deletions connect every state to the empty [matching in a graph](../../../../../matching-graph-theory.md).

For completeness, the [canonical paths for the weighted matching chain](../../../../../canonical-paths-for-the-weighted-matching-chain.md) give a polynomial bound without assuming a mixing theorem. The [symmetric difference](../../../../../symmetric-difference.md) $I\triangle F$ consists of alternating [graph paths](../../../../../path-in-a-graph.md) and [graph cycles](../../../../../cycle-in-a-graph.md). Order its components deterministically, orient open components from their smaller endpoint, and convert them from $I$ to $F$ by moving an unmatched endpoint with exchanges. If the first [edge](../../../../../edge-of-a-graph.md) belongs to $I$, delete it first. For a [graph cycle](../../../../../cycle-in-a-graph.md), delete one $I$-[edge](../../../../../edge-of-a-graph.md), move the unmatched endpoint around the opened cycle, then insert the last $F$-[edge](../../../../../edge-of-a-graph.md). Each intermediate state is a [matching in a graph](../../../../../matching-graph-theory.md), and each entire transition [path in a graph](../../../../../path-in-a-graph.md) has length at most $4n$.

Fix a directed transition with initial state $M$. The complementary edge set $K=I\triangle F\triangle M$ agrees with one of the two [matchings in a graph](../../../../../matching-graph-theory.md) outside the active component and has at most two degree-two [vertices](../../../../../vertex-graph-theory.md) on that component. Remove at most two offending [edges](../../../../../edge-of-a-graph.md) to obtain a [matching in a graph](../../../../../matching-graph-theory.md) $K'$. Store those [edges](../../../../../edge-of-a-graph.md) and one bit specifying the initial alternating colour of the active component. This encoding is injective for the fixed transition: it restores $K$ and $I\triangle F=M\triangle K$, identifies the active component from the changed [edges](../../../../../edge-of-a-graph.md), and recovers the two colours using the fixed component order. Completed components have $F$'s colour in $M$, pending components have $I$'s colour, and the stored bit resolves the active component. Common [edges](../../../../../edge-of-a-graph.md) are $M\cap K$.

There are at most $2(m+1)^2$ auxiliary records per $K'$, where $m$ is the number of [graph](../../../../../graph-split.md) [edges](../../../../../edge-of-a-graph.md). If $d=|K|-|K'|\leq2$, then

$$
\pi_\lambda(I)\pi_\lambda(F)=\lambda^d\pi_\lambda(M)\pi_\lambda(K').
$$

Also $Q(M,M')\geq\pi_\lambda(M)/(2m\max(\lambda,\lambda^{-1}))$. Sum over the encodings and use the [path](../../../../../continuous-path.md) length bound to obtain

$$
\rho\leq16nm(m+1)^2\max(1,\lambda^2)\max(\lambda,\lambda^{-1}).
$$

This is polynomial whenever $\lambda$ and $\lambda^{-1}$ are polynomially bounded. Starting at the empty [matching in a graph](../../../../../matching-graph-theory.md), $\log(1/\pi_\lambda(\varnothing))=\log Z(\lambda)\leq m\log(1+\lambda)$, so the [Discrete Poincare inequality](../../../../../poincare-inequality-for-a-reversible-markov-chain.md) gives polynomial-time sampling to any prescribed [total variation distance](../../../../../total-variation-distance.md). The addition/deletion/exchange construction is also described in [Section 12.4 of Jerrum and Sinclair's survey](https://people.eecs.berkeley.edu/~sinclair/mcmc.pdf).

It remains to turn sampling into a relative count; merely sampling [perfect matchings](../../../../../perfect-matching.md) would not do that. For $0<\varepsilon\leq1/2$, choose $\lambda_0=\varepsilon/(8m)$ and $\lambda_*=8C_0/\varepsilon$. The elementary bounds above give

$$
1\leq Z(\lambda_0)\leq(1+\lambda_0)^m\leq1+\varepsilon/4,
\qquad
1\leq\frac{Z(\lambda_*)}{m_n\lambda_*^n}
\leq\sum_{j=0}^n(C_0/\lambda_*)^j\leq1+\varepsilon/4.
$$

Choose a schedule $\lambda_0<\lambda_1<\cdots<\lambda_J=\lambda_*$ whose successive ratios are at most $1+1/n$. It has $J=O(n\log(n/\varepsilon))$ stages. The [annealing ratios for a matching generating function](../../../../../annealing-ratios-for-a-matching-generating-function.md) satisfy

$$
\frac{Z(\lambda_{j+1})}{Z(\lambda_j)}
=\mathbb E_{\pi_{\lambda_j}}\left(\frac{\lambda_{j+1}}{\lambda_j}\right)^{|M|}.
$$

Each observable lies in $[1,e]$, so the [Hoeffding inequality](../../../../../hoeffding-inequality.md) gives relative accuracy $\eta=\varepsilon/(10J)$ with $O(\eta^{-2}\log(J/\delta))$ independent samples per stage. Run independent copies of the chain from the empty [matching in a graph](../../../../../matching-graph-theory.md); make the [total variation distance](../../../../../total-variation-distance.md) per sample at most $\delta/(3JK)$, where $K$ is that sample count. The [coupling characterization of total variation distance](../../../../../coupling-characterization-of-total-variation-distance.md) and the [union bound](../../../../../boole-s-inequality.md) make the entire sample collection coincide with exact stationary samples except with probability at most $\delta/3$. Choose the sample-count constant so all stationary sample means are accurate except with probability at most $\delta/3$.

Let $\widehat R$ be the product of the sample means, and output $\widehat p=\widehat R/\lambda_*^n$. On the successful event its multiplicative error relative to $Z(\lambda_*)/Z(\lambda_0)$ lies between $e^{-\varepsilon/5}$ and $e^{\varepsilon/5}$. Combining the two endpoint bounds proves

$$
\boxed{\mathbb P\bigl((1-\varepsilon)\operatorname{per}A\leq\widehat p\leq(1+\varepsilon)\operatorname{per}A\bigr)\geq1-\delta.}
$$

Activities, sample counts, simulation lengths and rational bit lengths are polynomial in $n,\varepsilon^{-1},\log(\delta^{-1})$. Thus this is a [fully polynomial randomized approximation scheme](../../../../../fully-polynomial-randomized-approximation-scheme.md). Small dimensions can be evaluated directly.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
