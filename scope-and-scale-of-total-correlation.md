# Scope and scale of total correlation

↑ **Parent:** [Total correlation](total-correlation.md)

For finite [alphabets](alphabet.md), $H(X_1,\ldots,X_n)\geq\max_iH(X_i)$, so

$$
0\leq\operatorname{TC}(X_1,\ldots,X_n)
\leq\sum_iH(X_i)-\max_iH(X_i).
$$

For $n$ identical copies of one fair [bit](bit.md), the upper bound is attained and [total correlation](total-correlation.md) is $n-1$ [bits](bit.md). Adding another copy increases the result without introducing a new underlying random choice. The choice of coordinates and their grouping therefore matters when comparing systems of different sizes.

For more general [random variables](random-variable-split.md), the [relative entropy](kullback-leibler-divergence.md) against the product of the marginals supplies a definition of [total correlation](total-correlation.md) that may be infinite. Subtracting [differential entropies](differential-entropy.md) is justified only when those quantities are finite and the entropy identity is valid; an undefined difference of infinities is not a definition. The finite-[alphabet](alphabet.md) examples above avoid that problem entirely.

## ↑ Ancestors (6)

1. [Total correlation](total-correlation.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
