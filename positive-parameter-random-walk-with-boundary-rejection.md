# Positive-parameter random walk with boundary rejection

↑ **Parent:** [Random-walk Metropolis algorithm](random-walk-metropolis-algorithm.md)

To update a positive parameter, a symmetric additive [proposal distribution](proposal-distribution.md) can be generated on the whole real line. Reject nonpositive proposals; accept positive ones using the target density ratio. The off-diagonal proposal remains symmetric. Repeatedly redrawing until the proposal is positive instead truncates and renormalizes the proposal differently at different current states, so a Hastings correction is then required. A symmetric walk in $\log v$ is another valid method, but its transformed target includes the [Jacobian determinant](jacobian-determinant.md) factor $v$.

## ↑ Ancestors (9)

1. [Random-walk Metropolis algorithm](random-walk-metropolis-algorithm.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/a/iii/solution.md)
