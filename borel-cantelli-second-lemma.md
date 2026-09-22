# Borel-Cantelli second lemma

↑ **Parent:** [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)

If the [events](event.md) $A_n$ are mutually [independent events](independent-events.md) and $\sum_{n=1}^{\infty}\mathbb P(A_n)=\infty$, then $\mathbb P(\limsup_n A_n)=1$. For an infinite family, mutual [independence](independent-random-variables.md) means every finite subfamily satisfies the factorization defining [independent events](independent-events.md).[§2.3, Theorem 2.3.7 and its proof, printed p. 70](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

Proof outline: for $M\geq m$, [independent events](independent-events.md) and $1-x\leq e^{-x}$ give

$$
\mathbb P\left(\bigcap_{n=m}^{M}A_n^c\right)
=\prod_{n=m}^{M}\left(1-\mathbb P(A_n)\right)
\leq\exp\left(-\sum_{n=m}^{M}\mathbb P(A_n)\right)\longrightarrow0.
$$

[Continuity of probability](continuity-of-probability.md) makes each infinite tail [union](set-union.md) have [probability](probability.md) one; their countable [intersection](set-intersection.md) has [probability](probability.md) one as well.

**Table of contents**

- [Shared-uniform counterexample to the second Borel-Cantelli lemma](shared-uniform-counterexample-to-the-second-borel-cantelli-lemma.md)

## ↑ Ancestors (6)

1. [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md)
