<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the two sine modes, [orthogonality](../../../../../orthogonal-vectors.md) gives

$$
\int_0^1\widetilde\psi^2dx=\frac{1+\alpha^2}{2},\qquad\int_0^1\widetilde\psi'^2dx=\frac{\pi^2}{2}(1+4\alpha^2).
$$

The diagonal potential integrals vanish, while the mixed one is

$$
\int_0^1\sin(\pi x)\sin(2\pi x)\cos(\pi x)dx=\frac14.
$$

Thus $\int_0^1\cos(\pi x)\widetilde\psi^2dx=\alpha/2$, giving the [two-sine variational bound for a Dirichlet Mathieu equation](../../../../../two-sine-variational-bound-for-a-dirichlet-mathieu-equation.md):

$$
\boxed{R(\alpha)=\frac{\pi^2+\alpha+4\pi^2\alpha^2}{1+\alpha^2}.}
$$

Its [derivative](../../../../../derivative.md) vanishes when $1+6\pi^2\alpha-\alpha^2=0$. Hence the two stationary parameters are $3\pi^2\pm\sqrt{9\pi^4+1}$. To identify the minimum, use the normalized sine basis: the restricted [self-adjoint operator](../../../../../self-adjoint-operator.md) has real [symmetric matrix](../../../../../symmetric-matrix.md)

$$
H_{\mathrm{trial}}=\begin{pmatrix}\pi^2&1/2\\1/2&4\pi^2\end{pmatrix}.
$$

Its smaller [eigenvalue](../../../../../eigenvalue.md) is the minimum of the [Rayleigh quotient](../../../../../rayleigh-quotient.md), attained at the negative stationary parameter. Therefore

$$
\boxed{\alpha_{\mathrm{opt}}=3\pi^2-\sqrt{9\pi^4+1},\qquad\lambda_0\leq\frac{5\pi^2-\sqrt{9\pi^4+1}}2\approx9.86116.}
$$

The estimate improves on the single-sine value $\pi^2$. The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) remains valid here even though $q(x)=\cos(\pi x)$ changes sign: on this finite interval the [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) is self-adjoint and bounded below, which is sufficient for the upper bound.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
