<h1 id="41d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\omega_{2N}=e^{-\pi i/N}$ and split the transform into its even and odd input samples. If $E_k$ and $O_k$ are the two length-$N$ transforms, then

$$
Y_k=E_k+\omega_{2N}^kO_k,
\qquad
Y_{k+N}=E_k-\omega_{2N}^kO_k,
\qquad 0\leq k<N.
$$

Thus a length-$2N$ transform requires two length-$N$ transforms and $O(N)$ further multiplications. Its multiplication count satisfies

$$
M(2N)\leq2M(N)+CN.
$$

Since $N$ is a power of two, iteration through $\log_2(2N)$ levels gives $M(2N)=O(N\log N)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41D](../../41d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
