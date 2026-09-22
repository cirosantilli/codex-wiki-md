<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since the derivative of $\tanh(\beta x)$ at zero is $\beta$, the [Jacobian matrix](../../../../../../jacobian-matrix.md) of this directed rate network is

$$
J=\frac1\tau\begin{pmatrix}-1&0&\beta W_{13}\\\beta W_{21}&-1&0\\0&\beta W_{32}&-1\end{pmatrix}.
$$

With $a=1+\tau\lambda$, its characteristic determinant is

$$
\tau^3\det(\lambda I-J)=\det\begin{pmatrix}a&0&-\beta W_{13}\\-\beta W_{21}&a&0\\0&-\beta W_{32}&a\end{pmatrix}=a^3-\beta^3W_{13}W_{32}W_{21}.
$$

Thus the [eigenvalues](../../../../../../eigenvalue.md) satisfy

$$
\boxed{(1+\tau\lambda)^3=\Gamma,\qquad\Gamma=\beta^3W_{13}W_{32}W_{21}}.
$$

This establishes [three-neuron ring stability](../../../../../../three-neuron-ring-stability.md) from the loop product. The ring is directed, so the symmetric-weight [Hopfield network](../../../../../../hopfield-network.md) energy argument does not apply. Assume the physical relaxation time $\tau>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
