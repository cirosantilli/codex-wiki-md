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

## ← Incoming links (8)

- [Divergence of normalized iid partial sums without a first absolute moment](divergence-of-normalized-iid-partial-sums-without-a-first-absolute-moment.md)
- [Infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2010/a/2/b/ii/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2010/a/3/a/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2011/a/2/b/solution.md)
- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2011/a/2/c/iii/solution.md)
- [Positivity of the limiting Pólya urn proportion](positivity-of-the-limiting-polya-urn-proportion.md)
- [Rare-jump counterexample to a strong law with convergent first-moment averages](rare-jump-counterexample-to-a-strong-law-with-convergent-first-moment-averages.md)
