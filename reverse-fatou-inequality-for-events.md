# Reverse Fatou inequality for events

↑ **Parent:** [Limsup of events](limsup-of-events.md)

For any [sequence](sequence.md) of [events](event.md), its [limsup of events](limsup-of-events.md) satisfies

$$
\mathbb P(\limsup_n A_n)\geq\limsup_n\mathbb P(A_n).
$$

Set $C_N=\bigcup_{n\geq N}A_n$. These are decreasing [events](event.md) with [intersection](set-intersection.md) $\limsup_n A_n$. [Continuity of probability](continuity-of-probability.md) from above gives

$$
\mathbb P(\limsup_n A_n)=\lim_N\mathbb P(C_N)
\geq\lim_N\sup_{n\geq N}\mathbb P(A_n).
$$

This is also the bounded-indicator form of the reversed [Fatou lemma](fatou-s-lemma.md). The inequality can be strict: independent fair-coin head [events](event.md) each have [probability](probability.md) $1/2$, while their [limsup of events](limsup-of-events.md) has [probability](probability.md) $1$ by the [Second Borel-Cantelli lemma](borel-cantelli-second-lemma.md).

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

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/b/i/solution.md)
