# Tail measurability of limits of sample averages

↑ **Parent:** [Tail sigma-algebra](tail-sigma-algebra.md)

Let $(X_j)$ be a [sequence](sequence.md) of finite real [random variables](random-variable-split.md), and write $M_n=n^{-1}\sum_{j=1}^nX_j$ for its [sample mean](sample-mean.md). For fixed $m$ and $n>m$, put $M_n^{(m)}=n^{-1}\sum_{j=m+1}^nX_j$. Then, at each outcome,

$$
M_n-M_n^{(m)}=\frac{X_1+\cdots+X_m}{n}\longrightarrow0.
$$

Consequently $\limsup_n M_n=\limsup_n M_n^{(m)}$. The right-hand [limit superior](limit-superior.md) is a [measurable function](measurable-function.md) of $X_{m+1},X_{m+2},\ldots$ for every $m$, so the extended-real [random variable](random-variable-split.md) $\limsup_n M_n$ is measurable with respect to the [tail sigma-algebra](tail-sigma-algebra.md). The same holds for the [limit inferior](limit-inferior.md). Thus the [event](event.md) of convergence to a finite [limit of a sequence](limit-of-a-sequence.md), and the [event](event.md) $\{M_n\to a\}$ for any specified real $a$, are [tail events](tail-event.md).

For a worked deterministic example, let $x_j$ alternate $0,1,0,1,\ldots$, and replace its first three entries $0,1,0$ by $1,0,1$. For every $n\geq3$ the two [sample means](sample-mean.md) differ by exactly $1/n$, so both converge to $1/2$. Finite edits can change small-sample answers while preserving the infinite [limit of a sequence](limit-of-a-sequence.md).

Under [independence](independent-random-variables.md), [Kolmogorov's zero–one law](kolmogorov-s-zero-one-law.md) makes each specified convergence [event](event.md) have [probability](probability.md) zero or one. It does not select which value occurs. If a finite [random variable](random-variable-split.md) measurable with respect to the [tail sigma-algebra](tail-sigma-algebra.md) $L$ exists, the [events](event.md) $\{L\leq q\}$ for rational $q$ each have [probability](probability.md) zero or one; [continuity of probability](continuity-of-probability.md) and their nesting force $L$ to be constant [almost surely](almost-sure-convergence.md). For fair [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md), the [strong law of large numbers](strong-law-of-large-numbers.md) establishes $M_n\to1/2$ [almost surely](almost-sure-convergence.md); the zero–one conclusion alone proves neither convergence nor the value $1/2$.

## ↑ Ancestors (7)

1. [Tail sigma-algebra](tail-sigma-algebra.md)
2. [Independent sigma-algebras](independent-sigma-algebras.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/3/c/solution.md)
