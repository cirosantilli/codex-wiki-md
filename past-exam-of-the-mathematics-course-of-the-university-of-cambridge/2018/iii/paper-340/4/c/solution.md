<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The printed definition of the [restricted isometry constant](../../../../../../restricted-isometry-constant.md) omits the quantifier: the two inequalities must hold for every vector with at most $s$ nonzero entries. The constant is the smallest nonnegative value, or the infimum over positive values; it can be zero.

Let $T=\operatorname{supp}u\cup\operatorname{supp}v$ and $B=A_T^*A_T-I$. The [restricted isometry property](../../../../../../restricted-isometry-property.md) of order $s+t$ says $|z^*Bz|\le\delta_{s+t}\|z\|_2^2$ for every $z$ supported on $T$. Since $B$ is a [Hermitian matrix](../../../../../../hermitian-operator.md), the [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) implies $\|B\|_{2\to2}\le\delta_{s+t}$. Disjoint supports give $\langle u,v\rangle=0$, hence

$$
\boxed{|\langle Au,Av\rangle|=|u_T^*Bv_T|\le\delta_{s+t}\|u\|_2\|v\|_2.}
$$

This argument works over $\mathbb C$ and avoids the loss of a factor caused by treating real and imaginary parts separately.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
