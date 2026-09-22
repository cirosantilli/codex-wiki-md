<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [codeword](../../../../../codeword.md) lengths are [integers](../../../../../integer-split.md). For necessity, take $L=\max_k l_k$ and view [codewords](../../../../../codeword.md) as [nodes](../../../../../node-dynamical-systems.md) of the [binary tree](../../../../../binary-tree.md). A [codeword](../../../../../codeword.md) of length $l_k$ has $2^{L-l_k}$ descendant words at depth $L$. [Prefix-freeness](../../../../../prefix-code.md) makes these descendant [sets](../../../../../set-split.md) disjoint, so

$$
\sum_k2^{L-l_k}\leq2^L,\qquad\text{hence}\quad\sum_k2^{-l_k}\leq1.
$$

For sufficiency, reorder the lengths nondecreasingly. Assign words successively. At depth $l_k$, words extending previously assigned [codewords](../../../../../codeword.md) number

$$
\sum_{i<k}2^{l_k-l_i}.
$$

The asserted [inequality](../../../../../inequality-mathematics.md), even after dropping the later nonnegative terms, gives

$$
\sum_{i<k}2^{l_k-l_i}+1\leq2^{l_k}.
$$

Thus at least one depth-$l_k$ word does not extend an earlier word. Choose it. Since lengths are nondecreasing, it cannot be a proper prefix of a shorter earlier word, and equal-length duplicates have been excluded. [Induction](../../../../../mathematical-induction.md) constructs the required code. Therefore [Kraft inequality](../../../../../kraft-mcmillan-inequality.md) is necessary and sufficient:

$$
\boxed{\text{a binary prefix code with these lengths exists}\iff\sum_k2^{-l_k}\leq1.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
