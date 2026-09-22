# Geometric tail bound from a uniform escape probability

↑ **Parent:** [Stopping time](stopping-time.md)

Suppose a nonnegative [stopping time](stopping-time.md) $T$ and constants $L>0$, $0<q\leq1$ satisfy $\mathbb P(T\leq nL+L\mid\mathcal F_{nL})\geq q$ on $\{T>nL\}$. Take $L$ to be a positive integer in discrete time. Then

$$
\mathbb P(T>nL)\leq(1-q)^n,\qquad \mathbb ET\leq L/q.
$$

On the surviving [event](event.md), conditional survival is at most $1-q$. The [tower property of conditional expectation](law-of-total-expectation.md) therefore gives

$$
\mathbb P(T>(n+1)L)\leq(1-q)\mathbb P(T>nL).
$$

Induction proves the geometric bound. Partitioning the tail [integral](integral.md) into intervals of length $L$ then gives $\mathbb ET\leq L\sum_{n\geq0}\mathbb P(T>nL)\leq L/q$; in discrete time, group the tail sum into $L$ successive integer indices instead. This proves finite [expected hitting times](expected-hitting-time.md) when every surviving state has a uniform positive chance of escaping within a fixed time. It works in discrete or continuous time without assuming [independence](independent-random-variables.md) of successive survival [events](event.md).

**Table of contents**

- [Random-walk exit bound from a positive-increment block](random-walk-exit-bound-from-a-positive-increment-block.md)

## ↑ Ancestors (7)

1. [Stopping time](stopping-time.md)
2. [Martingale](martingale-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Brownian hitting of lattice spheres](brownian-hitting-of-lattice-spheres.md)
- [Drifted Brownian interval-exit probability](drifted-brownian-interval-exit-probability.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/5/a/solution.md)
- [Random-walk exit bound from a positive-increment block](random-walk-exit-bound-from-a-positive-increment-block.md)
- [Waiting time for a word in independent nonuniform symbols](waiting-time-for-a-word-in-independent-nonuniform-symbols.md)
