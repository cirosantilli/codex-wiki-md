<h1 id="a/2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $0<\epsilon<\pi/2$. On $[\epsilon,\pi/2]$, $\sin^2t\geq\sin^2\epsilon>0$, so that part of the integral is bounded by $(\pi/2)e^{-x\sin^2\epsilon}$, exponentially smaller than $x^{-1/2}$.

By the assumed local equivalence, the remaining part is asymptotic to $\int_0^\epsilon e^{-xt^2}dt$. Substitute $s=\sqrt x\,t$:

$$
\int_0^\epsilon e^{-xt^2}dt=x^{-1/2}\int_0^{\epsilon\sqrt x}e^{-s^2}ds
\sim\frac{\sqrt\pi}{2\sqrt x}.
$$

The last step uses the [Gaussian integral](../../../../../gaussian-integral.md) and monotone convergence of the upper limit to infinity. Hence

$$
\boxed{\int_0^{\pi/2}e^{-x\sin^2t}dt\sim\tfrac12\sqrt{\pi/x}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
