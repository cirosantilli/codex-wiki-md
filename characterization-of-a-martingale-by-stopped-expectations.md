# Characterization of a martingale by stopped expectations

↑ **Parent:** [Stopped martingale in discrete time](stopped-martingale-in-discrete-time.md)

Let an integrable process $(M_n)$ be [adapted](adapted-process.md) to $(\mathcal F_n)$. It is a [martingale](martingale-split.md) if and only if $\mathbb E[M_{n\wedge\tau}]=\mathbb E[M_0]$ for every $n$ and every [stopping time](stopping-time.md) $\tau$. For the reverse implication, fix $A\in\mathcal F_n$ and take $\tau=n$ on $A$ and $\tau=n+1$ on $A^c$. Comparing its stopped expectation at $n+1$ with the expectation obtained from the deterministic stopping time $n+1$ gives $\mathbb E[\mathbf1_A(M_{n+1}-M_n)]=0$. Since this holds for every $A\in\mathcal F_n$, it is exactly $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$.

## ↑ Ancestors (8)

1. [Stopped martingale in discrete time](stopped-martingale-in-discrete-time.md)
2. [Stopping time](stopping-time.md)
3. [Martingale](martingale-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/30k/c/iii/solution.md)
