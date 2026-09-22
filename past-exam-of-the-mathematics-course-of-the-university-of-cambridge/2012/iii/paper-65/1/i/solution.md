<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $X=\rho-\sigma$. The [trace distance](../../../../../../trace-distance.md) is $D(\rho,\sigma)=\tfrac12\|X\|_1$, where $\|X\|_1=\operatorname{Tr}\sqrt{X^\dagger X}$. Since $X$ is a [Hermitian operator](../../../../../../hermitian-operator.md), its [spectral decomposition](../../../../../../spectral-decomposition.md) is $X=\sum_jx_j|j\rangle\langle j|$. Define its [positive part of a Hermitian operator](../../../../../../positive-part-of-a-hermitian-operator.md) and [negative part of a Hermitian operator](../../../../../../negative-part-of-a-hermitian-operator.md) by

$$
Q=\sum_{x_j>0}x_j|j\rangle\langle j|,\qquad
R=\sum_{x_j<0}(-x_j)|j\rangle\langle j|.
$$

They are [positive semidefinite operators](../../../../../../positive-operator.md), satisfy $X=Q-R$ and $QR=0$, and obey $|X|=Q+R$. Therefore

$$
\boxed{D(\rho,\sigma)=\frac12(\operatorname{Tr}Q+\operatorname{Tr}R).}
$$

The states have equal trace, so $\operatorname{Tr}X=0$ and $\operatorname{Tr}Q=\operatorname{Tr}R=D(\rho,\sigma)$. This is the [spectral-parts formula for trace distance](../../../../../../spectral-parts-formula-for-trace-distance.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
