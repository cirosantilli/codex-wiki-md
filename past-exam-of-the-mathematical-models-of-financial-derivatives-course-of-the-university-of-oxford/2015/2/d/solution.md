<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the [risk-neutral measure](../../../../risk-neutral-measure.md), set $a=\sigma\sqrt\tau$ and $m=\log(S/K)+(r-\sigma^2/2)\tau$. Then $\log(S_T/K)=m+aZ$ with $Z$ a [standard normal random variable](../../../../standard-normal-random-variable.md), and $d_-=m/a$. The [log-call option](../../../../log-call-option.md) is the discounted [Gaussian positive-part expectation](../../../../gaussian-positive-part-expectation.md):

$$
\begin{aligned}
V(S,t)&=e^{-r\tau}\int_{-d_-}^{\infty}(m+az)\phi(z)\,dz\\
&=e^{-r\tau}\bigl[m\Phi(d_-)+a\phi(d_-)\bigr],
\end{aligned}
$$

since $\phi'(z)=-z\phi(z)$. Therefore

$$
\boxed{V(S,t)=e^{-r\tau}\sigma\sqrt\tau
\left[d_-\operatorname N(d_-)+\frac{e^{-d_-^2/2}}{\sqrt{2\pi}}\right].}
$$

Here $\phi$ and $\Phi=\operatorname N$ are the [standard normal density](../../../../standard-normal-density.md) and [standard normal distribution function](../../../../standard-normal-distribution-function.md). At expiry the continuous terminal [limit](../../../../limit-of-a-function.md) is $(\log(S/K))^+$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
