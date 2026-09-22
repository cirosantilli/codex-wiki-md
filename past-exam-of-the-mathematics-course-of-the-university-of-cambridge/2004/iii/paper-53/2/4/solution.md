<h1 id="2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Apply the [Hadamard transform](../../../../../../hadamard-transform.md) to the conditional [coset state](../../../../../../coset-state.md). The amplitude of a first-register output $z$ is

$$
\frac{(-1)^{x_k\cdot z}+(-1)^{(x_k+s)\cdot z}}{\sqrt{2^{n+1}}}=\frac{(-1)^{x_k\cdot z}}{\sqrt{2^{n+1}}}\bigl[1+(-1)^{s\cdot z}\bigr].
$$

When $s\cdot z=1$ over $\mathbb F_2$, the two terms cancel exactly. When $s\cdot z=0$, their squared modulus is $2^{-(n-1)}$. Thus

$$
\boxed{\Pr(z)=\begin{cases}2^{-(n-1)},&z\cdot s=0,\\0,&z\cdot s=1.\end{cases}}
$$

There are $2^{n-1}$ orthogonal outputs, so these probabilities sum to one. The distribution is independent of the particular observed fibre. It is the [Single-sample distribution in Simon's algorithm](../../../../../../single-sample-distribution-in-simon-s-algorithm.md): each run gives a uniform random equation restricting the hidden period to the [orthogonal complement over the binary field](../../../../../../orthogonal-complement-over-the-binary-field.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
