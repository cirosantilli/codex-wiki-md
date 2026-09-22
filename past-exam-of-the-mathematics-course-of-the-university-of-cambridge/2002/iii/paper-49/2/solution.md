<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $h$ be layer thickness and $g$ gravitational acceleration. The unforced [shallow water equations](../../../../../shallow-water-equations.md) on the equatorial [beta plane](../../../../../beta-plane.md) are

$$
u_t+uu_x+vu_y-\beta yv=-gh_x,\qquad
v_t+uv_x+vv_y+\beta yu=-gh_y,\qquad
h_t+(hu)_x+(hv)_y=0.
$$

Linearize about $u=v=0$, $h=h_0$. Put $c_0=\sqrt{gh_0}$ and $L=\sqrt{c_0/\beta}$, and scale $(x,y)=L(X,Y)$, $t=(L/c_0)T$, $(u,v)=c_0(U,V)$ and $h=h_0(1+\eta)$. Dropping capitals, the [linearized shallow water equations](../../../../../linearized-shallow-water-equations.md) become

$$
u_t-yv=-\eta_x,\qquad
v_t+yu=-\eta_y,\qquad
\eta_t+u_x+v_y=0.
$$

The choice $\beta L^2/c_0=1$ makes both the wave speed and the coefficient of the dimensionless [Coriolis parameter](../../../../../coriolis-parameter.md) equal to one.

Take [Fourier modes](../../../../../fourier-mode.md) $\{u(y),v(y),\eta(y)\}e^{i(kx-\omega t)}$ that decay as $y\to\pm\infty$. Their equations are

$$
\omega u-k\eta=iyv,\qquad
\omega\eta-ku=-iv',\qquad
-i\omega v+yu=-\eta'.
$$

For $v=0$ and nonzero $k$, the first two require $\omega^2=k^2$. The root $\omega=k$ gives $u=\eta$, and meridional balance becomes $u'=-yu$. Hence the [equatorial Kelvin wave](../../../../../equatorial-kelvin-wave.md) is

$$
\boxed{\omega=k,\qquad v=0,\qquad u=\eta=C e^{-y^2/2}.}
$$

It travels eastward at speed $c_0$ in dimensional units. The other sign gives $\eta=-u$ and $u'=yu$, so $u\propto e^{y^2/2}$ is not trapped.

For $v\ne0$, $\omega\ne0$ and $\omega^2\ne k^2$, inversion of the first two equations gives the [equatorial wave velocity polarization](../../../../../equatorial-wave-velocity-polarization.md)

$$
u=\frac{i(\omega yv-kv')}{\omega^2-k^2},\qquad
\eta=\frac{i(kyv-\omega v')}{\omega^2-k^2}.
$$

Substitute in the remaining momentum equation. Multiplication by $(\omega^2-k^2)/i$ leaves

$$
-\omega(\omega^2-k^2)v+\omega y^2v+kv-\omega v''=0,
$$

so

$$
v''+(\lambda-y^2)v=0,\qquad
\lambda=\omega^2-k^2-\frac k\omega.
$$

Writing $v=e^{-y^2/2}H(y)$ yields $H''-2yH'+(\lambda-1)H=0$, the [Hermite differential equation](../../../../../hermite-differential-equation.md). The trapped solutions have the [Hermite oscillator quantization](../../../../../hermite-oscillator-quantization.md) $\lambda=2n+1$ and $H=H_n$.

For completeness, quantization follows without assuming that every acceptable solution is a [polynomial](../../../../../polynomial-split.md). On decaying smooth functions, define $a=d/dy+y$, $a^\dagger=-d/dy+y$ and $\mathcal H=-d^2/dy^2+y^2=a^\dagger a+1$. [Integration by parts](../../../../../integration-by-parts.md) gives $\lambda\ge1$ and $\|av\|^2=(\lambda-1)\|v\|^2$. If $av\ne0$, it is an [eigenfunction](../../../../../eigenfunction.md) of $\mathcal H$ with [eigenvalue](../../../../../eigenvalue.md) $\lambda-2$. Repeated lowering must terminate: otherwise it eventually produces an [eigenvalue](../../../../../eigenvalue.md) below one. At termination $av=0$, so the terminal [eigenfunction](../../../../../eigenfunction.md) is $e^{-y^2/2}$ and has [eigenvalue](../../../../../eigenvalue.md) one. Repeated raising gives $H_n(y)e^{-y^2/2}$ and $\lambda=2n+1$; uniqueness of a decaying solution at one end of this second-order equation fixes each mode up to scale.

Thus, away from the exceptional quotients, all fields are determined by

$$
\boxed{
v=C H_n(y)e^{-y^2/2},\qquad
\omega^2-k^2-\frac k\omega=2n+1,\qquad n=0,1,2,\ldots.}
$$

Insert this $v$ and its [derivative](../../../../../derivative.md) in the polarization formulae to obtain $u$ and $\eta$. For $n\ge1$, the cubic $\omega^3-(k^2+2n+1)\omega-k=0$ supplies the low-frequency [equatorial Rossby wave](../../../../../equatorial-rossby-wave.md) and two [equatorial inertia--gravity wave](../../../../../equatorial-inertia-gravity-wave.md) branches. Their meridional structures are Gaussian-weighted [Hermite polynomials](../../../../../hermite-polynomial.md).

For $n=0$, multiplication by $\omega$ factorizes the [equatorial shallow-water dispersion relation](../../../../../equatorial-shallow-water-dispersion-relation.md) as

$$
(\omega+k)(\omega^2-k\omega-1)=0.
$$

The physically admissible quadratic gives the [mixed Rossby-gravity wave](../../../../../rossby-gravity-waves.md), equivalently the [Yanai wave](../../../../../rossby-gravity-waves.md):

$$
\boxed{\omega-k-\frac1\omega=0,\qquad
v=C e^{-y^2/2},\qquad u=\eta=i\omega yv.}
$$

These fields satisfy all three original equations directly and decay at both infinities, including where the quotient formulae are singular.

To test the other factor, set $\omega=-k\ne0$. The original equations give $u+\eta=-iyv/k$ and $v'=-yv$. Put $\delta=u-\eta$; meridional momentum then gives

$$
\delta'-y\delta=i(2k-k^{-1})v,\qquad
(e^{-y^2/2}\delta)'=i(2k-k^{-1})C e^{-y^2}.
$$

Decay of $u,\eta$ at both infinities requires the integral of the right side to vanish. Hence $C=0$ unless $k^2=1/2$. Ordinarily the extra factor supplies no trapped mode. At the [exceptional root of the mixed Rossby-gravity mode](../../../../../exceptional-root-of-the-mixed-rossby-gravity-mode.md), $k^2=1/2$, it coincides with the quadratic root and gives the same physical fields, not an additional branch. This distinction avoids discarding a regular physical mode at the crossing.

These arguments concern nonzero wave [angular frequency](../../../../../angular-frequency.md). At $k=0$, the oscillatory nonzero-$v$ modes have $\omega=\pm\sqrt{2n+1}$, while zero-frequency $v=0$ geostrophic states must be considered in the original equations rather than in expressions divided by $\omega$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
