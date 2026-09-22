<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each $n$,

$$
\{\tau\leq n\}=\bigcup_{k=0}^n\{S_k\in\{a,b\}\}\in\mathcal F_n,
$$

since $S_k$ is [adapted](../../../../../adapted-process.md). This verifies directly that $\tau$ is a [stopping time](../../../../../stopping-time.md).

Set $d=b-a$. On $\{\tau>md\}$, the [random walk](../../../../../random-walk-split.md) is at some integer strictly between $a$ and $b$. If its next $d$ steps are all $+1$, it must hit $b$ within that block. These future steps are [independent](../../../../../independent-random-variables.md) of $\mathcal F_{md}$ and have [probability](../../../../../probability.md) $2^{-d}$ of being all $+1$. Hence

$$
\mathbb P(\tau>(m+1)d\mid\mathcal F_{md})
\leq(1-2^{-d})\mathbf1_{\{\tau>md\}}.
$$

The [law of total expectation](../../../../../law-of-total-expectation.md) and [mathematical induction](../../../../../mathematical-induction.md) give the [geometric tail bound from a uniform escape probability](../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md):

$$
\mathbb P(\tau>md)\leq(1-2^{-d})^m\longrightarrow0.
$$

Therefore **$\mathbb P(\tau<\infty)=1$**. In fact this also proves $\mathbb E\tau\leq d\,2^d<\infty$ by grouping the [tail-sum formula](../../../../../tail-sum-formula.md) into blocks of length $d$. No assertion of [independence](../../../../../independent-random-variables.md) between successive survival [events](../../../../../event.md) is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
