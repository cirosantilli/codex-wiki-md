# Asymptotic normality of a weighted regression slope

↑ **Parent:** [Linear regression](linear-regression-split.md)

Suppose $\epsilon_1,\epsilon_2,\ldots$ are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) with [mean](expected-value-split.md) zero and finite [variance](variance-split.md) $\sigma^2>0$. For deterministic weights $x_{n,i}$, put $S_n=\sum_{i=1}^n x_{n,i}^2>0$. If

$$
\frac{\max_i x_{n,i}^2}{S_n}\longrightarrow0,
$$

then the [Lindeberg-Feller central limit theorem](lindeberg-feller-central-limit-theorem.md) gives

$$
\frac{\sum_i x_{n,i}\epsilon_i}{\sigma\sqrt{S_n}}\xrightarrow d N(0,1).
$$

This is the condition that no observation dominates the weighted error sum. In a centered [linear regression](linear-regression-split.md) with [orthogonal](orthogonal-vectors.md) explanatory columns, $\widehat\beta_1-\beta_1=\sum_i x_{n,i}\epsilon_i/S_n$, so the result justifies a [normal approximation](normal-approximation.md) with [variance](variance-split.md) $\sigma^2/S_n$.

To verify the [Lindeberg condition](lindeberg-condition.md), write $a_{n,i}=x_{n,i}/\sqrt{S_n}$ and $\delta_n=\max_i|a_{n,i}|\to0$. For each $\eta>0$,

$$
\sum_i\mathbb E\left[\left(\frac{a_{n,i}\epsilon_i}{\sigma}\right)^2\mathbf1_{\{|a_{n,i}\epsilon_i|>\eta\sigma\}}\right]
\le\frac1{\sigma^2}\mathbb E\left[\epsilon_1^2\mathbf1_{\{|\epsilon_1|>\eta\sigma/\delta_n\}}\right]\longrightarrow0.
$$

The inequality uses $\sum_i a_{n,i}^2=1$, and the limit follows from the finite second moment. Without the maximum-weight condition, adding observations with zero explanatory value can leave the slope determined by a fixed number of nonnormal errors for every sample size.

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iii/8/b/iii/solution.md)
