# Fractional moment decay of independent mean-one products

↑ **Parent:** [Product martingale from independent mean-one factors](product-martingale-from-independent-mean-one-factors.md)

Suppose $(X_n)$ are identically distributed [independent random variables](independent-random-variables.md) with $X_n\geq0$, $\mathbb EX_n=1$, and $X_1$ not constant [almost surely](almost-sure-convergence.md). For each $0<r<1$, strict [concavity](concave-function.md) of $t^r$ gives

$$
0<q:=\mathbb E[X_1^r]<1.
$$

The [moment](moment.md) is finite because $t^r\leq1+t$ on $[0,\infty)$. Let $Y_n=\prod_{k=1}^nX_k$. [Independence](independent-random-variables.md) and [Markov's inequality](markov-s-inequality.md) give

$$
\mathbb E[Y_n^r]=q^n,\qquad
\mathbb P(Y_n>\varepsilon)\leq\varepsilon^{-r}q^n.
$$

The [series](series-mathematics.md) of the latter [probabilities](probability.md) is finite. The [First Borel-Cantelli lemma](borel-cantelli-first-lemma.md), applied for the countable choices $\varepsilon=1/m$, proves $Y_n\to0$ [almost surely](almost-sure-convergence.md). This proof requires neither existence nor [integrability](integrability.md) of $\log X_1$.

Although this nonnegative [martingale](martingale-split.md) has $\mathbb EY_n=1$ at every time, its terminal [expected value](expected-value-split.md) is zero. It is therefore not [uniformly integrable](uniform-integrability.md). The contrast is useful: bounded [expected values](expected-value-split.md) ensure [almost sure convergence](almost-sure-convergence.md) here, but do not allow preservation of the [expected value](expected-value-split.md) through the limit.

## ↑ Ancestors (7)

1. [Product martingale from independent mean-one factors](product-martingale-from-independent-mean-one-factors.md)
2. [Martingale](martingale-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/c/i/solution.md)
