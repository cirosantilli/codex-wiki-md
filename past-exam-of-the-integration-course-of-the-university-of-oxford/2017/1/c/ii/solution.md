<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) says that if measurable $f_n$ converge [almost everywhere](../../../../../almost-everywhere.md) to $f$ and $|f_n|\leq H$ almost everywhere for a single [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md) $H\geq0$, then $f$ is integrable and

$$
\int|f_n-f|\longrightarrow0,\qquad \int f_n\longrightarrow\int f.
$$

Here, for $x>0$, put $H_0(x)=x^{-1/2}e^{-x}$ and $f_n(x)=H_0(x)(1-(-1)^ne^{-nx})$. The [exponential function](../../../../../exponential-function.md) gives $e^{-nx}\to0$ at every such $x$, so $f_n\to H_0$. Also $|f_n(x)|\leq2H_0(x)$. This dominator is integrable: on $(0,1)$, $H_0(x)\leq x^{-1/2}$, whose integral is two; on $[1,\infty)$, $H_0(x)\leq e^{-x}$, whose integral is finite. DCT therefore proves the required limit.

The limiting value can also be evaluated. Substitute $x=t^2$ and use the [Gaussian integral](../../../../../gaussian-integral.md):

$$
\boxed{\lim_{n\to\infty}\int_0^\infty f_n(x)\,dx
=\int_0^\infty x^{-1/2}e^{-x}\,dx=\sqrt\pi.}
$$

In fact, scaling the second exponential term gives the exact integral $\sqrt\pi\,[1-(-1)^n/\sqrt{n+1}]$. The integral error decays as $n^{-1/2}$ despite exponential convergence at each fixed positive $x$; the slow part lies near the endpoint zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
