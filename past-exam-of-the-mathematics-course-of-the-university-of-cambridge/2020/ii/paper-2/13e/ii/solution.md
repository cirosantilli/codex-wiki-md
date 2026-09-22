<h1 id="13e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $f(t)=\sin\omega t$,

$$
\widehat f(p)=\frac{\omega}{p^2+\omega^2},
\qquad
\widehat y(x,p)=\frac{\omega e^{-px/c}}{p^2+\omega^2}.
$$

The [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md) gives

$$
y(x,t)=\frac{1}{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}
\frac{\omega e^{p(t-x/c)}}{p^2+\omega^2}\,dp.
$$

When $t>x/c$, close the contour to the left. The residues at $p=\pm i\omega$ sum to $\sin(\omega(t-x/c))$. When $t<x/c$, close it to the right, where there are no poles, and the integral vanishes. Hence

$$
\boxed{y(x,t)=
\begin{cases}
0,&t<x/c,\\
\sin\!\bigl(\omega(t-x/c)\bigr),&t\ge x/c.
\end{cases}}
$$

Equivalently, $y(x,t)=\Theta(t-x/c)\sin(\omega(t-x/c))$ in terms of the [Heaviside step function](../../../../../../heaviside-step-function.md). The boundary oscillation travels to the right at [wave speed](../../../../../../wave-speed.md) $c$ without reflection or dispersion; a point at $x$ begins moving after the propagation delay $x/c$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
