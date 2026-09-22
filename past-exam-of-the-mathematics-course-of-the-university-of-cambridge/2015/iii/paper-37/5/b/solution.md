<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A convenient general-state-space ergodic theorem is the following. For a [positive Harris recurrent Markov chain](../../../../../../positive-harris-recurrent-markov-chain.md) with invariant [probability measure](../../../../../../probability-measure.md) $\pi$, and a measurable function $h$ with $\pi|h|<\infty$,

$$
\boxed{\frac1n\sum_{t=1}^nh(X_t)\longrightarrow\pi h\quad\text{almost surely}.}
$$

Here $\pi h=\int h\,d\pi$ is the stationary [expected value](../../../../../../expected-value.md). [Harris recurrence](../../../../../../harris-recurrent-markov-chain.md) means that every set of positive irreducibility measure is visited almost surely from every state; positive recurrence supplies an invariant probability rather than only an infinite invariant measure. The [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md) holds from any starting state under these Harris hypotheses. [aperiodicity](../../../../../../aperiodic-markov-chain.md) is not necessary just for averages.

A useful sufficient form of the [central limit theorem for a geometrically ergodic Markov chain](../../../../../../central-limit-theorem-for-a-geometrically-ergodic-markov-chain.md) adds [aperiodicity](../../../../../../aperiodic-markov-chain.md), [geometric ergodicity](../../../../../../geometric-ergodicity.md), and $\pi(|h|^{2+\delta})<\infty$ for some $\delta>0$. It gives

$$
\boxed{\sqrt n\left(\frac1n\sum_{t=1}^nh(X_t)-\pi h\right)\Rightarrow N(0,v_h),\qquad
v_h=\gamma_h(0)+2\sum_{k=1}^\infty\gamma_h(k).}
$$

These are sufficient hypotheses, not a claim that irreducibility alone ensures a [central limit theorem](../../../../../../central-limit-theorem.md). The [Markov chain Monte Carlo asymptotic variance](../../../../../../markov-chain-monte-carlo-asymptotic-variance.md) uses stationary covariances $\gamma_h(k)=\operatorname{Cov}_\pi(h(X_0),h(X_k))$, with $\gamma_h(0)=\operatorname{Var}_\pi h$. The series is absolutely convergent under the stated sufficient assumptions. If $\gamma_h(0)>0$, write $\rho_h(k)=\gamma_h(k)/\gamma_h(0)$ and $v_h=\gamma_h(0)\tau_{\rm int}$, where the [integrated autocorrelation time](../../../../../../integrated-autocorrelation-time.md) is $\tau_{\rm int}=1+2\sum_{k\geq1}\rho_h(k)$. When $v_h>0$, the [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md) is approximately $n/\tau_{\rm int}$. Negative correlations can reduce the asymptotic [variance](../../../../../../variance-split.md); a zero asymptotic [variance](../../../../../../variance-split.md) gives a degenerate normal limit. For constant $h$, [variance](../../../../../../variance-split.md) is zero and the autocorrelation normalization is undefined.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
