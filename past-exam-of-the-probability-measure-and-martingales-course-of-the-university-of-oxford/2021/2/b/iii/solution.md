<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [tail sigma-algebra](../../../../../tail-sigma-algebra.md) of this [sequence](../../../../../sequence.md) is

$$
\mathcal T=\bigcap_{r\geq1}\sigma(X_r,X_{r+1},\ldots).
$$

For each fixed $r$, the preceding [event](../../../../../event.md) equality gives

$$
A=\bigcap_{N\geq r}\bigcup_{n\geq N}\{X_n>a_n\}.
$$

Every [event](../../../../../event.md) on the right is determined by coordinates with index at least $r$. Therefore $A\in\sigma(X_r,X_{r+1},\ldots)$ for every $r$, and $A\in\mathcal T$. The [random variables](../../../../../random-variable-split.md) $X_n$ are [independent](../../../../../independent-random-variables.md), so [Kolmogorov's zero–one law](../../../../../kolmogorov-s-zero-one-law.md) applies: every [tail event](../../../../../tail-event.md) has [probability](../../../../../probability.md) zero or one. Hence **$\mathbb P(A)\in\{0,1\}$**.

The role of [independence](../../../../../independent-random-variables.md) can also be seen directly. A [tail event](../../../../../tail-event.md) is independent of each finite initial [sigma-algebra](../../../../../sigma-algebra.md) $\sigma(X_1,\ldots,X_m)$. The [Monotone class theorem](../../../../../monotone-class-theorem.md) extends this [independence](../../../../../independent-random-variables.md) to $\sigma(X_1,X_2,\ldots)$; since $A$ itself lies there, it is independent of itself. Thus $\mathbb P(A)=\mathbb P(A)^2$.[§2.5, Theorem 2.5.3, printed pp. 81–82: the tail sigma-field zero–one law](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
