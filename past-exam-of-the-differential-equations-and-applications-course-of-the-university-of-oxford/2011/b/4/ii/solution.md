<h1 id="b/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the moving stretched coordinates, $\partial_t=\partial_\tau-s'(\tau)\varepsilon^{-1}\partial_\xi$ and $\partial_x=\varepsilon^{-1}\partial_\xi$. Multiplying the [damped Burgers equation](../../../../../damped-burgers-equation.md) by $\varepsilon$ gives

$$
\varepsilon(u_\tau+u)+(u-s')u_\xi=u_{\xi\xi}.
$$

Discarding the order-$\varepsilon$ terms yields the leading [Viscous Burgers travelling shock](../../../../../viscous-burgers-travelling-shock.md) equation $\boxed{(u-s')u_\xi=u_{\xi\xi}}$. Integrate across a nonconstant transition whose derivative vanishes at either end:

$$
\boxed{\left[\frac{u^2}{2}-s'u\right]_-^+=0.}
$$

Multiplication by $u$ and a further [integration by parts](../../../../../integration-by-parts.md) give

$$
\boxed{\left[\frac{u^3}{3}-\frac{s'u^2}{2}\right]_-^+=-\int_{-\infty}^{\infty}u_\xi^2\,d\xi<0.}
$$

The first identity is the [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md), giving $s'=(u_-+u_+)/2$. Substitution into the second makes its left side $(u_+-u_-)^3/12$, so the viscosity-selected [entropy shock](../../../../../entropy-shock.md) has $u_->u_+$.

After the first characteristic collapse, the shock is fed by the left constant initial state and the right zero state. Their damped values are $u_-=2e^{-\tau}$ and $u_+=0$. Therefore $s'=e^{-\tau}$. Matching to $s(\log2)=0$ yields

$$
\boxed{s(\tau)=\frac12-e^{-\tau},\qquad\tau>\log2.}
$$

These matching states are consistent with the characteristic feet: the left foot is $s-2(1-e^{-\tau})=-3/2+e^{-\tau}<-1$, while the right foot is $s>0$. The formula describes the leading thin-layer position in the small-viscosity limit.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
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
