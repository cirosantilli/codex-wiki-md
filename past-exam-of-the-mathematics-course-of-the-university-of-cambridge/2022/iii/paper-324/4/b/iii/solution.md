<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Prepare $2^{-n/2}\sum_x|x\rangle|0^n\rangle$, query the oracle, and measure or discard the output register. For $p\ne0$, the input register becomes the [coset state](../../../../../../../coset-state.md)

$$
\frac{|x\rangle+|x\mathbin\oplus p\rangle}{\sqrt2}.
$$

Apply $H^{\otimes n}$, the [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) over $(\mathbb Z_2)^n$. The two amplitudes interfere destructively unless the [binary inner product](../../../../../../../binary-inner-product.md) satisfies

$$
y\mathbin\cdot p=0\pmod2,
$$

and every vector in this orthogonal subspace is sampled uniformly. Repeat until $n-1$ independent equations have been collected, then use [Gaussian elimination](../../../../../../../gaussian-elimination.md) over $\mathbb F_2$ to find their one-dimensional [null space](../../../../../../../kernel-of-a-linear-map.md); its nonzero vector is $p$. This is [Simon's algorithm](../../../../../../../simon-s-algorithm.md). It uses $O(n)$ oracle queries with high probability and polynomial classical work. When $p=0^n$, the function is injective and the samples eventually span all of $(\mathbb F_2)^n$, which distinguishes that case with arbitrarily high probability.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
