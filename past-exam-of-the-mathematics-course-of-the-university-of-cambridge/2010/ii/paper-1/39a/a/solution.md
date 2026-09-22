<h1 id="39a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Householder-John theorem](../../../../../../householder-john-theorem.md) says that, for a splitting $A=M-N$ with $A$ Hermitian positive definite, positivity of $H=M^*+N=M^*+M-A$ implies $M$ is invertible and $\rho(M^{-1}N)<1$. Invertibility follows since $Mx=0$ for $x\ne0$ would give $x^*Hx=-x^*Ax<0$.

For clarity, the spectral-radius conclusion follows from a useful energy identity. Put $T=M^{-1}N=I-M^{-1}A$. Direct multiplication gives

$$
A-T^*AT=(I-T)^*H(I-T).
$$

If $Tv=\lambda v$, then

$$
(1-|\lambda|^2)v^*Av=|1-\lambda|^2v^*Hv.
$$

The [eigenvalue](../../../../../../eigenvalue.md) one is impossible because $A$ is invertible. Both quadratic forms are positive, so $|\lambda|<1$. The splitting iteration $Mx^{(k+1)}=Nx^{(k)}+b$ propagates its error by $T$; [spectral radius](../../../../../../spectral-radius.md) less than one therefore gives **convergence from every initial vector**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39A](../../39a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
