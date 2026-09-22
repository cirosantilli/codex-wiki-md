<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [spectral theorem for compact self-adjoint operators](../../../../spectral-theorem-for-compact-hermitian-operators.md) used here concerns a compact [self-adjoint operator](../../../../self-adjoint-operator.md): its nonzero [eigenvalues](../../../../eigenvalue.md) are real, have finite multiplicity and can accumulate only at zero; the orthogonal complement of its kernel is the closed span of its orthonormal eigenvectors. Self-adjointness is essential for this eigenbasis statement.

Let $Kf$ be the unique zero-parameter [weak solution](../../../../weak-solution.md). Uniqueness gives linearity. Testing with $Kf$ and using coercivity gives $\|Kf\|_{H^1}\leq\nu^{-1}\|f\|_2$. The [Rellich-Kondrachov theorem](../../../../rellich-kondrachov-theorem.md) makes the embedding $H_0^1(\Omega)\hookrightarrow L^2(\Omega)$ compact on this bounded $C^1$ domain, so $K$ is compact on $L^2$. Symmetry gives

$$
\langle Kf,g\rangle=B[Kg,Kf]=\langle f,Kg\rangle.
$$

It is self-adjoint and positive. It is injective: if $Kf=0$, the weak equation pairs $f$ to zero with all $H_0^1$ tests, dense in $L^2$, so $f=0$. Moreover $\langle Kf,f\rangle=B[Kf,Kf]>0$ for $f\ne0$.

The parameter equation is equivalent to $u=K(f+\lambda u)$, that is

$$
\boxed{u-\lambda Ku=Kf.}
$$

A solution of this operator equation in $L^2$ lies in $H_0^1$, because its right-side representation is $K(f+\lambda u)$, and the equivalence follows in both directions. For $\lambda\leq0$, the form $B[u,v]-\lambda\langle u,v\rangle$ remains coercive; the preceding minimization argument gives a unique [weak solution](../../../../weak-solution.md).

The [spectral theorem](../../../../spectral-theorem.md) now supplies a complete [orthonormal basis](../../../../orthonormal-basis.md) $(\phi_j)$ of $L^2$ with $K\phi_j=\kappa_j\phi_j$, $\kappa_j>0$, and $\kappa_j\to0$. The elliptic [eigenvalues](../../../../eigenvalue.md) are $\lambda_j=1/\kappa_j>0$, with finite multiplicity and tending to infinity, and $L\phi_j=\lambda_j\phi_j$ weakly. If $\lambda$ is not one of them, then

$$
\boxed{u=\sum_j\frac{\langle f,\phi_j\rangle}{\lambda_j-\lambda}\phi_j.}
$$

This converges even in $H_0^1$: its squared energy [norm](../../../../norm.md) is $\sum_j\lambda_j|\langle f,\phi_j\rangle|^2/|\lambda_j-\lambda|^2$, finite because the multiplier is bounded over $j$. Partial sums solve the weak equation with the corresponding $L^2$ projections of $f$. Passing to the limit proves the equation for every test; the same coefficients force uniqueness. Thus the expansion represents **the unique [weak solution](../../../../weak-solution.md) away from the elliptic [eigenvalues](../../../../eigenvalue.md)**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
