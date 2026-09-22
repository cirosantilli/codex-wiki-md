# Success-count and waiting-time duality

↑ **Parent:** [Negative binomial stopping argument](negative-binomial-stopping-argument.md)

The same stopping rule connects a waiting count to a fixed-length count. Let $N=X+r$ be the trial number of the $r$th success, and let $B_n$ count successes in the first $n$ trials, so $B_n$ has a [binomial distribution](binomial-distribution.md). For any nonnegative [integer](integer-split.md) $n$,

$$
\{N>n\}=\{B_n<r\},\qquad
\mathbb P(N>n)=\sum_{k=0}^{\min(r-1,n)}\binom nk p^k(1-p)^{n-k}.
$$

The target is still unmet after $n$ trials exactly when fewer than $r$ successes have occurred. With $r=2$, $p=1/2$ and $n=4$, this gives $\mathbb P(N>4)=(1+4)/16=5/16$; equivalently, $\mathbb P(X\leq2)=1-5/16=11/16$, matching $1/4+1/4+3/16$. At $p=1$, the [event](event.md) identity still holds, with $N=r$ and $B_n=n$ deterministically.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/12/b/ii/solution.md)
