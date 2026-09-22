<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the standard regular self-adjoint assumptions on the [Sturm-Liouville problem](../../../../sturm-liouville-problem.md), including positive weight $w$. The normalized [eigenfunctions](../../../../eigenfunction.md) obey [orthogonality](../../../../orthogonal-vectors.md)

$$
\int_a^bw(x)y_m(x)^*y_n(x)dx=\delta_{mn}.
$$

Completeness means every function in the weighted $L^2$ space has expansion $f(x)=\sum_ny_n(x)\int_a^bw(\xi)y_n(\xi)^*f(\xi)d\xi$, with convergence in that space. Comparing the action of this kernel on test functions with the [Dirac delta](../../../../dirac-delta-function.md) gives, in the distributional sense,

$$
\boxed{w(\xi)\sum_{n=1}^\infty y_n(\xi)^*y_n(x)=\delta(x-\xi).}
$$

If zero is not an [eigenvalue](../../../../eigenvalue.md), divide each term by $\lambda_n$. Since $Ly_n=\lambda_ny_n$, application of $L$ recovers the displayed delta expansion, proving

$$
\boxed{G(x;\xi)=w(\xi)\sum_{n=1}^\infty\frac{y_n(x)y_n(\xi)^*}{\lambda_n}.}
$$

The factor $w(\xi)$ is required because the source equation uses an ordinary, unweighted delta. It distinguishes the [normalized Sturm-Liouville spectral Green kernel](../../../../normalized-sturm-liouville-spectral-green-kernel.md) from a kernel integrated against weighted source measure. If there is a zero [eigenvalue](../../../../eigenvalue.md), an inverse for arbitrary forcing does not exist; the unqualified division by that [eigenvalue](../../../../eigenvalue.md) is invalid.

For $L=-d^2/dx^2+\omega^2$ with real $\omega$ and zero endpoints on $[0,1]$, the weight is one, $y_n=\sqrt2\sin(n\pi x)$ and $\lambda_n=n^2\pi^2+\omega^2>0$. Substitution yields

$$
\boxed{G(x;\xi)=\sum_{n=1}^\infty\frac{2\sin(n\pi\xi)\sin(n\pi x)}{n^2\pi^2+\omega^2}.}
$$

The series is absolutely and uniformly convergent, although applying the differential operator is understood distributionally at its source point.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
