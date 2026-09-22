<h1 id="3i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A binary code $c:\mathcal A\to\{0,1\}^*$ is a [prefix code](../../../../../../prefix-code.md) when no codeword is a proper prefix of another. If the source letters have probabilities $p_1,\ldots,p_m$ and codeword lengths $l_1,\ldots,l_m$, the [expected value](../../../../../../expected-value.md) of its codeword length is

$$
L=\sum_{r=1}^m p_r l_r.
$$

It is an [optimal prefix code](../../../../../../optimal-prefix-code.md) when it minimizes $L$ among all binary prefix codes for that source.

Suppose $p_i>p_j$ but $l_i>l_j$. Exchanging the codewords assigned to $\mu_i$ and $\mu_j$ leaves the set of words, and hence prefix-freeness, unchanged. The change in expected length is

$$
p_i l_j+p_j l_i-(p_i l_i+p_j l_j)
=(p_i-p_j)(l_j-l_i)<0,
$$

contradicting optimality. Thus

$$
\boxed{p_i>p_j\ \Longrightarrow\ l_i\leq l_j},
$$

which is the [probability monotonicity of optimal prefix-code lengths](../../../../../../probability-monotonicity-of-optimal-prefix-code-lengths.md).

Represent the code by its binary prefix tree and choose a codeword $wb$ of maximal length, where $b\in\{0,1\}$. Its sibling is $w(1-b)$. If that sibling were not a codeword, it could not have a codeword below it either, since such a word would be longer than $wb$. Replacing $wb$ by $w$ would then preserve prefix-freeness and strictly reduce $L$. This is impossible for an optimal code, so $w(1-b)$ is also a maximal-length codeword. The pair differs only in its last digit, proving the [deepest sibling property of an optimal prefix code](../../../../../../deepest-sibling-property-of-an-optimal-prefix-code.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3I](../../3i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
