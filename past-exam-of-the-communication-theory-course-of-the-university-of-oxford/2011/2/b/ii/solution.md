<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First consider any instantaneous code. Put $K_0=\sum_k2^{-l_k}\leq1$ and $q_k=2^{-l_k}/K_0$. Part 1(a) gives

$$
0\leq d(p,q)=-H(X)+\mathbb EL+\log_2K_0,
$$

so $\mathbb EL\geq H(X)-\log_2K_0\geq H(X)$.

For the construction, take the Shannon lengths $l_k=\lceil-\log_2p_k\rceil$. Then $2^{-l_k}\leq p_k$, so Kraft's condition holds. Also $l_k<-\log_2p_k+1$ for every $k$. Averaging gives

$$
\boxed{H(X)\leq\mathbb EL<H(X)+1.}
$$

For a nontrivial [alphabet](../../../../../alphabet.md) all $p_k<1$, so these lengths are positive and the ordinary code convention applies. For a deterministic one-symbol source, the usual zero-bit convention uses $l_1=0$ when the number of source symbols is externally known. If strictly nonempty [codewords](../../../../../codeword.md) and arbitrary unframed message lengths are required instead, that degenerate case has $\mathbb EL\geq1$ and cannot satisfy the printed strict upper bound. This convention issue does not affect sources with at least two symbols.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
