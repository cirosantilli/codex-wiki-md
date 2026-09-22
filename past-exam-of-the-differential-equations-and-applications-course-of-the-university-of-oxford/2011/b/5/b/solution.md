<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat u(k,t)=\int_{\mathbb R}e^{-ikx}u(x,t)\,dx$. Then the equation and [Dirac delta](../../../../../dirac-delta-function.md) initial condition become

$$
\partial_t\widehat u+(k^2+1)\widehat u=0,\qquad\widehat u(k,0)=1,
$$

so $\widehat u=e^{-(k^2+1)t}$. The [inverse Fourier transform](../../../../../inverse-fourier-transform.md) gives

$$
u(x,t)=\frac{e^{-t}}{2\pi}\int_{\mathbb R}e^{-tk^2+ikx}\,dk.
$$

Complete the square as $-tk^2+ikx=-t(k-ix/(2t))^2-x^2/(4t)$ and use the permitted complex-shift [Gaussian integral](../../../../../gaussian-integral.md). Thus the [heat kernel with constant absorption](../../../../../heat-kernel-with-constant-absorption.md) is

$$
\boxed{u(x,t)=\frac1{\sqrt{4\pi t}}\exp\left(-t-\frac{x^2}{4t}\right),\qquad t>0.}
$$

Its mass is $e^{-t}$, consistent with constant absorption, and it tends to the [Dirac delta](../../../../../dirac-delta-function.md) as a [distribution](../../../../../distribution-mathematical-analysis.md) as $t\downarrow0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
