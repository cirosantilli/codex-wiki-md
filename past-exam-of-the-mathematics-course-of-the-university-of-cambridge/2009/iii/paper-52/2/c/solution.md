<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $N=2$, take the normalized [Pauli operators](../../../../../../pauli-operator.md) as the traceless basis. The matrix associated with a vector $s$ is $\rho=I/2+s\cdot\sigma$, where these basis matrices are the usual Pauli matrices divided by $\sqrt2$. Their multiplication relations give

$$
(s\cdot\sigma)^2=\frac{\|s\|^2}{2}I,
\qquad
\operatorname{spec}\rho=\left\{\frac12+\frac{\|s\|}{\sqrt2},\
\frac12-\frac{\|s\|}{\sqrt2}\right\}.
$$

At radius $1/\sqrt2$, these [eigenvalues](../../../../../../eigenvalue.md) are one and zero. Every sphere point therefore gives a positive rank-one projector. Any other orthonormal Hermitian basis merely changes the real coordinates by an [orthogonal transformation](../../../../../../orthogonal-transformation.md), so the result is basis independent.

For every $N>2$, choose a rank-one projector $P$ and consider the Hermitian trace-one matrix

$$
A=\frac2N I-P.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are $2/N-1$ once and $2/N$ with multiplicity $N-1$. They sum to one and satisfy

$$
\operatorname{Tr}(A^2)=\left(\frac2N-1\right)^2+(N-1)\frac4{N^2}=1.
$$

By orthonormality its traceless coordinate vector has squared length $1-1/N$, so it is on the specified sphere. But $2/N-1<0$, so $A$ is not a [density operator](../../../../../../density-matrix.md). Thus **for $N>2$, the [pure states](../../../../../../pure-state.md) occupy a proper subset of the sphere**; positivity excludes some of its points. In fact, this example is the antipodal [Bloch vector](../../../../../../bloch-vector.md) to that of $P$.

The usual assertion presumes $N\geq2$. If the trivial dimension $N=1$ is admitted, the radius-zero sphere consists of the single coordinate point, also corresponding to the single [pure state](../../../../../../pure-state.md), so that dimension is an additional trivial exception.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
