<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

Define the [binomial coefficient](../../../../../binomial-coefficient.md) $\binom nk$ as the number of $k$-element subsets of an $n$-element set. Equivalently it is $n!/[k!(n-k)!]$: there are $n(n-1)\cdots(n-k+1)$ ordered lists of $k$ distinct elements, and each subset gives $k!$ such lists. The empty subset gives $\binom n0=1$.

Distinguish one element of the set. A $k$-element subset either omits it, giving $\binom{n-1}k$ possibilities, or contains it and chooses its other $k-1$ elements from the remaining set, giving $\binom{n-1}{k-1}$ possibilities. These cases are disjoint and exhaustive, proving [Pascal's identity](../../../../../pascal-s-rule.md):

$$
\boxed{\binom{n-1}k+\binom{n-1}{k-1}=\binom nk.}
$$

For the requested sum, fix $n\ge0$ and use [mathematical induction](../../../../../mathematical-induction.md) on $k$. At $k=0$, both sides equal one. If the assertion holds at $k$, adding the next summand gives

$$
\sum_{j=0}^{k+1}\binom{n+j}j
=\binom{n+k+1}k+\binom{n+k+1}{k+1}
=\binom{n+k+2}{k+1},
$$

where the last equality is [Pascal's identity](../../../../../pascal-s-rule.md). Thus the induction proves the [hockey-stick identity](../../../../../hockey-stick-identity.md) for all nonnegative $n,k$:

$$
\boxed{\sum_{j=0}^k\binom{n+j}j=\binom{n+k+1}k.}
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
