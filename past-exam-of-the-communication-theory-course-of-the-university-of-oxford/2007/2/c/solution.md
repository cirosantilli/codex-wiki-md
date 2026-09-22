<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At an interior tree node write $A,B$ for the total masses in its two children, and $S=A+B$. Counting path lengths and telescoping the [Shannon entropy](../../../../information-entropy-split.md) over the binary decisions gives

$$
\bar s=\sum_vS_v,\qquad H(X)=\sum_vS_vh(A_v/S_v).
$$

Indeed each symbol contributes its probability once per ancestral interior node to the first sum. In the second sum, expanding $S h(A/S)=S\log_2S-A\log_2A-B\log_2B$ cancels the interior terms and leaves the source [Shannon entropy](../../../../information-entropy-split.md). The supplied inequality now bounds redundancy by

$$
\bar s-H(X)\le\sum_v|A_v-B_v|.
$$

Consider the cut between adjacent symbols $k,k+1$ made at one node. If its left side is heavier, moving its last symbol to the right must not improve the chosen cut. Writing $\Delta=A-B\ge0$, this says $|\Delta-2p_k|\ge\Delta$, which implies $\Delta\le p_k$; when the left side is a singleton the same bound is immediate. If the right side is heavier, the corresponding argument gives $|A-B|\le p_{k+1}$. In all cases

$$
|A-B|\le\max(p_k,p_{k+1})\le p_k+p_{k+1}.
$$

Recursive subdivision of contiguous blocks uses each original gap exactly once. Summing over the $m-1$ gaps therefore gives

$$
\bar s-H(X)\le2-p_1-p_m<2,
$$

proving **$\bar s<H(X)+2$**. If probabilities are already nonincreasing, each maximum is $p_k$ and the improved bound is $\bar s-H(X)\le1-p_m<1$. Thus **the sorted version has expected length less than $H(X)+1$**, although it need not be optimal. For one symbol the assertions hold directly. This is the [Fano slice code redundancy bound](../../../../fano-slice-code-redundancy-bound.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
