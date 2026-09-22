<h1 id="b/4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $k=k_0=\min\{j:j!\geq n\}$. Then $k\to\infty$ and $(k-1)!<n\leq k!$. Also $k=O(\log n)$, because $j!\geq2^{j-1}$, so the needed block lengths are below $n/2$ for large $n$.

If $L\geq k+1$, then $X_{k+1}\geq1$. [Markov's inequality](../../../../../../markov-s-inequality.md) gives

$$
\mathbb P(L\geq k+1)\leq\frac n{(k+1)!}\leq\frac1{k+1}\to0.
$$

For $j=k-2$, the expected count satisfies $\mu=n/j!>k-1\to\infty$. Part (ii) bounds its [variance](../../../../../../variance-split.md) by $2\mu$, so [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) gives

$$
\mathbb P(L<k-2)=\mathbb P(X_{k-2}=0)\leq\frac2\mu<\frac2{k-1}\to0.
$$

Combining the tails proves

$$
\boxed{\mathbb P(k_0-2\leq L\leq k_0)\longrightarrow1}.
$$

The blocks are consecutive in the cyclic order throughout; this is not the longest increasing subsequence with arbitrary omitted positions.

This establishes the [longest increasing cyclic run of a random permutation](../../../../../../longest-increasing-cyclic-run-of-a-random-permutation.md) concentration bound.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
