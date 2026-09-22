<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

For the [simple random walk on the integer line](../../../../../simple-random-walk-on-the-integer-line.md), a return to the origin is possible only at an [even](../../../../../even-number.md) time. At time $2n$, exactly $n$ of the increments must be $+1$, so the return probability is

$$
p_{2n}=\frac1{2^{2n}}\binom{2n}{n}.
$$

The supplied factorial bounds, equivalently the order estimate in the [Stirling formula](../../../../../stirling-formula.md), give

$$
p_{2n}\asymp n^{-1/2}.
$$

Consequently $\sum_np_{2n}$ diverges. By the [recurrence criterion by return probabilities](../../../../../recurrence-criterion-by-return-probabilities.md), the origin is a [recurrent state](../../../../../recurrent-state.md); translation invariance then makes the whole walk recurrent.

For three [independent](../../../../../independent-random-variables.md) walks, the probability that all three are at the origin at time $2n$ is

$$
p_{2n}^3
=\left(\frac{\binom{2n}{n}}{4^n}\right)^3
\asymp n^{-3/2}.
$$

This [P-series](../../../../../p-series.md) is convergent, so the first of the [Borel-Cantelli lemmas](../../../../../borel-cantelli-lemmas.md) says that simultaneous returns occur only finitely often with probability one. Therefore the requested probability is

$$
\boxed{0}.
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
