<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

For the real [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), multiply the equations for $y_n$ and $y_m$ by $y_m$ and $y_n$, respectively, and subtract. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
(\lambda_n-\lambda_m)\int_0^1wy_ny_mdx
=\left[p(y_ny_m'-y_my_n')\right]_0^1=0.
$$

The boundary term vanishes because both functions are zero at both endpoints. Distinct [eigenvalues](../../../../../eigenvalue.md) therefore imply weighted orthogonality. For equal indices the integral is the squared weighted norm, so

$$
\boxed{\int_0^1wy_ny_mdx=\delta_{nm}\int_0^1wy_n^2dx.}
$$

Let $c_n=\int_0^1wy_n^2dx>0$. For $y=\sum a_ny_n$ in the operator domain, with convergence sufficient to evaluate its quadratic energy, weighted orthogonality gives

$$
\int_0^1wy^2dx=\sum a_n^2c_n,\qquad
\int_0^1y\mathcal Ly\,dx=\sum\lambda_na_n^2c_n.
$$

For finite sums these identities follow immediately; the corresponding convergent energy expansion follows by approximation in the operator or quadratic-form domain. For nonzero $y$, the [Rayleigh quotient](../../../../../rayleigh-quotient.md) is a weighted average of the [eigenvalues](../../../../../eigenvalue.md), so

$$
\boxed{\frac{\int_0^1y\mathcal Ly\,dx}{\int_0^1wy^2dx}\ge\lambda_1.}
$$

Equality occurs precisely when only a lowest-eigenvalue component is present.

Assume completeness as permitted and take a sufficiently regular solution of the diffusion equation. It belongs to the weighted expansion space at each positive time; its modal coefficients satisfy $\dot a_n=-\lambda_na_n$. Alternatively differentiate its energy directly and use the preceding inequality:

$$
\boxed{\frac12\frac d{dt}\int_0^1wy^2dx
=\int_0^1wy\,y_tdx=-\int_0^1y\mathcal Ly\,dx
\le-\lambda_1\int_0^1wy^2dx.}
$$

Thus the squared weighted norm is at most its initial value times $e^{-2\lambda_1t}$. This describes decay when $\lambda_1>0$; positivity of $p,w$ alone does not require $\lambda_1>0$ if the potential $q$ can be negative. The displayed inequality remains valid regardless of that sign.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
