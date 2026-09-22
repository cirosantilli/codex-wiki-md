# Birth-death-immigration jump chain

↑ **Parent:** [Birth-death chain](birth-death-chain.md)

Here $0<p<1$, $\theta>0$, and the upward step is either a birth or immigration, the latter having [conditional probability](conditional-probability.md) $\theta/(k+\theta)$. At zero immigration occurs with [probability](probability.md) one. Put $q=1-p$, $a=\theta/p$ and $r=p/q$. The [stationary weights of a reflected birth-death chain](stationary-weights-of-a-reflected-birth-death-chain.md) are

$$
w_k=\frac{k+\theta}{\theta}\frac{\Gamma(k+a)}{\Gamma(a)k!}r^k.
$$

Their successive ratio tends to $r$, so they are summable for $p<1/2$. For $p\geq1/2$, $u_k>1/2>d_{k+1}$ makes the weights strictly increasing, ruling out a [stationary distribution](stationary-distribution.md). Thus [positive recurrence](positive-recurrent-markov-chain.md) holds exactly for $p<1/2$. In that case the [binomial series](binomial-series.md) gives $\sum_kw_k=2(1-r)^{-a-1}$, and

$$
\pi_k=\frac{(1-r)^{a+1}}{2\theta\Gamma(a)}\frac{(k+\theta)\Gamma(k+a)}{k!}r^k.
$$

Every step reverses parity and a two-step return has positive [probability](probability.md), so the [period of a state in a Markov chain](period-of-a-state-in-a-markov-chain.md) is two. Starting at zero, $\mathbb P(X_{2n}=0)\to2\pi_0=(1-r)^{a+1}$, whereas $\mathbb P(X_{2n+1}=0)=0$.

## ↑ Ancestors (8)

1. [Birth-death chain](birth-death-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Immigration fraction among upward steps](immigration-fraction-among-upward-steps.md)
- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2023/3/b/i/solution.md)
