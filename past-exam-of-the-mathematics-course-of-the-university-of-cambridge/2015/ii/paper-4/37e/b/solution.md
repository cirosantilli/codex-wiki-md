<h1 id="37e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [linear-system residual](../../../../../../linear-system-residual.md) at an approximate solution $x_m$ is $r_m=b-Ax_m$. For symmetric positive definite $A$, the [Conjugate gradient method](../../../../../../conjugate-gradient-method.md) has $x_m\in x_0+K_m(A,r_0)$ and minimizes the squared $A$-norm of the error over that affine space; its residual is orthogonal to $K_m(A,r_0)$.

If $A$ has $t$ distinct eigenvalues, interpolate $q(\lambda)=1/\lambda$ on them with a polynomial of degree at most $t-1$. The [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) gives $A^{-1}=q(A)$, so the exact correction $x_*-x_0=A^{-1}r_0$ lies in $K_t(A,r_0)$. The minimum possible error at step $t$ is therefore zero. Thus $\boxed{\text{CG terminates in at most }t\text{ steps}}$ in exact arithmetic, possibly earlier if the initial residual has fewer eigencomponents. If $r_0=0$, it terminates immediately.

A symmetric positive definite [matrix preconditioner](../../../../../../matrix-preconditioner.md) $M$ changes the system to $M^{-1/2}AM^{-1/2}z=M^{-1/2}b$, with $x=M^{-1/2}z$; practical preconditioned CG applies solves with $M$. It can accelerate convergence by reducing the [spectral condition number of a positive-definite matrix](../../../../../../spectral-condition-number-of-a-positive-definite-matrix.md), which improves the usual bound involving $(\sqrt\kappa-1)/(\sqrt\kappa+1)$, and by clustering [eigenvalues](../../../../../../eigenvalue.md), which allows low-degree residual polynomials small on the spectrum even when the extreme-eigenvalue bound is pessimistic.

Choosing $\boxed{M=A}$ makes the transformed matrix $I$, so one step suffices. But applying $M^{-1}$ already requires solving the original problem, and constructing an exact factorization generally incurs its original computational cost. It is therefore not a useful shortcut for a single unsolved system, though an available factorization can be reused for multiple right-hand sides. Effective [matrix preconditioning](../../../../../../matrix-preconditioning.md) balances spectral improvement against inexpensive application.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37E](../../37e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
