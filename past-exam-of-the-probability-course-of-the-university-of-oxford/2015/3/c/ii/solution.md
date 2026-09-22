<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work on the single event of [probability](../../../../../probability.md) one where $Y_n/n\to\mu=2p-1>0$. On every [sample path](../../../../../sample-path.md) in that event, $Y_n\to+\infty$ and the unit-step property ensures that every positive [integer](../../../../../integer-split.md) $j$ is reached, so $T_j<\infty$. Starting from zero requires at least $j$ steps to reach $j$, hence $T_j\geq j$ and $T_j\to\infty$.

The convergent numerical sequence $Y_n/n$ on this fixed [sample path](../../../../../sample-path.md) also converges along its possibly random subsequence $n=T_j$. Since $Y_{T_j}=j$,

$$
\frac{j}{T_j}=\frac{Y_{T_j}}{T_j}\longrightarrow\mu.
$$

Taking the reciprocal is valid because $\mu>0$. We obtain

$$
\boxed{\mathbb P\!\left(\frac{T_j}{j}\longrightarrow\alpha\right)=1,
\qquad\alpha=\frac1{2p-1}.}
$$

This is a [first-passage law of large numbers for an upward skip-free random walk](../../../../../first-passage-law-of-large-numbers-for-an-upward-skip-free-random-walk.md). No independence between the [hitting times](../../../../../first-passage-time.md) and the path is needed: [almost sure convergence](../../../../../almost-sure-convergence.md) already supplies convergence along every diverging subsequence on the same event.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
