<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [function](../../../../../function-split.md) is not [Lebesgue integrable](../../../../../lebesgue-integrable-function.md).** Fix $0<\eta<\pi/2$ and restrict to $x\geq1$, $0<y<\eta$. There $\cos y\geq\cos\eta>0$. [Tonelli's theorem](../../../../../tonelli-theorem.md) for the nonnegative absolute value gives the lower bound

$$
\begin{aligned}
\iint|g(x,y)|\,dx\,dy
&\geq\cos\eta\int_1^\infty|\cos2x|\int_0^\eta e^{-xy}\,dy\,dx\\
&=\cos\eta\int_1^\infty|\cos2x|\frac{1-e^{-\eta x}}x\,dx\\
&\geq\cos\eta(1-e^{-\eta})\int_1^\infty\frac{|\cos2x|}x\,dx.
\end{aligned}
$$

The last integral diverges. Indeed, on $[k\pi,k\pi+\pi/6]$, $|\cos2x|\geq1/2$; each such interval contributes at least a positive constant times $1/(k+1)$. The [harmonic series](../../../../../harmonic-series.md) diverges. Hence the integral of $|g|$ is infinite, regardless of possible signed cancellations. One cannot infer [Lebesgue integrability](../../../../../integrability.md) by formally applying [Fubini's theorem](../../../../../fubini-s-theorem.md) to the oscillatory integrand.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
