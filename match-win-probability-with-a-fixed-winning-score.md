# Match win probability with a fixed winning score

↑ **Parent:** [Negative binomial stopping argument](negative-binomial-stopping-argument.md)

Suppose independent [Bernoulli trials](bernoulli-trial.md) give a player a win with [probability](probability.md) $p$, and the match ends when either player reaches $r$ wins. The player's match-win probability is

$$
\sum_{n=0}^{r-1}\binom{r+n-1}{r-1}p^r(1-p)^n.
$$

For a win with $n$ losses, the final trial must be a win. The preceding $r+n-1$ trials contain exactly $r-1$ wins and $n$ losses; the [binomial coefficient](binomial-coefficient-split.md) counts their arrangements. Because $n<r$, the opponent cannot already have won, and because the player has only $r-1$ previous wins, the match has not ended earlier. Summing the disjoint terminal events gives the formula, a truncated [negative binomial distribution](negative-binomial-distribution.md) sum. The constant game-win probability must describe independent games, or equivalently remain the same conditional on every previous history.

## ↑ Ancestors (9)

1. [Negative binomial stopping argument](negative-binomial-stopping-argument.md)
2. [Negative binomial distribution](negative-binomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/11/c/solution.md)
