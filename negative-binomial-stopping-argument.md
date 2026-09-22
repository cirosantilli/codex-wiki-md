# Negative binomial stopping argument

↑ **Parent:** [Negative binomial distribution](negative-binomial-distribution.md)

For the [negative binomial distribution](negative-binomial-distribution.md) with positive [integer](integer.md) target $r$ and success [probability](probability.md) $0<p<1$, the $r$th success occurs after exactly $x$ failures only if the final trial is a success, while the preceding $x+r-1$ trials contain $x$ failures and $r-1$ successes. Choosing the failure locations gives the [binomial coefficient](binomial-coefficient.md) $\binom{x+r-1}{x}$. Each such stopped sequence has [probability](probability.md) $(1-p)^xp^r$ by [independence](independent-random-variables.md), and the sequences describe mutually exclusive [events](event.md), so their [probabilities](probability.md) add. This proves the [probability mass function](probability-mass-function.md). Counting arrangements among all $x+r$ positions would wrongly include sequences that already reached the target earlier. The same argument is used for three heads in [MIT 18.05, spring 2022, problem set 9 solutions, problem 2(b)](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_pset09_sol.pdf).

A short route to normalization and moments is to split the failures count into successive waiting blocks:

$$
X=F_1+\cdots+F_r,
$$

where $F_i$ counts failures after success $i-1$ and before success $i$, with $F_1$ starting at the first trial. Fresh [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md) make the blocks [independent](independent-random-variables.md), each with the failures-count [geometric distribution](geometric-distribution.md). Each block has total mass $p\sum_{j=0}^{\infty}(1-p)^j=1$ by the [geometric series](geometric-series.md), so their sum also defines a normalized [probability distribution](probability-distribution.md). The [linearity of expectation](linearity-of-expectation.md) and [variance additivity for independent random variables](variance-additivity-for-independent-random-variables.md) give $\mathbb E X=r(1-p)/p$ and $\operatorname{Var}(X)=r(1-p)/p^2$. This makes the moments transparent without a long calculation of sums. For $p=1$, every block is zero.

The same stopping rule connects a waiting count to a fixed-length count. Let $N=X+r$ be the trial number of the $r$th success, and let $B_n$ count successes in the first $n$ trials, so $B_n$ has a [binomial distribution](binomial-distribution.md). For any nonnegative [integer](integer.md) $n$,

$$
\{N>n\}=\{B_n<r\},\qquad
\mathbb P(N>n)=\sum_{k=0}^{\min(r-1,n)}\binom nk p^k(1-p)^{n-k}.
$$

The target is still unmet after $n$ trials exactly when fewer than $r$ successes have occurred. With $r=2$, $p=1/2$ and $n=4$, this gives $\mathbb P(N>4)=(1+4)/16=5/16$; equivalently, $\mathbb P(X\leq2)=1-5/16=11/16$, matching $1/4+1/4+3/16$. At $p=1$, the [event](event.md) identity still holds, with $N=r$ and $B_n=n$ deterministically.

## ↑ Ancestors (8)

1. [Negative binomial distribution](negative-binomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Negative binomial distribution](negative-binomial-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2/12f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/5j/solution.md)
