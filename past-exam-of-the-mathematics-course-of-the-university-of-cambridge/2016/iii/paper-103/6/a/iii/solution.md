<h1 id="6/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Every old box either remains untouched or has its entry replaced by a strictly smaller incoming value. Thus **on all boxes of the original diagram**,

$$
\boxed{P'_{i,j}\leq P_{i,j}}.
$$

The appended box has no old entry to compare; equivalently, extend the old filling by $+\infty$ outside its diagram if the inequality is to be written for every position.

We now prove the unheaded [longest increasing subsequence](../../../../../../../longest-increasing-subsequence.md) assertion. After any prefix of the permutation has been inserted, write the first-row entries as $b_1<\cdots<b_r$. The useful invariant is: **$b_j$ is the smallest possible final value of an increasing subsequence of length $j$ in that prefix**, and $r$ is the greatest possible subsequence length. It holds for the empty prefix.

Suppose the next letter $x$ enters the first row in column $j$. Then $b_{j-1}<x$, if $j>1$, while $b_j>x$ if column $j$ already exists. A subsequence of length $j-1$ ending at $b_{j-1}$ can be extended by $x$, giving a subsequence ending at $x$ of length $j$; for $j=1$, the singleton suffices. A longer subsequence ending at $x$ would have an earlier length-$j$ prefix ending below $x$, contradicting the minimality of $b_j$. If $j=r+1$, the previous prefix has no subsequence longer than $r$, giving the same upper bound.

Replacing $b_j$ by $x$, or appending it at $j=r+1$, preserves the invariant. It lowers the smallest final value at length $j$. At smaller lengths, existing minima are already below $x$, so they cannot improve; no subsequence of greater length can end at $x$. The lower rows do not change this first-row update. Induction proves that **the longest increasing subsequence ending in $x_k$ has length exactly the column in which $x_k$ first enters**.

Taking the maximum over all letters gives **Schensted's first-row theorem**:

$$
\boxed{\operatorname{LIS}(\pi)=\lambda_1(P(\pi))}.
$$

This concerns the column of the incoming letter in the first row, not the column of the new box that eventually appears at the end of the bumping path.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
