<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A [self-adjoint operator](../../../../../self-adjoint-operator.md) $T$ satisfies $\langle Tx,y\rangle=\langle x,Ty\rangle$. If $Tx=\lambda x$, then $\lambda\langle x,x\rangle=\langle Tx,x\rangle=\langle x,Tx\rangle=\overline\lambda\langle x,x\rangle$, so $\lambda\in\mathbb R$. An eigenvector exists over $\mathbb C$; its [orthogonal complement](../../../../../orthogonal-complement.md) is $T$-invariant. Induction on dimension produces an [orthonormal basis](../../../../../orthonormal-basis.md) of eigenvectors, proving the [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md).

A self-adjoint $T$ is positive definite exactly when every eigenvalue is positive, since $\langle Tx,x\rangle=\sum_i\lambda_i|x_i|^2$ in an eigenbasis. The quadratic forms of two positive-definite operators add, so their sum is positive definite.

The same eigenbasis shows that $\operatorname{spec}T\subset[a,b]$ exactly when $T-\lambda I$ is positive definite for every $\lambda<a$ and negative definite for every $\lambda>b$. Finally, if $v$ is a unit eigenvector of $\alpha+\beta$ with eigenvalue $\gamma$, the [Rayleigh quotient](../../../../../rayleigh-quotient.md) bounds give

$$
\gamma=\langle\alpha v,v\rangle+\langle\beta v,v\rangle\in[a+c,b+d].
$$

Thus **every eigenvalue of $\alpha+\beta$ lies in $[a+c,b+d]$**.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
