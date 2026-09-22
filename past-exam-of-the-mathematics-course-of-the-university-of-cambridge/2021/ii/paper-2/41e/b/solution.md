<h1 id="41e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a length-$M$ DFT with $M$ even, split the input into its even and odd entries. Two length-$M/2$ DFTs determine the result, followed by at most $M$ multiplications by twiddle factors. Hence the multiplication count satisfies

$$
T(M)\leq2T(M/2)+M,
$$

so induction gives $T(M)\leq CM\log_2M$ for powers of two. This proves the needed [fast Fourier transform](../../../../../../cooley-tukey-fft-algorithm.md) bound rather than assuming it.

Part (a) computes the length-$2N$ DFT of the reflected vector $y$ and then recovers

$$
z_k=\frac12\omega_{2N}^{k/2}Y_k,\qquad0\leq k<N.
$$

Forming $y$ uses no multiplications and the final recovery uses only $N$. Therefore the [discrete cosine transform](../../../../../../discrete-cosine-transform.md) costs at most

$$
\boxed{C(2N)\log(2N)+N=O(N\log N).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41E](../../41e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
