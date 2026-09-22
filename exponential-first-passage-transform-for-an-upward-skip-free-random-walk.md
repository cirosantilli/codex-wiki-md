# Exponential first-passage transform for an upward skip-free random walk

↑ **Parent:** [Exponential martingale of a random walk](exponential-martingale-of-a-random-walk.md)

Let $S_n$ have integrable, mean-zero [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) as increments, taking integer values at most one, with $\mathbb P(X_1=1)>0$. For a positive integer $b$, put $T_b=\inf\{n:S_n=b\}$ and $M(\tau)=\mathbb E e^{\tau X_1}$, $\tau>0$. Then $T_b$ is finite [almost surely](almost-sure-convergence.md). Indeed, $b-S_{n\wedge T_b}$ is a nonnegative [martingale](martingale-split.md); finite convergence on $\{T_b=\infty\}$ would force its integer increments eventually to vanish, contrary to the [Borel-Cantelli lemmas](borel-cantelli-lemmas.md) applied to $\{X_n=1\}$.

The [exponential martingale of a random walk](exponential-martingale-of-a-random-walk.md) $e^{\tau S_n}/M(\tau)^n$ stopped at $T_b$ is bounded by $e^{\tau b}$ because $S_{n\wedge T_b}\leq b$ and $M(\tau)\geq1$. The [dominated convergence theorem](dominated-convergence-theorem.md) therefore preserves its mean one at the limit and proves the displayed [first-passage time](first-passage-time.md) transform. This argument accommodates arbitrarily large negative jumps; the restriction concerns upward jumps. For a [simple symmetric random walk](simple-symmetric-random-walk.md), $M(\tau)=\cosh\tau$, giving $\mathbb E e^{-\alpha T_b}=(e^\alpha-\sqrt{e^{2\alpha}-1})^b$.

## ↑ Ancestors (9)

1. [Exponential martingale of a random walk](exponential-martingale-of-a-random-walk.md)
2. [Random walk](random-walk.md)
3. [Markov chain](markov-chain.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34/4/d/solution.md)
