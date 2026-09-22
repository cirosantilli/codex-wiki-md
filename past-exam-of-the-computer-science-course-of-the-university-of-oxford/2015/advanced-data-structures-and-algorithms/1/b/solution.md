<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes: starting from zero, $n$ increments of the [decimal counter](../../../../../decimal-counter.md) cost $\Theta(n)$ [digit](../../../../../numerical-digit.md) changes**, uniformly in the number $k$ of [digits](../../../../../numerical-digit.md). An increment changes the trailing [digits](../../../../../numerical-digit.md) equal to $9$ into $0$ and increases the next [digit](../../../../../numerical-digit.md). Number [digits](../../../../../numerical-digit.md) from $0$ at the least significant end. [Digit](../../../../../numerical-digit.md) $i$ changes once every $10^i$ increments, so the exact number of changes is

$$
C_{10}(n,k)=\sum_{i=0}^{k-1}\left\lfloor\frac{n}{10^i}\right\rfloor
\leq n\sum_{i=0}^{\infty}10^{-i}=\frac{10n}{9}.
$$

Here the [floor function](../../../../../floor-function.md) counts carries reaching each position, and the last equality sums a [geometric series](../../../../../geometric-series.md). Since [digit](../../../../../numerical-digit.md) $0$ changes on every increment, $C_{10}(n,k)\geq n$ for $k\geq1$. The loop tests and carry handling add only a constant amount per changed [digit](../../../../../numerical-digit.md) and per operation, giving the same [time complexity](../../../../../time-complexity.md).

An [accounting method](../../../../../accounting-method.md) explanation is also possible. Charge two credits for each change of [digit](../../../../../numerical-digit.md) $0$: one pays for that change and one joins a common bank. For $n$ increments the higher [digits](../../../../../numerical-digit.md) change at most $n/9$ times, so their costs can be covered from that bank; the displayed prefix bound ensures that it never goes negative.

The formula allows wraparound modulo $10^k$; alternatively, restrict to increments before overflow. Initializing the [array](../../../../../array-data-structure.md) itself costs $\Theta(k)$ if that is counted separately. If the initial [digits](../../../../../numerical-digit.md) are arbitrary, the number of changes at position $i$ is at most $\lceil n/10^i\rceil$, giving $O(n+k)$ in [Big O notation](../../../../../big-o-notation.md). Starting with all [digits](../../../../../numerical-digit.md) equal to $9$ makes the first increment cost $k$, so the initial-state convention matters.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
