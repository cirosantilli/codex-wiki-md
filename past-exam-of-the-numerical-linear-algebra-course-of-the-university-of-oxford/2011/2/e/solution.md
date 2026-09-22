<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $0<\omega<2$, the coefficient $\gamma=2/\omega-1$ is positive. Moreover

$$
G=A^{1/2}B^{-T}DB^{-1}A^{1/2}
$$

is a [positive-definite matrix](../../../../positive-definite-matrix.md): for a nonzero [vector](../../../../vector.md) $z$, put $y=B^{-1}A^{1/2}z\ne0$; then $z^TGz=y^TDy>0$. Hence every [eigenvalue](../../../../eigenvalue.md) of $M=I-\gamma G$ is strictly below one. Part (d) also gives $M=T^TT$, so these [eigenvalues](../../../../eigenvalue.md) are nonnegative. Therefore

$$
\boxed{\|C(\omega)\|_A=\sqrt{\rho(M(\omega))}<1,\qquad0<\omega<2.}
$$

The [energy-norm proof of convergence of SOR](../../../../energy-norm-proof-of-convergence-of-sor.md) thus makes the iteration a strict [contraction mapping](../../../../contraction-mapping.md) in this norm. Its [forward error](../../../../forward-error.md) satisfies $e^{(j+1)}=C(\omega)e^{(j)}$, so it converges geometrically to zero.

## ↑ Ancestors (12)

1. [E](../e.md)
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
