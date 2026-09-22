<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the candidate potential by convolving the decaying [Green function](../../../../../../green-s-function-split.md) with the source. Acting with the [Laplacian](../../../../../../laplacian.md) in the observation variable gives, in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md),

$$
\begin{aligned}
\nabla_{\mathbf r}^2\int_{\mathbb R^3}G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3r'
&=-\int_{\mathbb R^3}\delta^{(3)}(\mathbf r-\mathbf r')\rho(\mathbf r')\,d^3r'\\
&=-\rho(\mathbf r).
\end{aligned}
$$

The final equality is the sifting property of the [Dirac delta](../../../../../../dirac-delta-function.md). The kernel found in part (ii) is locally [integrable](../../../../../../integrability.md), and its convolution with a sufficiently regular rapidly decaying source also vanishes at spatial infinity. Thus it satisfies the [Poisson equation](../../../../../../poisson-s-equation.md) and the required condition at infinity.

The difference from any other regular decaying solution is a [harmonic function](../../../../../../harmonic-function.md) on all of space vanishing at infinity, hence is zero by the [maximum principle](../../../../../../maximum-principle.md). Therefore

$$
\boxed{\phi(\mathbf r)=\int_{\mathbb R^3}G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3r'.}
$$

One can also obtain this expression from [Green's second identity](../../../../../../green-second-identity.md) on larger and larger balls, with the singularity of the kernel treated distributionally. The surface term at infinity vanishes for the usual $1/r$ potential decay and $1/r^2$ gradient decay.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
