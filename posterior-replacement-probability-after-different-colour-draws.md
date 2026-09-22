# Posterior replacement probability after different-colour draws

↑ **Parent:** [Bayes' theorem](bayes-theorem.md)

An urn has $N$ balls, including $K$ of one colour and $N-K$ of the other, with $0<K<N$. After a uniform first draw, an independent decision returns that ball with [probability](probability.md) $r$; the second draw is uniform from the remaining contents. Let $B_j$ mean the $j$th draw has the first colour and $R$ mean replacement. The two relevant joint [probabilities](probability.md) are

$$
P(\overline B_1\cap R\cap B_2)=\frac{N-K}{N}\,r\,\frac KN,\qquad
P(\overline B_1\cap\overline R\cap B_2)=\frac{N-K}{N}\,(1-r)\,\frac K{N-1}.
$$

Applying [Bayes' theorem](bayes-theorem.md) and cancelling the common factors gives the displayed [conditional probability](conditional-probability.md). It is independent of $K$ and satisfies

$$
r-P(R\mid\overline B_1\cap B_2)=\frac{r(1-r)}{N-r}\ge0.
$$

Two different observed colours therefore decrease the posterior [probability](probability.md) of replacement: removing the first colour makes the second more likely. The replacement decision must be independent of the first draw for this formula; its marginal [probability](probability.md) alone does not specify the model.

## ↑ Ancestors (7)

1. [Bayes' theorem](bayes-theorem.md)
2. [Conditional probability](conditional-probability.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/16/d/solution.md)
