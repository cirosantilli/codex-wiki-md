# Expected occupation before interval exit for a simple symmetric random walk

↑ **Parent:** [Simple symmetric random walk](simple-symmetric-random-walk.md)

Let $a<i<b$ and $a<j<b$ be integers. A [simple symmetric random walk](simple-symmetric-random-walk.md) started at $i$ exits the integer interval at $\tau=\inf\{n\geq0:S_n\in\{a,b\}\}$. Its expected occupation of $j$ before exit, including its initial state, is

$$
G_{a,b}(i,j)
=\mathbb E_i\sum_{k=0}^{\tau-1}\mathbf1_{\{S_k=j\}}
=\frac{2((i\wedge j)-a)(b-(i\vee j))}{b-a}.
$$

A block of $b-a$ consecutive positive steps forces exit, so the [geometric tail bound from a uniform escape probability](geometric-tail-bound-from-a-uniform-escape-probability.md) proves $\tau<\infty$ [almost surely](almost-sure-convergence.md). [Optional stopping](optional-sampling-theorem-for-a-supermartingale.md) at the [bounded stopping time](bounded-stopping-time.md) $n\wedge\tau$, followed by the [bounded convergence theorem](bounded-convergence-theorem.md) for $S_{n\wedge\tau}\in[a,b]$, gives the [gambler's ruin](gambler-s-ruin.md) probabilities

$$
\mathbb P_i(S_\tau=a)=\frac{b-i}{b-a},\qquad
\mathbb P_i(S_\tau=b)=\frac{i-a}{b-a}.
$$

Translate the [absolute value martingale of a simple symmetric random walk](absolute-value-martingale-of-a-simple-symmetric-random-walk.md) from zero to $j$. Bounded-time [optional stopping](optional-sampling-theorem-for-a-supermartingale.md) yields

$$
\mathbb E_i\sum_{k<n\wedge\tau}\mathbf1_{\{S_k=j\}}
=\mathbb E_i|S_{n\wedge\tau}-j|-|i-j|.
$$

Use [monotone convergence](monotone-convergence-theorem.md) on the increasing visit count and the [bounded convergence theorem](bounded-convergence-theorem.md) on the right. Substituting the exit [probabilities](probability.md) gives

$$
G_{a,b}(i,j)
=\frac{(b-i)(j-a)+(i-a)(b-j)}{b-a}-|i-j|,
$$

which simplifies to the displayed expression by considering $i\leq j$ and $i\geq j$. In particular, $G_{a,b}(0,0)=-2ab/(b-a)$ when $a<0<b$.

The proof establishes finite [expected value](expected-value-split.md) of the visit count. Therefore each translated stopped absolute-value [martingale](martingale-split.md) is dominated in absolute value by a constant plus that total count, an [integrable random variable](integrable-random-variable.md); its family of values is [uniformly integrable](uniform-integrability.md). This supplies the limit justification without assuming [uniform integrability](uniform-integrability.md) in advance.

## ↑ Ancestors (11)

1. [Simple symmetric random walk](simple-symmetric-random-walk.md)
2. [Simple random walk](simple-random-walk.md)
3. [Random walk on a graph](random-walk-on-a-graph.md)
4. [Random walk](random-walk-split.md)
5. [Markov chain](markov-chain-split.md)
6. [Markov process](markov-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/3/b/iii/solution.md)
