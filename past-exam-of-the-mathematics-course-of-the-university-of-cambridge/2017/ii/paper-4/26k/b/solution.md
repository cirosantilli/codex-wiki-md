<h1 id="26k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [M-M-1 queue with Bernoulli feedback](../../../../../../m-m-1-queue-with-bernoulli-feedback.md), assume $0<\delta\leq1$. The number of service visits before departure is geometric on $1,2,\ldots$, with probabilities $\delta(1-\delta)^{j-1}$, independent of the independent exponential visit lengths. The transform of the total time actually being served is

$$
\sum_{j=1}^\infty\delta(1-\delta)^{j-1}\left(\frac\mu{\mu+s}\right)^j
=\frac{\delta\mu}{\delta\mu+s}.
$$

Thus

$$
\boxed{B_{\rm total}\sim\operatorname{Exp}(\delta\mu).}
$$

This excludes the waiting between visits. A feedback completion changes the customer's position but not the number in the system. By exponential [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md), the latter process has births of rate $\lambda$ and true deaths of rate $\delta\mu$ while nonempty; unsuccessful completions are self-events. It is therefore an M/M/1 number process with effective service rate $\delta\mu$, giving

$$
\boxed{\lambda<\delta\mu,\qquad\pi_j=\left(1-\frac\lambda{\delta\mu}\right)\left(\frac\lambda{\delta\mu}\right)^j.}
$$

For positive $\lambda$ equality is null recurrent, larger arrival rate is unstable, and $\delta=0$ admits no departure-based equilibrium.

To prove the output claim, state the relevant [time reversal of a continuous-time Markov chain](../../../../../../time-reversal-of-a-continuous-time-markov-chain.md) theorem: an equilibrium continuous-time chain satisfying [detailed balance](../../../../../../detailed-balance.md) has the same reversed path law. In this reversible [birth-death process](../../../../../../birth-death-process.md), final departures are precisely downward jumps; time reversal turns them into upward jumps. Upward jumps are supplied by a state-independent Poisson clock of rate $\lambda$, so their process is Poisson. Hence **the stationary final-departure process is Poisson of rate $\lambda$**. This is the output conclusion of [Burke theorem](../../../../../../burke-s-theorem.md) for the effective number process; it does not say the process of all service completions has that rate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
