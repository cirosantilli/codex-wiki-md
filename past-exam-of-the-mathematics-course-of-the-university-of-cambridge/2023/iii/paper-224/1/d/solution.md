<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $M=\max_kp_k$ and choose an index $m$ with $p_m=M$. Splitting the overlap sum at $m$ gives

$$
q\leq\sum_{k<m}p_k+\sum_{k\geq m}p_{k+1}=1-p_m=1-M,
$$

so $1-q\geq M$. Moreover, [information entropy dominates min-entropy](../../../../../../information-entropy-dominates-min-entropy.md) gives $H(X)\geq-\log_2M$, and hence $2^{-H(X)}\leq M\leq1-q$.

Apply [Pinsker's inequality](../../../../../../pinsker-s-inequality.md) in natural logarithms. Because the paper writes total variation as the full $\ell^1$ distance, part c yields

$$
(\log_e2)D(P_X\Vert P_{X-1})
=D_e(P_X\Vert P_{X-1})
\geq\frac12\lVert P_X-P_{X-1}\rVert_1^2
=2(1-q)^2.
$$

Combining the two estimates proves

$$
(\log_e2)D(P_X\Vert P_{X-1})
\geq2(1-q)^2
\geq2M^2
\geq2^{-2H(X)+1}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
