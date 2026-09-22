<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The event (m=N) represents no change within the observed sequence:** every observation belongs to the first-rate segment, and the second-rate segment is empty. It is not the event $\lambda=\phi$; under continuous independent rate priors that exact equality has posterior probability zero. The endpoint is instead a distinct index value with positive prior mass.

For retained [Markov chain Monte Carlo](../../../../../../../markov-chain-monte-carlo.md) draws $(\lambda^{(b)},\phi^{(b)},m^{(b)})$, the direct estimate is

$$
\boxed{\widehat P(m=N\mid x)=\frac1B\sum_{b=1}^B\mathbf1_{\{m^{(b)}=N\}}.}
$$

Its consistency follows from the [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md). The draws are correlated, so an independent-binomial standard error would generally be incorrect; uncertainty should account for the [Markov chain Monte Carlo asymptotic variance](../../../../../../../markov-chain-monte-carlo-asymptotic-variance.md).

A [conditional Monte Carlo](../../../../../../../conditional-monte-carlo.md) alternative averages the conditional probability from the preceding solution:

$$
\frac1B\sum_{b=1}^B P(m=N\mid\lambda^{(b)},\phi^{(b)},x).
$$

The [tower property of conditional expectation](../../../../../../../law-of-total-expectation.md) shows that its posterior expectation is the same target. This replaces an indicator by its conditional expectation; for correlated chains one should assess efficiency rather than automatically assume its entire asymptotic variance is smaller.

An exact finite-sum check is available by integrating out both rates. The [marginal posterior weights of a Poisson count change point](../../../../../../../marginal-posterior-weights-of-a-poisson-count-change-point.md) are

$$
w_j=\frac{\Gamma(\alpha+S_j)\Gamma(\gamma+S-S_j)}{(\beta+j)^{\alpha+S_j}(\delta+N-j)^{\gamma+S-S_j}},\qquad\boxed{P(m=N\mid x)=\frac{w_N}{\sum_{j=1}^Nw_j}.}
$$

These follow from the [Gamma function](../../../../../../../gamma-function.md) integral $\int_0^\infty z^{a-1}e^{-bz}dz=\Gamma(a)/b^a$. All omitted prior-normalization and factorial factors are independent of $j$, so they cancel from this ratio. This exact calculation provides a useful independent check on either simulation estimate.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
