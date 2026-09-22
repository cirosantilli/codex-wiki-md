<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Laplace transform.** Use $Y(p)=\int_0^\infty e^{-pt}y(t)dt$. The initial value is zero and the [Dirac delta](../../../../dirac-delta-function.md) contributes $e^{-p}$, so the transformed equation is $pY+Y=e^{-p}$. Therefore

$$
\boxed{Y(p)=\frac{e^{-p}}{p+1},\qquad\operatorname{Re}p>-1.}
$$

**Bromwich inversion.** The [Bromwich inversion formula](../../../../bromwich-inversion-formula.md) is

$$
y(t)=\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}\frac{e^{p(t-1)}}{p+1}\,dp,\qquad\gamma>-1,
$$

with the vertical [Bromwich contour](../../../../bromwich-contour.md) traversed upwards and its symmetric improper limit understood. For $t>1$, close to the left, where the exponential decays; the enclosed [simple pole](../../../../simple-pole.md) at $p=-1$ has [residue](../../../../residue.md) $e^{-(t-1)}$. For $t<1$, close to the right, which contains no [pole](../../../../pole.md). Thus

$$
\boxed{y(t)=e^{-(t-1)}\Theta(t-1),}
$$

where $\Theta$ is the [Heaviside step function](../../../../heaviside-step-function.md). This agrees with the [Laplace transform time-shift rule](../../../../laplace-transform-time-shift-rule.md). At $t=1$, inversion returns the average $1/2$ of the two one-sided values. The value assigned at that single point does not affect the differential equation in the distributional sense.

**Fourier transform.** State the convention explicitly:

$$
\widetilde y(k)=\int_{-\infty}^{\infty}y(t)e^{-ikt}\,dt,\qquad y(t)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde y(k)e^{ikt}\,dk.
$$

The [Fourier transform](../../../../fourier-transform-split.md) of the distributional [derivative](../../../../derivative.md) is $ik\widetilde y(k)$, including the jump at $t=1$. The [Dirac delta](../../../../dirac-delta-function.md) has transform $e^{-ik}$, giving

$$
\boxed{\widetilde y(k)=\frac{e^{-ik}}{1+ik}.}
$$

**Inverse Fourier integral.** Substitute into the inverse [Fourier transform](../../../../fourier-transform-split.md):

$$
y(t)=\frac1{2\pi}\int_{-\infty}^{\infty}\frac{e^{ik(t-1)}}{1+ik}\,dk.
$$

The only [pole](../../../../pole.md) is at $k=i$. For $t>1$, close in the upper half-plane. [Jordan's lemma](../../../../jordan-s-lemma.md) removes the large arc and the [residue theorem](../../../../residue-theorem.md) gives $i\operatorname{Res}_{k=i}=i[e^{-(t-1)}/i]=e^{-(t-1)}$. For $t<1$, close in the lower half-plane, where there are no [poles](../../../../pole.md), giving zero. This reproduces

$$
\boxed{y(t)=\begin{cases}0,&t<1,\\e^{1-t},&t>1,\end{cases}\qquad y(1)=\tfrac12\text{ under symmetric inversion}.}
$$

Integrating the differential equation across the impulse checks the unit jump, $y(1^+)-y(1^-)=1$. Away from the impulse the solution obeys $y'=-y$, and it satisfies the stipulated zero past.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
