# Involutive Metropolis proposal

↑ **Parent:** [Proposal distribution](proposal-distribution.md)

An [involutive Metropolis proposal](involutive-metropolis-proposal.md) uses a deterministic bijection $S$ satisfying $S^2=I$. For a volume-preserving $S$ and target [probability density function](probability-density-function.md) $\rho$, accept $S(z)$ with probability $\min(1,\rho(S(z))/\rho(z))$. The identity $\rho(z)\alpha(z)=\min(\rho(z),\rho(S(z)))$ and a change of variables under $S$ prove [detailed balance](detailed-balance.md). A non-unit [Jacobian determinant](jacobian-determinant.md) must be included when volume is not preserved.

## ↑ Ancestors (9)

1. [Proposal distribution](proposal-distribution.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Involutive Metropolis proposal](involutive-metropolis-proposal.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/6/solution.md)
- [Surrogate Hamiltonian Monte Carlo](surrogate-hamiltonian-monte-carlo.md)
