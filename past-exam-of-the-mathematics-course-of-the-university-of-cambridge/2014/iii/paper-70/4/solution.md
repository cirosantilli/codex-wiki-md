<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $a=(\rho_b-\rho_t)/H=\rho_0N^2/g$. The initial density is $\rho(z)=\rho_t-az$. Conservation of mass in the material homogenized over $-h<z<0$ fixes its mean density to $\rho_u=\rho_t+ah/2$, while the untouched lower layer has interfacial density $\rho_i=\rho_t+ah$. Hence the [reduced gravity](../../../../../reduced-gravity-split.md) difference across the interface is

$$
\boxed{g'=\frac{g(\rho_i-\rho_u)}{\rho_0}=\frac{N^2h}{2}.}
$$

The reference contribution involving $\rho_t$ cancels from the difference.

Only the upper layer changes its [potential energy](../../../../../potential-energy.md). The [potential-energy cost of homogenizing a linear stratification](../../../../../potential-energy-cost-of-homogenizing-a-linear-stratification.md) is

$$
\begin{aligned}
\Delta P&=\pi R^2g\int_{-h}^0z\,[\rho_u-\rho(z)]\,dz\\
&=\pi R^2ga\int_{-h}^0z\left(\frac h2+z\right)dz
=\pi R^2ga\left(-\frac{h^3}{4}+\frac{h^3}{3}\right),
\end{aligned}
$$

so

$$
\boxed{\Delta P=\frac{\rho_0\pi R^2N^2h^3}{12},\qquad
\frac{dP}{dt}=\frac{\rho_0\pi R^2N^2h^2}{4}\frac{dh}{dt}.}
$$

The positive sign reflects work against stable stratification.

The rotating boundary supplies energy on scales set by $\Omega$ and $R$. Turbulent drag and dissipation remove energy, and [entrainment](../../../../../fluid-entrainment.md) adds initially stationary fluid that must be accelerated. If upper-layer energy grows, the increasing turbulent loss provides a restoring tendency; after a short adjustment, input and losses can approximately balance while the interface moves on a slower time scale. This gives a physical rationale for a [fixed-energy turbulent mixed layer](../../../../../fixed-energy-turbulent-mixed-layer.md), not a consequence of [mass conservation](../../../../../mass-conservation.md) alone. Its characteristic [kinetic energy](../../../../../kinetic-energy.md) is $K\sim\rho_0\pi R^2hu_u^2/2$. With the stipulated $N$-independent energy closure,

$$
u_u^2h=A\Omega^2R^3,\qquad K\sim\frac A2\rho_0\pi\Omega^2R^5,
$$

so the characteristic speed decreases as $h^{-1/2}$ rather than remaining constant.

The stress does work at a rate proportional to $\pi R^2\tau u_u=c_D\rho_0\pi R^2u_u^3$. Combine this with the energy increase and absorb fixed drag/geometrical factors into $C>0$:

$$
\dot h=C\frac{u_u^3}{N^2h^2}\left(\frac\Omega N\right)^\alpha\left(\frac\delta R\right)^\beta,
\qquad E=\frac{\dot h}{u_u}=C\frac{u_u^2}{N^2h^2}\left(\frac\Omega N\right)^\alpha\left(\frac\delta R\right)^\beta.
$$

Here the exponents $\alpha,\beta$ are unrelated to the plume [entrainment coefficient](../../../../../entrainment-coefficient.md) in Question 2. The [interfacial Richardson number](../../../../../interfacial-richardson-number.md) is

$$
\mathrm{Ri}_i=\frac{N^2h\delta}{2u_u^2}
=\frac1{2A}\left(\frac N\Omega\right)^2\left(\frac hR\right)^2\frac\delta R.
$$

Set $q=\Omega/N$, $d=\delta/R$ and $r=h/R$. Then $u_u^2/(N^2h^2)=d/(2r\mathrm{Ri}_i)$ and $r=q(2A\mathrm{Ri}_i/d)^{1/2}$. Substitution gives

$$
E=C' q^{\alpha-1}d^{\beta+3/2}\mathrm{Ri}_i^{-3/2}.
$$

The assumption that $E$ depends on the local [Richardson number](../../../../../richardson-number.md) alone excludes separate dependences on $q,d$. The [entrainment exponent from a local interfacial Richardson closure](../../../../../entrainment-exponent-from-a-local-interfacial-richardson-closure.md) is consequently

$$
\boxed{\alpha=1,\qquad\beta=-\frac32,\qquad\gamma=\frac32,\qquad E=C_E\mathrm{Ri}_i^{-3/2}.}
$$

This comparison treats $q$ and $d$ as independently variable external controls; fitting only a single apparatus would not by itself determine the exponents.

Finally, use the fixed-energy closure again:

$$
\dot h=C_Eu_u\left(\frac{N^2h\delta}{2u_u^2}\right)^{-3/2}
=C_*\frac{\Omega^4R^6}{N^3\delta^{3/2}}h^{-7/2},
\qquad C_*=2^{3/2}C_EA^2.
$$

Integrating from a positive initial mixed-layer depth $h_0$ at time $t_0$ gives

$$
h^{9/2}=h_0^{9/2}+\frac92C_*\frac{\Omega^4R^6}{N^3\delta^{3/2}}(t-t_0).
$$

When the growth term dominates the initial offset, the [rotating-disc mixed-layer depth law](../../../../../rotating-disc-mixed-layer-depth-law.md) is

$$
\boxed{\frac hR=B\left(\frac{\Omega^2R}{N^2\delta}\right)^{1/3}[\Omega(t-t_0)]^{2/9},\qquad B=\left(\frac92C_*\right)^{2/9}.}
$$

Taking the effective time origin to be zero gives the stated scaling. Its validity is limited to the regime of the closures and $h<H$; the singular velocity predicted at $h=0$ is not a model for the initial boundary-layer formation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
