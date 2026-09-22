<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N+1=\dim M_k(SL_2(\mathbb Z))$. For each $0\leq i\leq N$, the dimension formula, equivalently the [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md), ensures that

$$
k-12i=4a_i+6b_i
$$

for some nonnegative integers $a_i,b_i$. Define

$$
h_i=\Delta^iE_4^{a_i}E_6^{b_i}.
$$

The [modular discriminant](../../../../../../modular-discriminant.md), $E_4$, and $E_6$ have integral Fourier coefficients and leading terms $q$, $1$, and $1$, respectively. Hence

$$
h_i=q^i+\sum_{n>i}c_{i,n}q^n,
\qquad c_{i,n}\in\mathbb Z.
$$

Their distinct orders of vanishing make the $h_i$ linearly independent, so they form a basis.

Starting with $f_N=h_N$, define $f_i$ downwards by subtracting from $h_i$ the integral multiples of $f_{i+1},\ldots,f_N$ needed to kill the coefficients of $q^{i+1},\ldots,q^N$. This integer Gaussian elimination preserves all integral coefficients and gives

$$
f_i=q^i+\sum_{n\geq N+1}a_n(f_i)q^n,
\qquad a_n(f_i)\in\mathbb Z.
$$

This is the [integral echelon basis of level-one modular forms](../../../../../../integral-echelon-basis-of-level-one-modular-forms.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
