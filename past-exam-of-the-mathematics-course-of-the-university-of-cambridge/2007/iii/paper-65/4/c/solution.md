<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider the nontrivial gravitational mode with $k\ne0$. At $\omega^2=0$, horizontal momentum requires $ikW=0$, hence $W=0$ and

$$
\delta\rho=-\frac{\rho}{c_s^2}\phi.
$$

Substituting into the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) and using $4\pi G\rho_0/c_s^2=2/H^2$ gives

$$
\phi_{zz}+\left[\frac2{H^2}\operatorname{sech}^2(z/H)-k^2\right]\phi=0.
$$

Set $\tau=\tanh(z/H)$ and $\nu=kH$. Since $\partial_z=(1-\tau^2)\partial_\tau/H$, this becomes the [associated Legendre equation](../../../../../../associated-legendre-differential-equation.md) of degree one and order $\nu$:

$$
\boxed{\frac d{d\tau}\left[(1-\tau^2)\frac{d\phi}{d\tau}\right]
+\left[2-\frac{\nu^2}{1-\tau^2}\right]\phi=0}.
$$

To verify the two explicit solutions, put $\eta=z/H$ and $T=\tanh\eta$. They are

$$
F_+=e^{\nu\eta}(\nu-T),\qquad F_-=e^{-\nu\eta}(\nu+T),
$$

because $e^{2\eta}=(1+\tau)/(1-\tau)$. Differentiating $F_+$ twice gives

$$
(F_+)_{\eta\eta}=e^{\nu\eta}\left[\nu^2(\nu-T)-2\nu(1-T^2)+2T(1-T^2)\right],
$$

which cancels identically against $[2(1-T^2)-\nu^2]F_+$. Reflection $\eta\mapsto-\eta$ proves the same for $F_-$. Their [Wronskian](../../../../../../wronskian.md) is $2\nu(1-\nu^2)$, evaluated at $\eta=0$; thus they are generally independent but coincide or become dependent at the exceptional orders $0,\pm1$.

Use $n=|k|H>0$ to analyze decay, which is unaffected by the sign of $k$. The solution decaying at $+\infty$ is proportional to $e^{-n\eta}(n+\tanh\eta)$. At $-\infty$ its leading term is $(n-1)e^{n|\eta|}$, so it also decays there only if $n=1$. At this value

$$
e^{-\eta}(1+\tanh\eta)=e^{\eta}(1-\tanh\eta)=\operatorname{sech}\eta.
$$

Therefore the [marginal fragmentation mode of an isothermal slab](../../../../../../marginal-fragmentation-mode-of-an-isothermal-slab.md) has

$$
\boxed{|k|=\frac1H,\qquad \Phi'=\phi\propto\operatorname{sech}(z/H),\qquad
\delta\rho\propto\operatorname{sech}^3(z/H)}.
$$

At $n=1$ the second independent solution obtained by [reduction of order](../../../../../../reduction-of-order.md) grows at infinity, so the coincidence of the two explicit formulas does not supply an extra admissible mode. At $k=0$ a uniform vertical translation gives another neutral disturbance, and mass-preserving relabeling displacements can have $\delta\rho=\phi=0$. Neither is the nonzero-[wavenumber](../../../../../../wavenumber.md) fragmentation threshold just calculated.

**The unstable fragmentation modes have wavelengths greater than $2\pi H$.** Gas-[pressure](../../../../../../pressure.md) support becomes less effective relative to [self-gravity](../../../../../../self-gravity.md) at long wavelength. The side of the threshold can also be checked from the [energy](../../../../../../energy.md) identity: at $|k|=1/H$ the marginal [mass density](../../../../../../density.md) disturbance has zero quadratic [energy](../../../../../../energy.md). Keep that [mass density](../../../../../../density.md) disturbance and decrease $|k|$; the [pressure](../../../../../../pressure.md) integral stays fixed, while the gravitational term becomes more negative because the positive inverse operator $(-\partial_z^2+k^2)^{-1}$ increases as $k^2$ decreases. Thus the quadratic [energy](../../../../../../energy.md) becomes negative, giving an unstable mode on the longer-wavelength side. This argument concerns the gravitational sector and its stated decay conditions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
