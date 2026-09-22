<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The restriction $Q_C$ is a [finite Markov chain](../../../../../finite-markov-chain.md) that is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md). It is [aperiodic](../../../../../aperiodic-markov-chain.md), because its upper states have self-transition [probability](../../../../../probability.md) $a/(a+b)>0$, and the [period is constant on a communicating class](../../../../../period-is-constant-on-a-communicating-class.md). We now find its [stationary distribution](../../../../../stationary-distribution.md).

Every column of $Q_C$ sums to one. Here is the full incoming-mass check, with each total measured in units of $1/(a+b)$. For $j\in L$, the incoming contributions are $a$ from $j+b\in I$ and $b$ from the self-transition. For $j\in U$, they are $b$ from $j-a\in I$ and $a$ from the self-transition.

For $j\in I$, the upward predecessor $j-a$ lies in $I$ exactly when $j\geq-c+a$, contributing $b$ units. When $j\leq-c+a-1$, that predecessor is replaced by resets from all $b$ states of $L$, again contributing $b$ units. Independently, the downward predecessor $j+b$ contributes $a$ units when $j\leq c-b$; when $j\geq c-b+1$, resets from the $a$ states of $U$ contribute those $a$ units instead. Thus every column total is $a+b$ units.

Therefore $Q_C$ is a [doubly stochastic matrix](../../../../../doubly-stochastic-matrix.md), and the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $C$ is stationary:

$$
\boxed{\pi_j=\begin{cases}\displaystyle\frac1{2c+a+b+1},&-c-b\leq j\leq c+a,\\0,&\text{otherwise}.\end{cases}}
$$

The [countable-state Markov chain convergence theorem](../../../../../countable-state-markov-chain-convergence-theorem.md), applied to the finite closed class $C$, gives $Q_C^n(i,j)\to\pi_j$ for every $i\in C$. Its hypotheses hold: $C$ is finite and irreducible, hence [positive recurrent](../../../../../positive-recurrent-markov-chain.md), and it is [aperiodic](../../../../../aperiodic-markov-chain.md).

If $i_0>c+a$, the [hitting time](../../../../../first-passage-time.md) $H$ of $C$ has $\mathbb P(H>n)=(a/(a+b))^n$. If $i_0<-c-b$, the corresponding tail is $(b/(a+b))^n$. Thus $H<\infty$ [almost surely](../../../../../almost-sure-convergence.md) from every exterior initial state. Conditioning on $H$ and $R_H$, use convergence within $C$ after entrance and the [bounded convergence theorem](../../../../../bounded-convergence-theorem.md); equivalently, first restrict to $H\leq K$ and then let $K\to\infty$. This proves, for every $i_0\in\mathbb Z$,

$$
\boxed{R_n\xrightarrow{\mathrm d}\operatorname{Unif}\{-c-b,\ldots,c+a\}.}
$$

The [limiting distribution](../../../../../limiting-distribution.md) is independent of $i_0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
