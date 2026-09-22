<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The command uses the model without covariates, starts in mild fatigue at time zero, and calculates expected accumulated years in each state between times $0$ and $10$. Let $Z(t)$ be the fatigue state and $Q$ its fitted [generator matrix](../../../../../../generator-matrix.md). For the [occupation time of a continuous-time Markov chain](../../../../../../occupation-time-of-a-continuous-time-markov-chain.md),

$$
O_j(10)=\int_0^{10}\mathbf1_{\{Z(t)=j\}}\,dt,
$$

the [expected finite-horizon occupation time](../../../../../../expected-finite-horizon-occupation-time.md) is

$$
\mathbb E[O_j(10)\mid Z(0)=1]
=\int_0^{10}\Pr\{Z(t)=j\mid Z(0)=1\}\,dt
=\int_0^{10}(e^{tQ})_{1j}\,dt.
$$

The first equality follows by interchanging a bounded time integral and [expected value](../../../../../../expected-value.md), and the second uses the homogeneous [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) [transition matrix](../../../../../../stochastic-matrix.md). The reported expectations are **7.014800 years mild, 1.724686 years moderate, and 1.260514 years severe**. They sum to ten because the person occupies exactly one state at every time. All repeated entries are counted: these are not the lengths of single [holding times](../../../../../../holding-time.md), the durations until first reaching each state, or the probabilities of occupying the states at year ten. The interpretation of the time limits is also given in [the package documentation](https://chjackson.github.io/msm/reference/totlos.msm.html).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
