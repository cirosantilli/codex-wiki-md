# Borel-Cantelli first lemma

↑ **Parent:** [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)

For arbitrary [events](event.md) $A_n$ in one [probability space](probability-space.md),

$$
\sum_{n=1}^{\infty}\mathbb P(A_n)<\infty
\quad\Longrightarrow\quad
\mathbb P\left(\limsup_{n\to\infty}A_n\right)=0.
$$

Equivalently, only finitely many [events](event.md) occur [almost surely](almost-sure-convergence.md); no [independence](independent-random-variables.md) is needed.[§2.3, Theorem 2.3.1, printed p. 68](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

Proof outline: put $B_m=\bigcup_{n\geq m}A_n$. The [union bound](boole-s-inequality.md) gives

$$
0\leq\mathbb P\left(\limsup_n A_n\right)
\leq\mathbb P(B_m)\leq\sum_{n=m}^{\infty}\mathbb P(A_n)\longrightarrow0.
$$

The tail of a convergent nonnegative [series](series-mathematics.md) tends to zero.

## ↑ Ancestors (6)

1. [Borel-Cantelli lemmas](borel-cantelli-lemmas.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Almost-everywhere convergence from weak-type domination](almost-everywhere-convergence-from-weak-type-domination.md)
- [Brownian exit-skeleton clock convergence](brownian-exit-skeleton-clock-convergence.md)
- [Brownian upper law of the iterated logarithm](brownian-upper-law-of-the-iterated-logarithm.md)
- [Continuity of probability](continuity-of-probability.md)
- [Cramér model prime-gap upper bound](cramer-model-prime-gap-upper-bound.md)
- [Integral lower envelope for the Brownian maximum](integral-lower-envelope-for-the-brownian-maximum.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-5/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-31/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/2/c/solution.md)
- [Upper law of the iterated logarithm](upper-law-of-the-iterated-logarithm.md)
