<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

Differentiate the [Friedmann equation](../../../../../friedmann-equations.md) and use the [cosmological continuity equation](../../../../../cosmological-continuity-equation.md) to obtain $\dot H+H^2=-(4\pi G/3)(\rho+3P/c^2)$. The relation extends to turning points by continuity. Radiation obeys $\rho_R=\rho_{R0}a^{-4}$, while [dark energy](../../../../../dark-energy.md) with $P_\Lambda=-\rho_\Lambda c^2$ has constant density. Substitution at $a(t_0)=1$ gives $kc^2=\beta H_0^2$, and at arbitrary $a$ gives

$$
H^2=H_0^2\frac{a^4-\beta a^2+\beta}{a^4},\qquad
\dot H=-\beta H_0^2\frac{2-a^2}{a^4}.
$$

Put $x=a^2$. For $\beta>4$, the upward-opening polynomial $P(x)=x^2-\beta x+\beta$ has roots $x_\pm=(\beta\pm\sqrt{\beta(\beta-4)})/2$, with $1<x_-<2<x_+$. The expanding [Big Bang](../../../../../big-bang.md) branch reaches $x_-$ in finite time. There $H=0$ but $\dot H<0$, so expansion turns to contraction; it returns to $a=0$ in finite time, a [Big Crunch](../../../../../big-crunch.md). A sketch of $a^4H^2/H_0^2=P(x)$ has the forbidden negative interval between the roots, while $a^4\dot H/H_0^2=\beta(x-2)$ is a line crossing zero at two.

For $\beta=4$, $P(x)=(x-2)^2$. The branch starting at zero has $\dot x=2H_0(2-x)$, giving

$$
\boxed{a(t)=\sqrt{2(1-e^{-2H_0t})}.}
$$

At small $t$, $a\sim2\sqrt{H_0t}$, the radiation-dominated [scale factor](../../../../../scale-factor-cosmology.md). At large $t$, $a=\sqrt2[1-\tfrac12e^{-2H_0t}+O(e^{-4H_0t})]$. It approaches an [Einstein static universe](../../../../../einstein-static-universe.md) with equal radiation and dark-energy densities, rather than recollapsing or entering unbounded expansion.

<a id="15a/image-radiation-lambda-turning-points-and-the-critical-scale-factor"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1-radiation-lambda.png)

**[Figure 1](#15a/image-radiation-lambda-turning-points-and-the-critical-scale-factor). Radiation–Lambda turning points and the critical scale factor**.

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
