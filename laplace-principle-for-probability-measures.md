# Laplace principle for probability measures

↑ **Parent:** [Laplace principle (large deviations theory)](laplace-principle-large-deviations-theory.md)

A family satisfies this principle with speed $a_n\to\infty$ and [rate function](rate-function.md) $I$ when the displayed variational identity holds for every bounded [continuous](continuous-function.md) real function $f$. A [large deviation principle](large-deviation-principle.md) implies it by the [Varadhan lemma](varadhan-s-lemma.md). The lower bound restricts the [expectation](expected-value.md) to a neighborhood of a chosen point; the upper bound partitions the bounded range of $f$ into small intervals and applies the closed-set probability bounds.

For nonnegative $X_n$, the identity also gives

$$
-\lim_n a_n^{-1}\log\mathbb E e^{-\mu a_nX_n}
=\inf_{s\geq0}[I(s)+\mu s],\qquad \mu\geq0.
$$

For $\mu>0$, truncate $f(s)=-\mu s$ below at $-\mu R$. The resulting bounded-function identity applies, while the difference of the two exponential [expectations](expected-value.md) is at most $e^{-\mu Ra_n}$. Choosing $R$ sufficiently large makes this error negligible on the claimed exponential scale. The case $\mu=0$ is immediate. This extension identifies moment-decay rates of a [passive scalar](passive-scalar.md) from fluctuations of its logarithmic stretching.

## ↑ Ancestors (8)

1. [Laplace principle (large deviations theory)](laplace-principle-large-deviations-theory.md)
2. [Large deviation principle](large-deviation-principle.md)
3. [Convergence of random variables](convergence-of-random-variables-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Laplace principle (large deviations theory)](laplace-principle-large-deviations-theory.md)
- [Large-deviation decay rates of a Gaussian scalar packet](large-deviation-decay-rates-of-a-gaussian-scalar-packet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51/3/solution.md)
