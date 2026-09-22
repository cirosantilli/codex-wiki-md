<h1 id="kolmogorov-s-zero-one-law">Kolmogorov's zero–one law</h1>

↑ **Parent:** [Tail sigma-algebra](tail-sigma-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov's_zero–one_law)

For mutually [independent random variables](independent-random-variables.md), every [tail event](tail-event.md) has $\mathbb P(A)\in\{0,1\}$. Identical [probability distributions](probability-distribution-split.md) are unnecessary. The [tail sigma-algebra](tail-sigma-algebra.md) is trivial in [probability](probability.md): its [events](event.md) have [probability](probability.md) zero or one, though it can contain nonempty proper [sets](set-split.md).[Probability: Theory and Examples (fifth edition), §2.5, Theorem 2.5.3, printed pp. 81–82](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

For a proof, set $\mathcal F_m=\sigma(X_1,\ldots,X_m)$ and $\mathcal F_X=\sigma(X_1,X_2,\ldots)$. [Independence extended from generating pi-systems](independence-extended-from-generating-pi-systems.md) makes $\mathcal F_m$ independent of $\sigma(X_{m+1},X_{m+2},\ldots)$, hence of each [tail event](tail-event.md) $A$. The increasing [union](set-union.md) $\bigcup_m\mathcal F_m$ is a generating [pi-system](pi-system.md) for $\mathcal F_X$. For fixed $A$, the [events](event.md) $B$ satisfying $\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)$ form a [Dynkin system](dynkin-system.md). The [pi-lambda theorem](pi-lambda-theorem.md) extends this equality to all $B\in\mathcal F_X$. Taking $B=A$ gives

$$
\mathbb P(A)=\mathbb P(A\cap A)=\mathbb P(A)^2,
\qquad \mathbb P(A)(1-\mathbb P(A))=0.
$$

Thus $A$ is independent of itself, forcing the two stated values.[Probability: Theory and Examples (fifth edition), proof of Theorem 2.5.3, steps (a) and (b), printed pp. 81–82](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

The useful feature is the absence of intermediate [probabilities](probability.md) for infinite properties that ignore every finite prefix. It reduces some calculations to showing that a [tail event](tail-event.md) has positive [probability](probability.md), or that its [complement](complement-of-a-set.md) does. The theorem supplies no finite observation deadline, and an extra argument such as the calculation in [infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md) is needed to decide which value occurs.

**Table of contents**

- [A shared coin prevents a zero-one conclusion](a-shared-coin-prevents-a-zero-one-conclusion.md)

## ↑ Ancestors (7)

1. [Tail sigma-algebra](tail-sigma-algebra.md)
2. [Independent sigma-algebras](independent-sigma-algebras.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/25j/b/solution.md)
- [Tail measurability of limits of sample averages](tail-measurability-of-limits-of-sample-averages.md)
- [Tail sigma-algebra](tail-sigma-algebra.md)
