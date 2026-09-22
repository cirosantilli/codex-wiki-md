# Limsup of events

↑ **Parent:** [Event](event.md)

For [events](event.md) $A_n$ in a [probability space](probability-space.md), the infinitely-often [event](event.md) is

$$
\limsup_{n\to\infty}A_n
=\bigcap_{m=1}^{\infty}\bigcup_{n=m}^{\infty}A_n
=\{\omega:\text{for every }m\text{ there is }n\geq m\text{ with }\omega\in A_n\}.
$$

Its [complement of an event](complement-of-an-event.md) is $\bigcup_{m\geq1}\bigcap_{n\geq m}A_n^c$: after some outcome-dependent index, no more [events](event.md) occur.[§2.3 opening definition and infinitely-often notation, printed pp. 67–68](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

Deleting finitely many [events](event.md) leaves the [limsup of events](limsup-of-events.md) unchanged. It is therefore a [tail event](tail-event.md) of the sequence of [indicator random variables](indicator-random-variable.md) $\mathbf1_{A_n}$, whether or not those [random variables](random-variable-split.md) are [independent](independent-random-variables.md). For [independent events](independent-events.md), the [Kolmogorov zero-one law](kolmogorov-s-zero-one-law.md) restricts its [probability](probability.md) to zero or one; the [Borel-Cantelli lemmas](borel-cantelli-lemmas.md) determine which alternative holds from the [series](series-mathematics.md) of [probabilities](probability.md). Also $\mathbf1_{A_n}\to0$ precisely when only finitely many [events](event.md) occur, connecting the [First Borel-Cantelli lemma](borel-cantelli-first-lemma.md) to [almost sure convergence](almost-sure-convergence.md) and the existing [complete convergence](complete-convergence-of-random-variables.md) criterion.

## ↑ Ancestors (7)

1. [Event](event.md)
2. [Probability space](probability-space.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)
- [Limsup of events](limsup-of-events.md)
- [Shared-uniform counterexample to the second Borel-Cantelli lemma](shared-uniform-counterexample-to-the-second-borel-cantelli-lemma.md)
- [Summable and harmonic event probabilities](summable-and-harmonic-event-probabilities.md)
