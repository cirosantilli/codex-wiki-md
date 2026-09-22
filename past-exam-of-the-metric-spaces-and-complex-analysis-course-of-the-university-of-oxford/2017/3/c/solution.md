<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the real interval, $h(x)$ is real and $H(x)=h(x)^2\geq0$. Expanding and integrating the finite sum yields

$$
\sum_{r,s=1}^n\frac{a_ra_s}{r+s+1}=\int_0^1h(x)^2\,dx.
$$

Apply part (b)(iv) to the entire function $H=h^2$. Since $|H(e^{i\theta})|=|h(e^{i\theta})|^2$, [orthogonality of complex exponentials](../../../../orthogonality-of-complex-exponentials.md) gives

$$
\int_0^{2\pi}|h(e^{i\theta})|^2\,d\theta=\sum_{r,s}a_ra_s\int_0^{2\pi}e^{i(r-s)\theta}\,d\theta=2\pi\sum_{r=1}^n a_r^2.
$$

Consequently

$$
\boxed{\left|\sum_{r,s=1}^n\frac{a_ra_s}{r+s+1}\right|\leq\pi\sum_{r=1}^n a_r^2.}
$$

The quadratic form is actually nonnegative, so its absolute value can be dropped. This [shifted Hilbert quadratic-form bound](../../../../shifted-hilbert-quadratic-form-bound.md) comes from combining the logarithmic contour estimate with a finite [Parseval identity](../../../../parseval-identity.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
