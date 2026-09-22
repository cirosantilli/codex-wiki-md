<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $c_j=2^j+1$ for $0\leq j\leq k$, with a separate unit denomination. Choose, among all [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md)-coin representations of the target, one whose vector of counts is lexicographically largest when larger denominations come first. Such a choice exists because a fixed positive target has only finitely many representations.

There cannot be two unit coins: replacing them by one $c_0=2$ decreases the count. For $j<k$, two copies of $c_j$ can be exchanged using

$$
2c_j=c_{j+1}+1.
$$

This keeps the coin count unchanged but increases the first differing larger-denomination count, contradicting the chosen lexicographic [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md). Thus **there exists an optimal representation using at most one of each denomination below the largest**. The largest denomination may repeat.

It remains to show why that normalization implies greedy optimality; uniqueness alone is not enough for an arbitrary coin system. Fix a denomination $c_j$. Let $L$ be the total value of all coins smaller than $c_j$ in the chosen optimal representation, and let $r$ be their number. These smaller coins are distinct. If $I\subseteq\{0,\ldots,j-1\}$ records the selected non-unit denominations, then

$$
L=\sum_{i\in I}2^i+r,\qquad \sum_{i\in I}2^i\leq2^j-1.
$$

If $L\geq c_j$, replace all $r$ smaller coins by one $c_j$ and $L-c_j$ unit coins. The new number of coins is

$$
1+L-c_j=L-2^j\leq r-1,
$$

contradicting optimality. Therefore **the total value below every denomination $c_j$ is strictly less than $c_j$**.

At the largest denomination, this forces its count to be $\lfloor n/c_k\rfloor$: its residual value is nonnegative and smaller than $c_k$. Remove those coins. The same smaller-denomination property then forces the next quotient, and so on down to the unit coin. These are exactly greedy's choices, proving **greedy is optimal for every positive target**. The argument also covers $k=0$, where the denominations are two and one. Independent comparison with coin-change [dynamic programming](../../../../../dynamic-programming.md) confirmed the formula for all $0\leq k\leq8$ and targets from one to 2,000; that finite check supplements the proof.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
