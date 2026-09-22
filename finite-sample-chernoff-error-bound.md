# Finite-sample Chernoff error bound

↑ **Parent:** [Chernoff information](chernoff-information.md)

For equal [prior probabilities](prior-probability.md) and [independent and identically distributed](independent-and-identically-distributed-random-variables.md) observations on a [finite alphabet](finite-alphabet.md), [minimum sum of errors in a simple hypothesis test](minimum-sum-of-errors-in-a-simple-hypothesis-test.md) gives

$$
p_n^*=\frac12\sum_{x_1,\ldots,x_n}\min\{P^{\otimes n}(x_1,\ldots,x_n),Q^{\otimes n}(x_1,\ldots,x_n)\}.
$$

For nonnegative $a,b$ and $0<s<1$, $\min(a,b)\leq a^sb^{1-s}$. Applying this termwise and using the [independence of random variables](independent-random-variables.md) to factor the sum yields

$$
p_n^*\leq\frac12\left(\sum_xP(x)^sQ(x)^{1-s}\right)^n.
$$

Optimizing $s$, with an [infimum](infimum.md) if needed, proves $p_n^*\leq\tfrac12e^{-nC(P,Q)}$. This short argument gives a bound for every $n$. The theorem identifying the optimal [error exponent](error-exponents-in-hypothesis-testing.md) also needs the converse: no decision rule can achieve a strictly larger limiting exponent. A [log-likelihood ratio](log-likelihood-ratio.md) is a sum of independent contributions, so [large deviation principle](large-deviation-principle.md) supplies the relevant converse idea.

## ↑ Ancestors (7)

1. [Chernoff information](chernoff-information.md)
2. [Binary hypothesis testing in information theory](binary-hypothesis-testing-in-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Chernoff information](chernoff-information.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
