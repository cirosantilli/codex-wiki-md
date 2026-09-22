<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the positive transport coefficient $D$ from the preceding solution. The [porous medium equation](../../../../../../porous-medium-equation.md) here is $h_t=D(h^2h_x)_x=(D/3)(h^3)_{xx}$. A planar pulse conserves the water cross-sectional area $\mathcal V=\int h\,dx$. If the supplied lake volume is a three-dimensional volume $V$, introduce the constant out-of-plane width $B_y$ and take $\mathcal V=V/B_y$; alternatively $V$ may be understood as volume per unit span. A two-dimensional model cannot determine an absolute extent from an unspecified three-dimensional volume alone.

For a symmetric localized release, write $h=t^{-a}f(x/t^b)$. Area conservation requires $a=b$, and balancing the PDE powers gives $a+1=3a+2b$, hence **$a=b=1/4$**. With $\eta=x/t^{1/4}$, the profile equation is

$$
-\frac14(f+\eta f')=D(f^2f')'.
$$

Integrate once, using symmetry and zero central flux: $Df^2f'=-\eta f/4$. Inside the wet region this gives $f^2=C-\eta^2/(4D)$. The dry continuation is zero. Write the result as

$$
\boxed{h(x,t)=H(t)\left[1-\frac{x^2}{L(t)^2}\right]_+^{1/2},\quad
L(t)=2\left(\frac{\mathcal V}{\pi}\right)^{1/2}(Dt)^{1/4},\quad
H(t)=\left(\frac{\mathcal V}{\pi}\right)^{1/2}(Dt)^{-1/4}.}
$$

The normalization follows from $\int_{-L}^Lh\,dx=\pi HL/2=\mathcal V$. This [cubic diffusion pulse](../../../../../../semicircular-pulse-under-cubic-diffusion.md) has finite support $-L<x<L$, total extent $2L$, and spreading speed $\dot L=L/(4t)$. Although $h_x$ is singular at the ideal nose, the flux vanishes there and $u=-Dhh_x=x/(4t)$ tends to the finite front speed.

For a one-sided pulse on $0<x<L$ with a reflecting boundary at zero and the same area $\mathcal V$, replace $\mathcal V$ in the displayed full-line formulas by $2\mathcal V$. The power laws are unchanged. These are source-type [Barenblatt solutions](../../../../../../barenblatt-solution.md) for an instantaneous localized release; a finite initial lake footprint approaches the profile at long times and may require a virtual time origin, rather than matching this singular initial condition exactly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
