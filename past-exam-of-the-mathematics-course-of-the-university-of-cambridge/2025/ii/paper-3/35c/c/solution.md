<h1 id="35c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the chemical potential at its zero-temperature value $\mu=E_F$ and put $E'=E-E_F$. Away from $E'=0$,

$$
f(E)-\mathbf1_{E<E_F}
=\frac12\left[\operatorname{sgn}\!\left(\frac{\beta E'}2\right)
-\tanh\!\left(\frac{\beta E'}2\right)\right].
$$

Consequently

$$
\Delta N
=X\int_{-E_F}^{\infty}
\left[\operatorname{sgn}\!\left(\frac{\beta E'}2\right)
-\tanh\!\left(\frac{\beta E'}2\right)\right]dE',
$$

where

$$
\boxed{X=\frac g2=\frac{Am}{2\pi\hbar^2}}.
$$

The bracket is an odd function localized to $|E'|\lesssim k_BT$. When $\beta E_F\gg1$, extending the lower limit to $-\infty$ makes the integral vanish exactly. The omitted tail is exponentially small; indeed direct integration gives

$$
\Delta N=\frac g\beta\log(1+e^{-\beta E_F}).
$$

This is the [low-temperature particle-number cancellation for constant density of states](../../../../../../low-temperature-particle-number-cancellation-for-constant-density-of-states.md).

For the energy,

$$
\begin{aligned}
\Delta E_{\rm tot}
&=g\int_{-E_F}^{\infty}(E_F+E')
\bigl[f(E_F+E')-\mathbf1_{E'<0}\bigr]dE'\\
&=E_F\Delta N
+X\int_{-E_F}^{\infty}E'
\left[\operatorname{sgn}\!\left(\frac{\beta E'}2\right)
-\tanh\!\left(\frac{\beta E'}2\right)\right]dE'.
\end{aligned}
$$

At low temperature the first term is exponentially small. In the second, extend the lower limit to $-\infty$ and set $z=\beta E'/2$:

$$
\Delta E_{\rm tot}
\sim\frac{4X}{\beta^2}
\int_{-\infty}^{\infty}z[\operatorname{sgn}(z)-\tanh z]\,dz.
$$

The remaining integral is a finite positive constant, proving the [quadratic low-temperature energy correction for constant density of states](../../../../../../quadratic-low-temperature-energy-correction-for-constant-density-of-states.md):

$$
\boxed{\Delta E_{\rm tot}\propto\beta^{-2}\propto T^2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [35C](../../35c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
