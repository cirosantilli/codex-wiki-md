# Identification of a unique essential variable

↑ **Parent:** [Query complexity](query-complexity.md)

Suppose an unknown [function](function-split.md) on $\{1,\ldots,d\}^n$ has exactly one [essential variable](essential-variable-of-a-function.md). Query the diagonal inputs $(t,\ldots,t)$ to find two coordinates values $a,b$ giving distinct outputs; at most $d$ [function-evaluation oracle](function-oracle.md) calls suffice because the unary dependence is nonconstant. A query taking value $b$ on an index subset $H$ and $a$ outside it then tests whether the essential coordinate lies in $H$. Repeated halving locates it in at most $\lceil\log_2n\rceil$ further queries. If $n=1$, no query is needed.

For a matching lower bound with fixed $d$, restrict to $f^{(i)}(x)=1$ when $x_i=1$ and $2$ otherwise. Every query has only two possible replies. A binary [decision tree](decision-tree.md) distinguishing the $n$ possible essential indices needs at least $n$ leaves and depth $\lceil\log_2n\rceil$. [Integer](integer-split.md) outputs in the unrestricted problem need not be binary; the restricted family is what makes this [query complexity](query-complexity.md) argument valid.

## ↑ Ancestors (5)

1. [Query complexity](query-complexity.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/5/d/ii/solution.md)
