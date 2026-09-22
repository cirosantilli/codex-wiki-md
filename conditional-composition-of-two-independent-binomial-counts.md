# Conditional composition of two independent binomial counts

↑ **Parent:** [Binomial distribution](binomial-distribution.md)

Let $X$ and $Y$ be [independent random variables](independent-random-variables.md) with [binomial distributions](binomial-distribution.md) $\operatorname{Bin}(n,p)$ and $\operatorname{Bin}(m,q)$. Conditional on $X+Y=k$ having positive [probability](probability.md), the possible values of $X$ satisfy $\max(0,k-m)\leq j\leq\min(n,k)$. Their probabilities are

$$
\mathbb P(X=j\mid X+Y=k)=\frac{w_j}{\sum_iw_i},
\quad w_j=\binom nj\binom m{k-j}p^j(1-p)^{n-j}q^{k-j}(1-q)^{m-k+j},
$$

where the denominator sums over that feasible integer range. The formula follows by multiplying independent [binomial probabilities](binomial-probability.md) and dividing by the [probability](probability.md) of the disjoint union of all feasible count pairs.

For $p,q\in(0,1)$, common factors cancel and the weights are proportional to $\binom nj\binom m{k-j}\theta^j$, where $\theta=p(1-q)/[q(1-p)]$. If $p=q$, this reduces to the [hypergeometric distribution](hypergeometric-distribution.md), with probabilities $\binom nj\binom m{k-j}/\binom{n+m}k$. At parameter endpoints, use the original probability weights and check that the conditioning event has positive [probability](probability.md) before dividing.

## ↑ Ancestors (8)

1. [Binomial distribution](binomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
