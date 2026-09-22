<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider the counterclockwise [unit circle](../../../../complex-unit-circle.md) and set

$$
I=\frac1{2\pi i}\int_{|z|=1}z^{n-1}e^{-xz/2}e^{x/(2z)}\,dz.
$$

The parametrization $z=e^{i\theta}$ gives

$$
I=\frac1{2\pi}\int_0^{2\pi}e^{i(n\theta-x\sin\theta)}\,d\theta.
$$

The [imaginary part](../../../../imaginary-part.md) is zero: replacing $\theta$ by $2\pi-\theta$ conjugates the integrand, since $n$ is an integer and $x$ is real. The [real part](../../../../real-part.md) is precisely the defining Bessel integral, so $I=J_n(x)$.

Both exponential series converge absolutely and uniformly on the [circle](../../../../circle.md). Their product may therefore be integrated term by term:

$$
z^{n-1}e^{-xz/2}e^{x/(2z)}
=\sum_{j,k\geq0}\frac{(-1)^j(x/2)^{j+k}}{j!k!}z^{n-1+j-k}.
$$

Uniform [absolute convergence](../../../../absolute-convergence.md) can also be checked by summing the absolute coefficient bounds, which gives $e^{|x|}$. The [residue](../../../../residue.md) is obtained exactly when $n-1+j-k=-1$, or $k=n+j$. The [Cauchy coefficient formula](../../../../cauchy-coefficient-formula.md) consequently yields

$$
\boxed{J_n(x)=\sum_{j=0}^{\infty}\frac{(-1)^j}{j!(n+j)!}\left(\frac x2\right)^{n+2j},\qquad n\geq0.}
$$

This proves the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md) series directly from its integral, including the sign and [factorial](../../../../factorial.md) normalization.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
