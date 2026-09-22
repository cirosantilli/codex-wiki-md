<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $y\ne0$. The [function](../../../../function-split.md) $x\mapsto f(x,y)$ is continuous on $[-1,1]$, because its denominator is bounded away from zero, and it is an [odd function](../../../../odd-function.md) of $x$. Its [integral](../../../../integral-split.md) over this symmetric [interval](../../../../interval-mathematics.md) is therefore zero. At $y=0$ the entire section is zero, including the specified value at the origin. Thus the inner $x$ [integral](../../../../integral-split.md) exists for every $y$ and is identically zero. The same reasoning with $x$ and $y$ exchanged gives

$$
\boxed{\int_{-1}^1\left(\int_{-1}^1f(x,y)\,dx\right)dy
=\int_{-1}^1\left(\int_{-1}^1f(x,y)\,dy\right)dx=0.}
$$

To test [Lebesgue integrability](../../../../integrability.md) in two dimensions, examine the [absolute value](../../../../absolute-value.md) near the origin. For $0<\varepsilon<1$, the annulus $\varepsilon<\sqrt{x^2+y^2}<1$ lies inside the square. In [polar coordinates](../../../../polar-coordinates.md),

$$
|f(r\cos\theta,r\sin\theta)|=\frac{|\cos\theta\sin\theta|}{r^4},\qquad dx\,dy=r\,dr\,d\theta.
$$

The [change of variables formula](../../../../change-of-variables-formula.md) on this annulus, where the [integrand](../../../../integrand.md) has no singularity, gives

$$
\begin{aligned}
\int_{[-1,1]^2}|f(x,y)|\,dx\,dy
&\geq\int_\varepsilon^1r^{-3}\,dr\int_0^{2\pi}|\cos\theta\sin\theta|\,d\theta\\
&=\frac{\varepsilon^{-2}-1}{2}\cdot2
=\varepsilon^{-2}-1.
\end{aligned}
$$

The lower bound tends to infinity as $\varepsilon\downarrow0$. Hence

$$
\boxed{\int_{[-1,1]^2}|f|=\infty,\qquad f\notin L^1([-1,1]^2).}
$$

Moreover reflection in either coordinate axis exchanges the [positive part](../../../../positive-part-of-a-real-valued-function.md) and [negative part](../../../../negative-part-of-a-real-valued-function.md) while preserving [Lebesgue measure](../../../../lebesgue-measure.md). Both parts therefore have infinite [integral](../../../../integral-split.md), so a signed double [Lebesgue integral](../../../../lebesgue-integral.md) would involve the undefined expression $\infty-\infty$.

There is no contradiction with [Fubini's theorem](../../../../fubini-s-theorem.md): its [absolute integrability](../../../../integrability.md) hypothesis is missing. This is an example of [finite iterated integrals without joint integrability](../../../../finite-iterated-integrals-without-joint-integrability.md), with every individual one-dimensional section integrable despite the two-dimensional singularity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
