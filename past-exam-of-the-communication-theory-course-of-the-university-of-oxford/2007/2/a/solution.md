<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A binary [prefix code](../../../../prefix-code.md) assigns distinct finite binary strings to the source symbols, with no assigned string a prefix of another. It is instantaneous because a complete codeword is recognized without needing the next word's bits.

Associate a word of length $\ell$ with its dyadic subinterval of $[0,1)$ of length $2^{-\ell}$. A prefix relation corresponds to interval containment. Prefix-free words therefore give disjoint intervals, whose total length is at most one. This proves necessity of [Kraft inequality](../../../../kraft-mcmillan-inequality.md).

For sufficiency, sort the requested nonnegative integer lengths increasingly and construct a code greedily in a binary tree. At depth $\ell_j$, the preceding codewords forbid exactly $\sum_{i<j}2^{\ell_j-\ell_i}$ nodes. The assumed inequality, retaining the positive contribution of the present word, bounds this integer by $2^{\ell_j}-1$. Thus at least one node is available; choose it. It is not below an earlier codeword, and the nondecreasing lengths prevent it from being a proper ancestor of an earlier word. Continue to obtain a [prefix code](../../../../prefix-code.md) of all the required lengths. Hence

$$
\boxed{\text{Such a code exists exactly when }\sum_k2^{-\ell_k}\le1}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
