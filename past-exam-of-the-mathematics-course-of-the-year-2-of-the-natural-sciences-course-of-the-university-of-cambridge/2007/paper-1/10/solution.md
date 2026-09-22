<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

For a nonzero real [function](../../../../function-split.md), write $\Lambda=F/G$ with $G=\int_a^bw y^2dx>0$. Multiplying the [Sturm-Liouville equation](../../../../sturm-liouville-equation.md) by $y$ and integrating gives

$$
\lambda G=\int_a^b\bigl[p(y')^2+qy^2\bigr]dx-\left[pyy'\right]_a^b.
$$

Thus the stated vanishing boundary product proves $\lambda=\Lambda[y]$.

For the variational statement, the [first variation](../../../../first-variation.md) is

$$
\delta\Lambda=\frac2G\left\{\left[py'\eta\right]_a^b+\int_a^b\left[-(py')'+qy-\Lambda wy\right]\eta\,dx\right\}.
$$

With admissible [boundary conditions](../../../../boundary-condition.md) that also make $[py'\eta]_a^b=0$ for every allowed variation, the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) identifies stationary functions with the [eigenfunctions](../../../../eigenfunction.md) and stationary values with their [eigenvalues](../../../../eigenvalue.md). Zero [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), zero [Neumann boundary conditions](../../../../neumann-boundary-condition.md), and matched periodic data give familiar examples. The single printed condition $[pyy']_a^b=0$ proves the quotient identity but, by itself, does not specify the admissible variations needed for stationarity; the [boundary conditions for variational Rayleigh quotients](../../../../boundary-conditions-for-variational-rayleigh-quotients.md) make this distinction explicit.

For the half-line equation, multiplication by $x^{n-1}$ gives $p=w=x^{n-1}$ and $q=x^{n+1}$. Use the regular radial boundary condition at zero and square-integrable decay at infinity, under which the proposed Gaussian is admissible. With $y=e^{ax^2}$, $a<0$, $y'=2axy$, so

$$
\Lambda(a)=(4a^2+1)\frac{\int_0^\infty x^{n+1}e^{2ax^2}dx}{\int_0^\infty x^{n-1}e^{2ax^2}dx}=-n\left(a+\frac1{4a}\right).
$$

The ratio of the two [Gaussian integrals](../../../../gaussian-integral.md) is $n/(-4a)$, from a [change of variables](../../../../change-of-variables-formula.md) and the [Gamma function recurrence](../../../../gamma-function-recurrence.md). Differentiating gives $\Lambda'(a)=-n[1-1/(4a^2)]$, so the minimum on $a<0$ occurs at $a=-1/2$. The [Gaussian variational bound for a radial harmonic oscillator](../../../../gaussian-variational-bound-for-a-radial-harmonic-oscillator.md) therefore gives

$$
\boxed{\lambda_0\leq n,\qquad y_{\rm trial}=e^{-x^2/2}.}
$$

Here the trial actually satisfies the [differential equation](../../../../differential-equation-split.md) with $\lambda=n$. Moreover, on the same regular decaying domain, [integration by parts](../../../../integration-by-parts.md) gives $F[y]-nG[y]=\int_0^\infty x^{n-1}(y'+xy)^2dx\geq0$. Hence the estimate is exact, with $\boxed{\lambda_0=n}$. For $n=1$, regular radial data mean the [Neumann boundary condition](../../../../neumann-boundary-condition.md) $y'(0)=0$; imposing a zero [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) there would exclude this trial and give a different problem.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
