# Barker acceptance probability

↑ **Parent:** [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)

The [Barker acceptance probability](barker-acceptance-probability.md) accepts a proposal using the displayed ratio. If $a=\pi(x)q(x,y)$ and $b=\pi(y)q(y,x)$, the accepted flux is $ab/(a+b)$, symmetric in the two states. This proves [detailed balance](detailed-balance.md); define acceptance as zero when $a=b=0$. Rejected proposals contribute to the diagonal [transition probability](transition-probability.md). Replacing $\pi$ by an unnormalized target leaves the ratio unchanged. For a common proposal, $t/(1+t)\leq\min(1,t)$ shows that its acceptance [probability](probability.md) never exceeds the [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md). The name refers to [A. A. Barker](a-a-barker.md)'s work on [Monte Carlo methods](monte-carlo-method-split.md) for a plasma; the initials are retained without an unverified expansion.[Australian Journal of Physics 18, 119–134 (1965), bibliographic provenance](monte-carlo-calculations-of-the-radial-distribution-functions-for-a-proton-electron-plasma-by-a-a-barker.md)

## ↑ Ancestors (8)

1. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Barker acceptance probability](barker-acceptance-probability.md)
- [Monte Carlo Calculations of the Radial Distribution Functions for a Proton-Electron Plasma by A. A. Barker](monte-carlo-calculations-of-the-radial-distribution-functions-for-a-proton-electron-plasma-by-a-a-barker.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/1/d/solution.md)
