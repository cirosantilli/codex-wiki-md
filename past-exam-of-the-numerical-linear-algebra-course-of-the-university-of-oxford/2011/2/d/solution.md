<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [matrix norm induced by an energy norm](../../../../matrix-norm-induced-by-an-energy-norm.md) and set $T=A^{1/2}C(\omega)A^{-1/2}=I-A^{1/2}B^{-1}A^{1/2}$. Multiplication gives

$$
T^TT=I-A^{1/2}\bigl[B^{-1}+B^{-T}-B^{-T}AB^{-1}\bigr]A^{1/2}.
$$

The bracket factors as $B^{-T}(B+B^T-A)B^{-1}$. Because $B=D/\omega+L$ and $A=D+L+L^T$,

$$
B+B^T-A=\left(\frac2\omega-1\right)D.
$$

Thus $T^TT=M(\omega)$ for the stated [matrix](../../../../matrix.md). In particular $M(\omega)$ is a [positive semidefinite matrix](../../../../positive-semidefinite-matrix.md). The Euclidean [operator norm](../../../../operator-norm.md) squared is the largest [eigenvalue](../../../../eigenvalue.md) of $T^TT$, and all those [eigenvalues](../../../../eigenvalue.md) are nonnegative. Consequently

$$
\boxed{\|C(\omega)\|_A=\|T\|_2=\rho(M(\omega))^{1/2}.}
$$

This identity is the algebraic step in the [energy-norm proof of convergence of SOR](../../../../energy-norm-proof-of-convergence-of-sor.md); [spectral radius](../../../../spectral-radius.md) equals the largest [eigenvalue](../../../../eigenvalue.md) here because $M(\omega)=T^TT$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
