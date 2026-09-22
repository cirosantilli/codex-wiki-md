<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

After $\tau$, the token product remains zero, whereas the deterministic term $nN/3$ continues to increase. Combining this with the pre-elimination calculation in part (ii),

$$
\boxed{\mathbb E[M_{n+1}-M_n\mid\mathcal F_n]
=\frac N3\mathbf1_{\{\tau\leq n\}}.}
$$

The [stochastic process](../../../../../stochastic-process-split.md) is [adapted](../../../../../adapted-process.md) and [integrable](../../../../../integrability.md) at each fixed time, and the displayed [conditional expectation](../../../../../conditional-expectation.md) is nonnegative. Thus **$(M_n)$ is a submartingale**.

For $N>0$ it is neither a [martingale](../../../../../martingale-split.md) nor a [supermartingale](../../../../../supermartingale.md). If $a,b,c>0$, there is positive [probability](../../../../../probability.md) that the first player transfers a token to the second in each of the next $a$ rounds. Until the last such round all three remain active, so this [event](../../../../../event.md) has [probability](../../../../../probability.md) $6^{-a}>0$ and entails $\tau\leq a$. At time $n=a$ the displayed [conditional expectation](../../../../../conditional-expectation.md) is therefore strictly positive on an [event](../../../../../event.md) of positive [probability](../../../../../probability.md), ruling out both the zero drift required of a [martingale](../../../../../martingale-split.md) and the nonpositive drift required of a [supermartingale](../../../../../supermartingale.md). If an initial holding is zero, $\tau=0$ and the same conclusion follows immediately. The degenerate case $N=0$ gives a constant [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
