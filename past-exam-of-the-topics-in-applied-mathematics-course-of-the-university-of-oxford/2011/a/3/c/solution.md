<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The nonzero homogeneous equilibrium is $\boxed{n_*=1,\ a_*=\alpha/\beta}$. Without transport its [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
\begin{pmatrix}-1&0\\\alpha&-\beta\end{pmatrix},
$$

with negative [eigenvalues](../../../../../eigenvalue.md) $-1,-\beta$.

Zero chemical flux gives $a_x=0$ at the endpoints; zero bacterial flux then gives $n_x=0$. Linear perturbations therefore have [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) and modes $\cos(k_mx)$, $k_m=m\pi$. For each mode, the amplitude matrix is

$$
J_m=\begin{pmatrix}-1-D_nk_m^2&\chi k_m^2\\\alpha&-\beta-D_ak_m^2\end{pmatrix}.
$$

Its trace is always negative. Its [determinant](../../../../../determinant.md) is

$$
\boxed{\Delta(k)=D_nD_ak^4+(D_a+\beta D_n-\alpha\chi)k^2+\beta.}
$$

A mode grows exactly when $\Delta(k_m)<0$. In particular, any nonzero mode is destabilized by sufficiently large $\chi$. For continuously variable $k$, a nonempty unstable band exists precisely when

$$
\boxed{\alpha\chi>(\sqrt{D_a}+\sqrt{\beta D_n})^2.}
$$

Writing $C=\alpha\chi-D_a-\beta D_n$, its squared-wavenumber endpoints are $[C\pm\sqrt{C^2-4\beta D_nD_a}]/(2D_nD_a)$. On the finite interval, at least one allowed $k_m^2$ must lie inside this band. The uniform $m=0$ mode stays stable. This is the [chemotactic pattern-instability criterion](../../../../../chemotactic-pattern-instability-criterion.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
