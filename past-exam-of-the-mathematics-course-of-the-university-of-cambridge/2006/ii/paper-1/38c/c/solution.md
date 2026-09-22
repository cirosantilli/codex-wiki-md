<h1 id="38c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an $n\times n$ [matrix](../../../../../../matrix.md) here, $D=I$. The sine vectors $v_j(i)=\sin(ij\pi/(n+1))$ give [eigenvalues](../../../../../../eigenvalue.md)

$$
\lambda_j=1+\frac12\cos\frac{j\pi}{n+1},\quad1\leq j\leq n.
$$

Thus every [eigenvalue](../../../../../../eigenvalue.md) lies strictly between $1/2$ and $3/2$. For $0<\omega\leq4/3$, $0<\omega\lambda_j<2$, so $|1-\omega\lambda_j|<1$, including the upper endpoint $\omega=4/3$. Hence **the iteration converges for the entire stated range**.

The extreme [eigenvalues](../../../../../../eigenvalue.md) are $1-a$ and $1+a$, with $a=\tfrac12\cos(\pi/(n+1))$. The [spectral radius](../../../../../../spectral-radius.md) is $\max(|1-\omega(1-a)|,|1-\omega(1+a)|)=|1-\omega|+a\omega$ for $\omega>0$. It decreases up to one and increases after one, since $0\leq a<1$. Therefore

$$
\boxed{\omega_{\rm opt}=1,\qquad\rho_{\rm opt}=\frac12\cos\frac{\pi}{n+1}.}
$$

For $n=1$ the same formula gives zero [spectral radius](../../../../../../spectral-radius.md) and exact solution in one ordinary Jacobi step.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38C](../../38c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
