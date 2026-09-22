<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

Here is a nested-interval proof of the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md). Put every term of the bounded real [sequence](../../../../../sequence.md) in a [closed interval](../../../../../closed-real-interval.md) $I_0=[-M,M]$, with $M>0$. Bisect this interval and choose a closed half containing infinitely many terms. Repeating gives nested [closed intervals](../../../../../closed-real-interval.md) $I_j=[l_j,r_j]$, each containing infinitely many [sequence](../../../../../sequence.md) terms, with length $2M/2^j$.

By the [least-upper-bound property](../../../../../least-upper-bound-property.md), $x_* =\sup_j l_j$ exists. For each $j$, every lower endpoint lies at most $r_j$, while $l_j\le x_*$; hence $x_*\in I_j$. Choose increasing indices $n_j$ with $a_{n_j}\in I_j$, possible because each interval contains infinitely many terms. Then

$$
|a_{n_j}-x_*|\le 2M/2^j\longrightarrow0.
$$

Thus **every bounded real [sequence](../../../../../sequence.md) has a [convergent subsequence](../../../../../convergent-subsequence.md)**.

For a [sequence](../../../../../sequence.md) with no [convergent subsequence](../../../../../convergent-subsequence.md), take $a_n=n$: any [subsequence](../../../../../subsequence.md) has $n_j\ge j$, so its terms tend to positive infinity rather than to a finite [limit of a sequence](../../../../../limit-of-a-sequence.md). For an unbounded [sequence](../../../../../sequence.md) with a [convergent subsequence](../../../../../convergent-subsequence.md), take $a_{2n}=0$ and $a_{2n-1}=n$. Its odd terms are unbounded, while its even [subsequence](../../../../../subsequence.md) converges to zero.

## ↑ Ancestors (11)

1. [4C](../4c.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
