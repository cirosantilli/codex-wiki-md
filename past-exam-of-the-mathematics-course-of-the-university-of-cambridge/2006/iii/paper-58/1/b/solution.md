<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use most-significant-bit-first ordering, so $l=\sum_{j=1}^n b_j2^{n-j}$ and $|l\rangle=|b_1\rangle\otimes\cdots\otimes|b_n\rangle$. Then the coefficient factors as $e^{i\phi_ml}=\prod_je^{i\phi_m b_j2^{n-j}}$. Expanding a [tensor product](../../../../../../tensor-product.md) over all bit strings proves the [product decomposition of a Fourier phase state](../../../../../../product-decomposition-of-a-fourier-phase-state.md):

$$
\boxed{|\psi_m\rangle=\bigotimes_{j=1}^n
\frac{|0\rangle+e^{i\phi_m2^{n-j}}|1\rangle}{\sqrt2}.}
$$

Each factor is a normalized one-[qubit](../../../../../../qubit.md) state. The whole register is therefore a [product state](../../../../../../product-state.md), hence a [separable state](../../../../../../separable-quantum-state.md); no claim that arbitrary outputs of the Fourier transform are separable is needed. Reversing the bit convention reverses the order of these factors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
