<h1 id="a/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume constant [mass density](../../../../../density.md), a prismatic channel, approximately uniform cross-sectional [velocity](../../../../../velocity.md) $u$, a [hydrostatic pressure](../../../../../hydrostatic-pressure.md) distribution, small bed slope $S$, and no lateral inflow. Integrating [mass conservation](../../../../../mass-conservation.md) over a slice of length $dx$ gives $\rho A_tdx=\rho Au|_x-\rho Au|_{x+dx}$, hence $A_t+(Au)_x=0$.

Let $I(A)=\int_A(H-z)\,dA$ be the hydrostatic first moment, where $H$ is the actual free-surface depth. The downstream [momentum](../../../../../momentum-split.md) balance is

$$
(Au)_t+(Au^2+gI)_x=gAS-\frac{\tau\ell}{\rho}.
$$

Using $A_t+(Au)_x=0$ reduces its left side to $A(u_t+uu_x)+gI_x$. For a fixed prismatic cross-section, $dI/dH=A$, so $I_x/A=H_x$. Therefore the exact depth-averaged result is

$$
\boxed{u_t+uu_x=gS-\frac{\tau}{\rho R}-gH_x,\qquad R=A/\ell.}
$$

Here [hydraulic radius](../../../../../hydraulic-radius.md) converts perimeter [shear stress](../../../../../shear-stress.md) into [force](../../../../../force-split.md) per unit fluid volume. The printed notation $\bar h$ yields the requested equation if it denotes this hydraulic [pressure](../../../../../pressure-split.md) head, whose [derivative](../../../../../derivative.md) equals $H_x$.

**The geometrical definition printed in the next part needs care.** [Triangular-channel hydrostatic pressure head](../../../../../triangular-channel-hydrostatic-pressure-head.md) gives the factor explicitly. For the stated symmetric triangular notch, the actual depth is $H=(\ell/2)\sin\theta$, whereas its printed $\bar h=(\ell/4)\sin\theta$ is $H/2$. Indeed $A=H^2\cot\theta$ and $I=AH/3$, giving $I_x/A=H_x=2\bar h_x$. Thus the equation with precisely the printed geometrical $\bar h$ has [pressure](../../../../../pressure-split.md) term $-2g\bar h_x$. A first-principles derivation cannot remove that factor. The subsequent intended scaling can be carried out algebraically using the printed convention, as below, or with the [pressure](../../../../../pressure-split.md) scale doubled for the actual triangular channel.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
