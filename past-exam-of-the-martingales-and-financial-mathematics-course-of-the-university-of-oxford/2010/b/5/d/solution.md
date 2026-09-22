<h1 id="b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\tau=T-t$. Conditional on present information, $J=\int_t^T(W_u-W_t)du$ is independent of the past and is normal with mean zero and variance $\tau^3/3$. Part (c) gives

$$
\widetilde A_T^2=A_t^{2t/T}S_t^{2\tau/T}
\exp\left[(r-\sigma^2/2)\frac{\tau^2}{T}+\frac{2\sigma}{T}J\right].
$$

The future drift $r$ in this auxiliary stock is precisely the risk-neutral drift. Discounting the conditional expectation and applying the normal exponential-moment formula yields

$$
\boxed{V^A(t,S_t,A_t)=e^{-r\tau}A_t^{2t/T}S_t^{2\tau/T}
\exp\left[\left(r-\frac{\sigma^2}{2}\right)\frac{\tau^2}{T}
+\frac{2\sigma^2\tau^3}{3T^2}\right].}
$$

At expiry this reduces to $A_T^2$; at time zero it gives $S_0^2e^{\sigma^2T/6}$. This is a special case of [conditional power moments of a continuous geometric Asian average](../../../../../conditional-power-moments-of-a-continuous-geometric-asian-average.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
