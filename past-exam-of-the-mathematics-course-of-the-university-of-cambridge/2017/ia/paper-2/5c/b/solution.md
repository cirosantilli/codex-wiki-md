<h1 id="5c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The PDF gives $V=H(t)$, the [Heaviside step function](../../../../../../heaviside-step-function.md); the TeX incorrectly changes this to $V=I(t)$. A unit voltage step has derivative the [Dirac delta function](../../../../../../dirac-delta-function.md), so the current is the causal [Green function](../../../../../../green-s-function.md) for $L\,d^2/dt^2+R\,d/dt+1/C$.

The current must be continuous at zero: a jump would create a delta derivative through $LI''$, absent on the right-hand side. Integrating across zero therefore gives $L[I']+R[I]=1$, so $I(0^+)=0$ and $I'(0^+)=1/L$. Put

$$
r_\pm=\frac{-R\pm\sqrt{R^2-4L/C}}{2L}.
$$

These distinct negative [characteristic roots](../../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) give the [overdamped RLC response](../../../../../../overdamped-rlc-response.md)

$$
\boxed{I(t)=\frac{e^{r_+t}-e^{r_-t}}{L(r_+-r_-)}
=\frac{e^{r_+t}-e^{r_-t}}{\sqrt{R^2-4L/C}},\qquad t\geq0.}
$$

Together with $I(t)=0$ for $t<0$, this solves the step response. The eventual current is zero: the [capacitor](../../../../../../capacitor.md) charges and blocks steady current in the [series RLC circuit](../../../../../../series-rlc-circuit.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5C](../../5c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
