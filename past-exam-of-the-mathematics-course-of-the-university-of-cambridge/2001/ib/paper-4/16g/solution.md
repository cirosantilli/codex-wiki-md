<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

Assume nonzero upstream speed, so $F>0$. For steady constant-density flow, [mass conservation](../../../../../mass-conservation.md) gives the constant volume flux

$$
whu=WHU.
$$

The [Bernoulli equation](../../../../../bernoulli-equation.md) states that $u^2/2+p/\rho+gz$ is constant along each streamline of a steady inviscid constant-density flow under gravity. It need not have the same value across unrelated [streamlines](../../../../../streamline.md) in a general rotational flow. Here uniform upstream [velocity](../../../../../velocity.md) supplies the same head, and the slowly varying, nearly horizontal channel permits [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $p=p_{\rm atm}+\rho g(h-z)$. Neglecting losses, the [Bernoulli equation](../../../../../bernoulli-equation.md) therefore gives

$$
\frac{u^2}{2}+gh=\frac{U^2}{2}+gH.
$$

Substitute $u=UWH/(wh)$ and set $s=h/H$, $F=U^2/(gH)$, the square of the upstream [Froude number](../../../../../froude-number.md). Rearrangement gives

$$
\boxed{\left(\frac Ww\right)^2=G(s),\qquad
G(s)=\left(1+\frac2F\right)s^2-\frac2F s^3.}
$$

For positive depth, this cubic increases to its maximum at $s_*=(F+2)/3$ and then decreases until it reaches zero at $(F+2)/2$. Its maximum is $G(s_*)=(F+2)^3/(27F)$. Consequently the [critical width of a rectangular open-channel contraction](../../../../../critical-width-of-a-rectangular-open-channel-contraction.md) is

$$
\boxed{w_c=W\sqrt{\frac{27F}{(F+2)^3}},\qquad w(x)\ge w_c.}
$$

At equality the two positive-depth branches coalesce and the local [Froude number](../../../../../froude-number.md) equals one.

When $w>w_c$ everywhere, a smooth solution connected to the upstream state cannot change branch without passing through that coalescence. At $w=W$ the upstream depth is $s=1$, with $G'(1)=2(F-1)/F$. If $F<1$, this point is on the descending, subcritical branch. At a wider location $w>W$, the left-hand side falls below $1=G(1)$, so the depth on that branch must increase: **$h>H$ for subcritical upstream flow $F<1$**. If $F>1$, the upstream state is on the ascending, supercritical branch and decreasing the left-hand side decreases $s$: **$h<H$ for supercritical upstream flow $F>1$**.

For $F=1$, $w_c=W$ and the upstream state is critical. A literally constant-width upstream region then conflicts with the strict assumption $w>w_c$ everywhere. If the upstream state is interpreted only as an asymptotic critical limit, a widened channel has one solution with $h<H$ and one with $h>H$; a further branch condition is required. Merely solving the cubic at one location, without retaining the upstream-connected branch, would not determine the physically continued depth.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
