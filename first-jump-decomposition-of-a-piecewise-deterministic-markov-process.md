# First-jump decomposition of a piecewise-deterministic Markov process

↑ **Parent:** [Piecewise-deterministic Markov process](piecewise-deterministic-markov-process.md)

For a [piecewise-deterministic Markov process](piecewise-deterministic-markov-process.md), conditional on no jump before $u$, the state is $z(u)=\varphi(s,x,u)$ and the [survival probability](survival-probability.md) is $S(u)=\exp[-\int_s^u\alpha(z(r))dr]$. The first jump has [probability density function](probability-density-function.md) $\alpha(z(u))S(u)$; conditioning on its time and its destination gives $P_{s,t}f(x)=S(t)f(z(t))+\int_s^t\alpha(z(u))S(u)\int P_{u,t}f(y)K_u(z(u),dy)du$. This proves the identity for bounded [Borel measurable functions](borel-measurable-function.md) under [nonexplosion](nonexplosion-of-a-continuous-time-markov-chain.md).

## ↑ Ancestors (7)

1. [Piecewise-deterministic Markov process](piecewise-deterministic-markov-process.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford/2025/1/b/solution.md)
