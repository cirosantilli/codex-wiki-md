<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

For example, impose homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) $y(a)=y(b)=0$, and use variations vanishing there. Homogeneous [Neumann boundary conditions](../../../../neumann-boundary-condition.md) $py'=0$ are another choice removing the boundary terms. Put $N[y]=\int_a^b(py'^2+qy^2)dx$, $D[y]=\int_a^bwy^2dx>0$, and $I=N/D$. At a stationary function let $\lambda=I[y]$. The quotient rule gives $\delta I=(\delta N-\lambda\delta D)/D$. After [integration by parts](../../../../integration-by-parts.md), stationarity under every allowed variation gives

$$
0=\int_a^b[-(py')'+qy-\lambda wy]\eta\,dx,
$$

so the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields the stated [Sturm-Liouville problem](../../../../sturm-liouville-problem.md). Conversely an eigenfunction with those boundary conditions has $N=\lambda D$ and makes the quotient stationary. The lowest eigenvalue minimizes the [Rayleigh quotient](../../../../rayleigh-quotient.md) under the usual self-adjoint, lower-bounded hypotheses; higher eigenvalues are stationary values with orthogonality constraints when minimizing successively.

The hydrogen equation becomes $-(r^2\psi')'-2r\psi=2Er^2\psi$. Its radial energy quotient is therefore

$$
E[\psi]=\frac{\int_0^\infty[r^2\psi'^2-2r\psi^2]dr}{2\int_0^\infty r^2\psi^2dr}.
$$

Regularity at zero and decay at infinity remove the boundary term $r^2\psi\psi'$. The condition $\psi(0)=1$ fixes an arbitrary amplitude for these trial functions; it is not their three-dimensional probability normalization, which cancels from the quotient.

For $\psi=e^{-\alpha r}$, elementary exponential integrals give $\int r^2\psi^2dr=1/(4\alpha^3)$, $\int r^2\psi'^2dr=1/(4\alpha)$, and $\int r\psi^2dr=1/(4\alpha^2)$. Hence

$$
E(\alpha)=\frac{\alpha^2}{2}-\alpha=\frac12(\alpha-1)^2-\frac12,\qquad\boxed{\alpha=1,\quad E_{\exp}=-\frac12.}
$$

For the [compactly supported linear trial for hydrogen](../../../../compactly-supported-linear-trial-for-hydrogen.md), the norm, gradient and Coulomb integrals are $\beta^3/30$, $\beta/3$, and $\beta^2/12$, respectively. Thus

$$
E(\beta)=\frac5{\beta^2}-\frac5{2\beta},\qquad E'(\beta)=\frac{5(\beta-4)}{2\beta^3},\qquad\boxed{\beta=4,\quad E_{\mathrm{linear}}=-\frac5{16}.}
$$

The derivative changes from negative to positive at four, so this is the minimum over positive $\beta$. The [quantum variational principle](../../../../quantum-variational-principle.md) gives upper bounds on the [ground-state energy](../../../../ground-state-energy.md); **the exponential trial is better**, and in fact $e^{-r}$ satisfies the exact differential equation at $E=-1/2$. It is the nodeless hydrogen ground state in the given units. The linear trial is admissible for the energy quadratic form despite its derivative jump at $r=\beta$; it need not possess a classical second derivative at that point.

<a id="10/image-variational-energy-curves-for-exponential-and-compact-linear-hydrogen-trials"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1-hydrogen-variational-trials.png)

**[Figure 2](#10/image-variational-energy-curves-for-exponential-and-compact-linear-hydrogen-trials). Variational energy curves for exponential and compact linear hydrogen trials**. Original energy curves in the equation's atomic units. The exponential family reaches the exact ground-state energy, while the best compact linear trial remains above it.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
