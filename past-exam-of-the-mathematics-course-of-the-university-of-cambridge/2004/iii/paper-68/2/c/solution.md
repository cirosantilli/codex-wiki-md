<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\beta=2(q-1)>0$. With zero viscosity and $S=f(r)\Sigma$, the [wind-loaded Keplerian disk evolution](../../../../../../wind-loaded-keplerian-disk-evolution.md) equation becomes

$$
\Sigma_t=\frac1r\partial_r(\beta r^2f\Sigma)-f\Sigma=\beta rf\Sigma_r+[\beta(2f+rf')-f]\Sigma.
$$

On an interval with $f>0$, introduce the inward travel-time coordinate and weighted density

$$
\boxed{x'(r)=\int^r\frac{du}{\beta u f(u)},\qquad g'(r,t)=f(r)r^{2-1/\beta}\Sigma(r,t).}
$$

Primes on $x'$ and $g'$ denote the new variables, not differentiation. To verify the transformation, let $W=fr^{2-1/\beta}$ and $w=\beta rf$. Its logarithmic derivative satisfies

$$
w\frac{W_r}{W}=\beta rf'+(2\beta-1)f=\beta(2f+rf')-f.
$$

Since $\partial_{x'}=w\partial_r$, multiplication of the density equation by W gives exactly

$$
\boxed{\partial_tg'=\partial_{x'}g'.}
$$

This establishes [inward transport by an angular-momentum-enhanced disk wind](../../../../../../inward-transport-by-an-angular-momentum-enhanced-disk-wind.md), including the amplitude weighting rather than only a characteristic speed.

The general local [advection equation](../../../../../../transport-equation.md) solution is $g'=F(x'+t)$; an initial profile fixes F on the interval swept out by its characteristics. A constant wave phase therefore obeys $dx'/dt=-1$, or

$$
\boxed{\frac{dr}{dt}=-\beta rf(r)<0,\qquad \Sigma(r,t)=\frac{F(x'(r)+t)}{f(r)r^{2-1/\beta}}.}
$$

Thus the transformed wave propagates inward. The physical [surface density](../../../../../../surface-density-of-a-disk.md) is not a rigid profile in r: its weighting accounts for radial compression and loss of mass into the outflow. The same velocity follows independently from the mass flux in part (a), $u_r=\mathcal F/(2\pi r\Sigma)=-\beta rf$. If f vanishes, the coordinate change applies only on the neighboring positive-loss intervals; at a loss-free point this wind-driven velocity vanishes.

A [magnetocentrifugal acceleration](../../../../../../magnetocentrifugal-acceleration.md) mechanism can produce $q>1$. A poloidal field anchored to the disc transmits a torque to the outflow and enforces approximate corotation below its [Alfvén surface](../../../../../../alfven-surface.md). The wind's total specific angular momentum is $\Omega_0r_A^2$, where $r_A$ is its cylindrical [Alfvén radius](../../../../../../alfven-radius.md), compared with the footpoint value $h_0=\Omega_0r_0^2$. Hence $q=(r_A/r_0)^2>1$ for a lever arm beyond the footpoint. Magnetic stresses remove the surplus angular momentum and drive accretion without an effective internal viscosity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
