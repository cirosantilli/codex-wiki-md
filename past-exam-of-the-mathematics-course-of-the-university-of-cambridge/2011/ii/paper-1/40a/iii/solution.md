<h1 id="40a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $\omega=1$, the [Jacobi method](../../../../../../jacobi-method.md) iteration matrix $T=I-D^{-1}A$ has zero diagonal, nonnegative axial entries $1/5$, and diagonal-neighbour entries $1/20$. Its row sums are at most one; they are strictly below one at grid points next to the Dirichlet boundary. Its graph is connected by the positive axial entries.

To prove the strict [spectral radius](../../../../../../spectral-radius.md) bound, let $Tz=\lambda z$ with $z\ne0$ and choose a component of maximum magnitude $M>0$. Then

$$
|\lambda|M\leq\sum_wT_{vw}|z_w|\leq M\sum_wT_{vw}\leq M,
$$

so $|\lambda|\leq1$. If equality held, every positive-weight neighbour of a maximal component would also have modulus $M$, and that row would have sum one. Propagating along axial edges reaches a boundary-adjacent row, whose sum is strictly less than one, a contradiction. This also covers a one-point interior grid, for which $T=0$. Hence

$$
\boxed{\rho(T)<1.}
$$

The standard convergence theorem for a stationary linear iteration says it converges from every initial vector exactly when its iteration matrix has spectral radius below one. Since $A$ is invertible by (i), the error satisfies $e^{(r)}=T^re^{(0)}\to0$ and

$$
\boxed{\omega=1\text{ converges to the unique solution of }Au=b.}
$$

Weak row diagonal dominance alone would not prove convergence; the connection to a strictly deficient boundary row supplies the required strictness.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [40A](../../40a.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
