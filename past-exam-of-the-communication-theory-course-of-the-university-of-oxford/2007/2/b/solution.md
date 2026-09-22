<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work on the source support, so its listed probabilities are positive; zero-probability symbols may be omitted. An optimal binary [prefix code](../../../../prefix-code.md) minimizes the [expected codeword length](../../../../expected-codeword-length.md) for that distribution. The same optimal expected length is attained when optimization is over uniquely decipherable codes, by the converse and existence parts of [Kraft–McMillan inequality](../../../../kraft-mcmillan-inequality.md).

Choose Shannon lengths $\ell_k=\lceil-\log_2p_k\rceil$. They satisfy $2^{-\ell_k}\le p_k$, so the preceding existence theorem gives a [prefix code](../../../../prefix-code.md) with those lengths. Also $\ell_k<-\log_2p_k+1$ for every symbol, including the integer cases. Thus its expected length is less than $H(X)+1$. An optimal code cannot have a larger expected length, proving

$$
\boxed{\sum_kp_k\ell_k<H(X)+1}.
$$

For a deterministic one-symbol source the empty word has length zero, consistent with this bound.

## ↑ Ancestors (12)

1. [B](../b.md)
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
