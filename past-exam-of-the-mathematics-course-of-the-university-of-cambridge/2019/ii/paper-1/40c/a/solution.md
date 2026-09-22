<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [matrix splitting](../../../../../../matrix-splitting.md) $A=M-N$ with $M$ invertible. Then $Ax=b$ is equivalent to

$$
x=M^{-1}Nx+M^{-1}b,
$$

and the associated [stationary iterative method for a linear system](../../../../../../stationary-iterative-method-for-a-linear-system.md) is

$$
x^{(k+1)}=Hx^{(k)}+M^{-1}b,
\qquad H=M^{-1}N.
$$

For the [Jacobi method](../../../../../../jacobi-method.md), write $A=D+L+U$ with $D$ diagonal and $L,U$ strictly lower and upper triangular, and take

$$
M=D,\qquad N=-(L+U).
$$

Thus

$$
\boxed{x^{(k+1)}=-D^{-1}(L+U)x^{(k)}+D^{-1}b.}
$$

The iteration converges for every initial vector exactly when the [spectral radius](../../../../../../spectral-radius.md) of its iteration matrix satisfies

$$
\boxed{\rho\bigl(-D^{-1}(L+U)\bigr)<1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
