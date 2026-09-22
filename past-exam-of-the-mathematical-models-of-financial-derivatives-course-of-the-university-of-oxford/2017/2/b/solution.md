<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the [risk-neutral measure](../../../../risk-neutral-measure.md), write $Z\sim N(0,1)$, $a=\sigma\sqrt\tau$, and $m=\log(S/K)+(r-\sigma^2/2)\tau$. Then $\log(S_T/K)=m+aZ$ and $d_-=m/a$. By [risk-neutral pricing](../../../../risk-neutral-pricing.md), this [log-call option](../../../../log-call-option.md) has value $e^{-r\tau}\mathbb E[(m+aZ)^+]$.

Let $\phi$ and $\Phi$ denote the [standard normal density](../../../../standard-normal-density.md) and [standard normal distribution function](../../../../standard-normal-distribution-function.md). The [Gaussian positive-part expectation](../../../../gaussian-positive-part-expectation.md) follows by integration:

$$
\mathbb E[(m+aZ)^+]
=\int_{-d_-}^{\infty}(m+az)\phi(z)\,dz
=m\Phi(d_-)+a\phi(d_-),
$$

because $\phi'(z)=-z\phi(z)$. Therefore

$$
\boxed{V(S,t)=e^{-r\tau}\sigma\sqrt\tau
\left[d_-\Phi(d_-)+\frac{e^{-d_-^2/2}}{\sqrt{2\pi}}\right],\qquad
d_-=\frac{\log(S/K)+(r-\sigma^2/2)\tau}{\sigma\sqrt\tau}.}
$$

For $\tau=0$ take the continuous terminal [limit](../../../../limit-of-a-function.md) $(\log(S/K))^+$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
