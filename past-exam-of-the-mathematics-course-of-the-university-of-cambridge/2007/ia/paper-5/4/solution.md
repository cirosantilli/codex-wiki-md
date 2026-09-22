<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Define the [binomial coefficient](../../../../../binomial-coefficient.md) $\binom nk$ to be the number of $k$-element subsets of an $n$-element set. Equivalently, count ordered selections and divide by the $k!$ orders of each subset to obtain $\binom nk=n!/[k!(n-k)!]$, with $\binom n0=\binom nn=1$.

Fix one distinguished element. The $k$-subsets not containing it are counted by $\binom{n-1}{k}$; those containing it correspond bijectively to $(k-1)$-subsets of the remaining $n-1$ elements. These are disjoint and exhaustive classes, proving [Pascal's identity](../../../../../pascal-s-rule.md):

$$
\boxed{\binom{n-1}{k}+\binom{n-1}{k-1}=\binom nk.}
$$

For the summation, use [mathematical induction](../../../../../mathematical-induction.md) on $k$, retaining an arbitrary fixed $n\ge0$. At $k=0$, both sides equal one. Suppose $\sum_{j=0}^k\binom{n+j}{j}=\binom{n+k+1}{k}$. Adding the next term and applying [Pascal's identity](../../../../../pascal-s-rule.md) gives

$$
\sum_{j=0}^{k+1}\binom{n+j}{j}=\binom{n+k+1}{k}+\binom{n+k+1}{k+1}=\binom{n+k+2}{k+1}.
$$

This is the required statement for $k+1$, completing the induction, including $n=0$. Hence the [hockey-stick identity](../../../../../hockey-stick-identity.md) in this form is

$$
\boxed{\displaystyle\sum_{j=0}^k\binom{n+j}{j}=\binom{n+k+1}{k}\quad(n,k\ge0).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
