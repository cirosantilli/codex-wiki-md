<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An even number of negative weights gives $\Gamma>0$ when all three connections are nonzero. Put $r=\Gamma^{1/3}$. The three cube roots give

$$
\boxed{\lambda_0=\frac{r-1}\tau,\qquad\lambda_\pm=\frac{-1-r/2\pm i\sqrt3r/2}\tau}.
$$

The complex pair always has negative real part, and the real [eigenvalue](../../../../../../eigenvalue.md) is negative exactly when $r<1$. Therefore **strict linear asymptotic stability requires $\Gamma<1$**. The origin is unstable when $\Gamma>1$. A zero connection gives $\Gamma=0$ and all eigenvalues $-1/\tau$, also stable, though the matrix need not be diagonalizable.

At $\Gamma=1$, linearization has a simple zero eigenvalue, so a strict negative-real-part test alone does not settle nonlinear stability. For completeness, take a nonzero real eigenvector $c$ of the weighted loop matrix $M=\beta W$, satisfying $Mc=c$, and set $x_i=c_i u_i$. The local equations are

$$
\tau\dot u_i=-u_i+u_{i-1}-\tfrac13\beta^2c_{i-1}^2u_{i-1}^3+O(u_{i-1}^5).
$$

The center direction has all $u_i=a$. Averaging the three equations on the center manifold gives $\tau\dot a=-(\beta^2\sum_i c_i^2/9)a^3+O(a^5)$. Its leading coefficient is negative, while the other modes decay exponentially. Hence the exact boundary origin is locally asymptotically stable for the specified hyperbolic-tangent nonlinearity, with algebraic rather than exponential decay. This qualification distinguishes actual nonlinear stability from the usual strict Jacobian criterion.

## ↑ Ancestors (11)

1. [D](../d.md)
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
