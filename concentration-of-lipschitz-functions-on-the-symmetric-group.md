# Concentration of Lipschitz functions on the symmetric group

↑ **Parent:** [Concentration inequality](concentration-inequality.md)

Equip the [symmetric group](symmetric-group.md) $S_n$ with its uniform [probability measure](probability-measure.md) and unnormalized [Hamming distance](hamming-distance.md). If $f$ has [Lipschitz constant](lipschitz-constant.md) $K$, it obeys the displayed two-sided bound, and each one-sided tail has the same exponential without the factor two. Reveal a uniform [permutation](permutation.md) one image at a time. Two possible next images have completion sets paired by swapping those two values, changing exactly two coordinates. Thus the corresponding conditional means differ by at most $2K$. Each increment of the [Doob exposure martingale](doob-exposure-martingale.md) has conditional range length at most $2K$. Applying the conditional [Hoeffding lemma](hoeffding-lemma.md) gives $\mathbb E e^{\lambda(f-\mathbb Ef)}\leq e^{n\lambda^2K^2/2}$; optimizing the [exponential Markov bound](exponential-markov-bound.md) proves the bound. A mere absolute-increment bound of $2K$ gives a weaker constant, so using the range length matters.

## ↑ Ancestors (7)

1. [Concentration inequality](concentration-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/2/i/solution.md)
