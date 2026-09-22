<h1 id="7c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $H=(\dot x^2+x^2)/2$. Then

$$
\dot H=\epsilon\dot x^2(1-\alpha x^2+\beta x^4).
$$

On an unperturbed circle write $x=r\cos t$, $\dot x=-r\sin t$. The supplied integrals give

$$
\Delta H=\epsilon\pi r^2\left(1-\frac{\alpha r^2}{4}+\frac{\beta r^4}{8}\right)+O(\epsilon^2).
$$

Equivalently, the leading [averaged amplitude equation](../../../../../../averaged-amplitude-equation.md) is

$$
\dot r=\frac{\epsilon r}{2}\left(1-\frac{\alpha r^2}{4}+\frac{\beta r^4}{8}\right).
$$

With $s=r^2$, its nonzero stationary amplitudes solve $\beta s^2-2\alpha s+8=0$. If $\alpha^2>8\beta$, both roots are positive and simple:

$$
\boxed{r_\pm^2=\frac{\alpha\pm\sqrt{\alpha^2-8\beta}}{\beta}.}
$$

The averaged drift is positive below $r_-$, negative between $r_-$ and $r_+$, and positive above $r_+$. Thus the **inner orbit is attracting and the outer orbit repelling**, with leading displacement amplitudes $r_-$ and $r_+$ and period $2\pi+O(\epsilon)$. The simple zeros of the [Poincaré return map](../../../../../../poincare-map.md) persist for sufficiently small $\epsilon$.

If $\alpha^2<8\beta$, the leading quadratic is strictly positive for all $s\ge0$; the energy increases on every nonzero unperturbed orbit, so the [energy balance method](../../../../../../energy-balance-method.md) yields no [periodic orbits](../../../../../../periodic-orbit.md) in any fixed compact range of nonzero amplitudes for sufficiently small $\epsilon$. This perturbative calculation does not itself establish a uniform global exclusion at amplitudes growing as $\epsilon$ tends to zero. At equality, the leading drift has a double zero at $r^2=\alpha/\beta$. It is positive on both sides, with a semistable candidate at that amplitude. **First-order averaging alone cannot decide whether the exact system has zero, one, or two nearby [periodic orbits](../../../../../../periodic-orbit.md) at equality**: higher-order drift determines the unfolding of this degenerate zero. The original PDF has $\alpha^2=8\beta$; the extra exponent on $\beta$ in the converted TeX is an OCR error.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7C](../../7c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
