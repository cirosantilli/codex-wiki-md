# Mean absorption time of a lazy symmetric random walk

↑ **Parent:** [Lazy random walk](lazy-random-walk.md)

Consider a [random walk](random-walk-split.md) on $\{0,1,\ldots,n\}$ with [absorbing states](absorbing-state.md) $0,n$. At each interior state it stays in place with [probability](probability.md) $q$, and moves one position in either direction with [probability](probability.md) $(1-q)/2$, where $0\leq q<1$. Its [mean](expected-value-split.md) [absorption time](absorption-time.md) from $k$ is

$$
\boxed{\mathbb E_k[T]=\frac{k(n-k)}{1-q}.}
$$

**Proof.** A sequence of at most $n$ consecutive leftward moves ensures absorption, with [probability](probability.md) at least $((1-q)/2)^n>0$. Dividing time into blocks of length $n$ gives a [geometric series](geometric-series.md) bound on the survival [probabilities](probability.md), so the [expected value](expected-value-split.md) is finite. Let $e_k=\mathbb E_k[T]$. The [law of total expectation](law-of-total-expectation.md) and [first-step analysis](first-step-analysis.md) give

$$
e_k=1+qe_k+\frac{1-q}{2}(e_{k+1}+e_{k-1}),\qquad e_0=e_n=0.
$$

Thus $e_{k+1}-2e_k+e_{k-1}=-2/(1-q)$. A [particular solution](particular-solution.md) of this [linear recurrence relation](linear-recurrence-relation.md) is $-k^2/(1-q)$; its homogeneous solutions are $A+Bk$. The two [boundary conditions](boundary-condition.md) give $A=0$, $B=n/(1-q)$, proving both the formula and its uniqueness. Holding slows the usual symmetric [random walk](random-walk-split.md) by the factor $1/(1-q)$.

## ↑ Ancestors (9)

1. [Lazy random walk](lazy-random-walk.md)
2. [Random walk](random-walk-split.md)
3. [Markov chain](markov-chain-split.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Absorption time](absorption-time.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-iii/4/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability/7/b/ii/solution.md)
