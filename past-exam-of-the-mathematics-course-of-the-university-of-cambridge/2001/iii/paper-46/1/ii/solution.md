<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $\kappa>0$ and initially $\omega\ne0$. Write $m_j(y,t)=\int_{\mathbb R}x^j\chi(x,y,t)\,dx$, and set $k=\pi/L$, $a=\kappa k^2$. The [advection-diffusion equation](../../../../../../advection-diffusion-equation.md) is $\chi_t+u\chi_x=\kappa(\chi_{xx}+\chi_{yy})$. Integration by parts in the unbounded coordinate gives the [longitudinal moment hierarchy for shear transport](../../../../../../longitudinal-moment-hierarchy-for-shear-transport.md)

$$
\partial_t m_0=\kappa\partial_y^2m_0,\qquad
\partial_t m_1=\kappa\partial_y^2m_1+um_0,\qquad
\partial_t m_2=\kappa\partial_y^2m_2+2um_1+2\kappa m_0.
$$

All three moments obey [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) at the walls. The initial values are $m_0=L$, $m_1=0$, $m_2=L^3/12$. These manipulations require finite moments and vanishing boundary terms at $x=\pm\infty$; diffusion of the compact initial distribution supplies the required decay for positive time.

The zeroth moment remains exactly $L$. Since $\sin(ky)$ is a Neumann eigenfunction, put $m_1=L g(t)\sin(ky)$. Then $g'+ag=U\cos(\omega t)$ and $g(0)=0$, giving

$$
g(t)=\frac{U}{a^2+\omega^2}[a\cos(\omega t)+\omega\sin(\omega t)-ae^{-at}].
$$

For the second moment, $2um_1=LUg\cos(\omega t)[1-\cos(2ky)]$. Thus $m_2=A(t)+B(t)\cos(2ky)$, with

$$
A'=2\kappa L+LUg\cos(\omega t),\qquad
B'+4aB=-LUg\cos(\omega t),\qquad A(0)=L^3/12,\quad B(0)=0.
$$

The equation for $B$ has positive damping and bounded forcing, so $B$ remains bounded. In the equation for $A$, the decaying term in $g$ contributes only a bounded accumulated transient. Over a complete nonzero-frequency cycle, $\langle\cos^2(\omega t)\rangle_t=1/2$ and $\langle\sin(\omega t)\cos(\omega t)\rangle_t=0$. Consequently

$$
A(t)=\left[2\kappa L+\frac{LU^2a}{2(a^2+\omega^2)}\right]t+O(1),
\qquad
\boxed{m_2(y,t)=2Ktm_0+O(1),\quad K=\kappa+\frac{U^2a}{4(a^2+\omega^2)}.}
$$

This proves [oscillating shear dispersion in an insulating channel](../../../../../../oscillating-shear-dispersion-in-an-insulating-channel.md), including the local-in-$y$ leading term, not just a cross-channel average. The instantaneous derivative retains bounded periodic oscillations; its cycle-averaged slope is $2Km_0$. Thus $2Ktm_0$ is the leading second moment, rather than a literal rate proportional to $t$.

The asymptotic statement holds for fixed positive [diffusivity](../../../../../../diffusion-coefficient.md) and fixed nonzero frequency, after times long compared with $a^{-1}$ and the oscillation period. If $|\omega|L^2/\kappa\ll1$, transverse [diffusion](../../../../../../diffusion.md) adjusts rapidly to the changing [shear flow](../../../../../../shear-flow.md), and

$$
K\simeq\kappa+\frac{U^2L^2}{4\pi^2\kappa}.
$$

This is the cycle average of the instantaneous steady-shear enhancement $U^2\cos^2(\omega t)/(2a)$. At exactly $\omega=0$, there is no cycle average: $g\to U/a$ and $K=\kappa+U^2/(2a)$. Hence the zero-frequency and long-time limits do not commute. In the intermediate range $a^{-1}\ll t\ll|\omega|^{-1}$, the shear is approximately steady at its initial amplitude and that latter enhancement is appropriate.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
