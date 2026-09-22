# Centered polynomial birth move in reversible-jump sampling

↑ **Parent:** [Reversible-jump Markov chain Monte Carlo](reversible-jump-markov-chain-monte-carlo.md)

A [polynomial regression](polynomial-regression.md) birth move can introduce a coefficient $z$ while shifting the intercept by $-cz$, with $c$ the sample average of the new monomial. The fitted-value increment is $z(x^{k+1}-c)$, whose sample average vanishes. The [Jacobian determinant](jacobian-determinant.md) of the coefficient transformation is one. A [reversible-jump Markov chain Monte Carlo](reversible-jump-markov-chain-monte-carlo.md) acceptance ratio must still include the normalized dimension-dependent [prior distributions](prior-probability.md), the model-order [prior distribution](prior-probability.md), the birth/death selection probabilities and the proposal density for $z$.

## ↑ Ancestors (8)

1. [Reversible-jump Markov chain Monte Carlo](reversible-jump-markov-chain-monte-carlo.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/b/ii/solution.md)
