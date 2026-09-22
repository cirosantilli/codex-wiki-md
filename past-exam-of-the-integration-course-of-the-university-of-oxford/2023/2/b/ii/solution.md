<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $h(t,x)=e^{-x^2-t^2/x^2}$. For every $t\geq0$, $0<h(t,x)\leq e^{-x^2}$, and the upper bound is a [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md) by part (b)(i). Since $h(t,x)\to e^{-x^2}$ for each $x>0$ as $t\downarrow0$, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives right [continuity](../../../../../continuous-function.md) at zero and

$$
F(0)=\lim_{t\downarrow0}F(t)=\frac{\sqrt\pi}{2}.
$$

To apply [dominated differentiation under the integral sign](../../../../../dominated-differentiation-under-the-integral-sign.md), fix $t_0>0$ and restrict $t$ to $[t_0/2,3t_0/2]$. Then

$$
|\partial_t h(t,x)|=\frac{2t}{x^2}e^{-x^2-t^2/x^2}
\leq D(x):=3t_0x^{-2}e^{-x^2-t_0^2/(4x^2)}.
$$

For $x\geq1$, $D(x)\leq3t_0e^{-x^2}$. For $0<x<1$, writing $a=t_0^2/4>0$, the [substitution rule](../../../../../integration-by-substitution.md) $u=1/x$ gives

$$
\int_0^1x^{-2}e^{-a/x^2}\,dx=\int_1^\infty e^{-au^2}\,du<\infty.
$$

Thus $D$ is integrable. The [mean value theorem](../../../../../mean-value-theorem.md) bounds nearby difference quotients by $D$, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) justifies the derivative at $t_0$. As $t_0$ was arbitrary,

$$
F'(t)=-2t\int_0^\infty x^{-2}e^{-x^2-t^2/x^2}\,dx,\qquad t>0.
$$

Now make the [change of variables](../../../../../change-of-variables-formula.md) $u=t/x$. The reversal of limits cancels the negative differential and gives

$$
\int_0^\infty x^{-2}e^{-x^2-t^2/x^2}\,dx
=\frac1t\int_0^\infty e^{-u^2-t^2/u^2}\,du=\frac{F(t)}t.
$$

Consequently $F'(t)=-2F(t)$. This also follows in sign from the fact that the positive integrand decreases strictly as $t$ increases: the printed equation with a positive sign cannot hold. Solving the [linear differential equation](../../../../../linear-differential-equation.md), or differentiating $e^{2t}F(t)$, and using right [continuity](../../../../../continuous-function.md) at zero gives

$$
\boxed{F'(t)=-2F(t)\ (t>0),\qquad F(t)=\frac{\sqrt\pi}{2}e^{-2t}\ (t\geq0).}
$$

This is a half-line instance of the [Gaussian integral with an inverse-square term](../../../../../gaussian-integral-with-an-inverse-square-term.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
