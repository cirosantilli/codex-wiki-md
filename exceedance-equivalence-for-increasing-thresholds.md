# Exceedance equivalence for increasing thresholds

↑ **Parent:** [Limsup of events](limsup-of-events.md)

Let $(a_n)$ be a nondecreasing real [sequence](sequence.md) tending to $+\infty$, and let $(x_n)$ be any real [sequence](sequence.md). The running maximum exceeds $a_n$ infinitely often exactly when $x_n>a_n$ infinitely often. Applying this pathwise to [random variables](random-variable-split.md) gives the displayed [event](event.md) equality, without any [independence](independent-random-variables.md) assumption.

One implication follows from $x_n\leq\max_{k\leq n}x_k$. For the other, if $x_n\leq a_n$ from some $N$ onwards, every later value with $N\leq k\leq n$ satisfies $x_k\leq a_k\leq a_n$. The finite prefix also lies below $a_n$ for all sufficiently large $n$, because $a_n\to\infty$. Therefore the entire running maximum eventually stays below the threshold.

Divergence of the thresholds prevents one large early observation from creating infinitely many crossings. Monotonicity ensures that a later running-maximum crossing is controlled by the corresponding earlier individual threshold. These two conditions explain why the resulting [event](event.md) belongs to the [tail sigma-algebra](tail-sigma-algebra.md) when the thresholds are deterministic.

## ↑ Ancestors (8)

1. [Limsup of events](limsup-of-events.md)
2. [Event](event.md)
3. [Probability space](probability-space-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/b/ii/solution.md)
