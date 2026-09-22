<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For deterministic square-integrable [volatility](../../../../../financial-volatility.md), apply [Itô's formula](../../../../../ito-s-lemma.md) to the exponential to obtain

$$
\boxed{S_t=S_0\exp\left(\mu t-\tfrac12\int_0^t\sigma(u)^2du
+\int_0^t\sigma(u)dW_u\right).}
$$

The [stochastic integral](../../../../../stochastic-integral.md) is centered Gaussian with [variance](../../../../../variance-split.md) $\int_0^t\sigma(u)^2du$.

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md) the drift is $r$. Conditional on $S_t=s$, put $\tau=T-t$ and $v=\int_t^T\sigma(u)^2du$. Then

$$
S_T=s\exp(r\tau-v/2+\sqrt v\,Z),\qquad Z\sim N(0,1).
$$

Integrating the discounted [call option](../../../../../call-option.md) against this [normal distribution](../../../../../normal-distribution.md) yields

$$
\boxed{C(t,s)=s\Phi(d_1)-Ke^{-r\tau}\Phi(d_2),}
$$



$$
d_1=\frac{\log(s/K)+r\tau+v/2}{\sqrt v},
\qquad d_2=d_1-\sqrt v.
$$

Thus the total remaining [variance](../../../../../variance-split.md) replaces $\sigma^2\tau$ throughout the ordinary formula; the corresponding effective constant [volatility](../../../../../financial-volatility.md) is $\sqrt{v/\tau}$. If $v=0$, use the limiting deterministic value $(s-Ke^{-r\tau})_+$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
