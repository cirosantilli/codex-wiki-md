<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work at fixed enclosed mass $m$, so the perturbations are [fluid Lagrangian perturbations](../../../../../lagrangian-perturbation-of-a-fluid-variable.md). The equilibrium acceleration vanishes. Varying the factor $r^{-4}$ in the gravitational force contributes $4Gm\delta r/(4\pi r^5)$, while varying the factor multiplying the acceleration gives no first-order term because the background acceleration is zero. With $\delta r=r\xi e^{-i\omega t}$, the linearized momentum equation is

$$
\boxed{\frac{d\delta p}{dm}-\frac{\omega^2\xi}{4\pi r}-\frac{Gm\xi}{\pi r^4}=0.}
$$

Conservation of the mass of each displaced shell gives its fractional density change as minus the fractional volume change. Thus

$$
\boxed{\delta\rho=-\frac{\rho}{r^2}\frac{d(r^2\delta r)}{dr}=-\rho(r\xi'+3\xi)=-\rho\chi.}
$$

The adiabatic relation is $\delta p=\gamma p\delta\rho/\rho=-\gamma p\chi$. Use $dm/dr=4\pi r^2\rho$ and the [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) $p'=-Gm\rho/r^2$ to turn the mass-coordinate momentum equation into $(\delta p)'-\omega^2\rho r\xi+4p'\xi=0$. It follows that the [radial stellar pulsation equation](../../../../../radial-stellar-pulsation-equation.md) is

$$
\boxed{\frac{d}{dr}[\gamma p(r\xi'+3\xi)]-4p'\xi+\omega^2\rho r\xi=0.}
$$

The [stellar adiabatic exponent](../../../../../stellar-adiabatic-exponent.md) may vary with radius, so it must remain inside the derivative.

Expand the derivative and multiply by $r^3$. The [self-adjoint differential equation](../../../../../self-adjoint-differential-equation.md) becomes

$$
\boxed{(\gamma pr^4\xi')'+\left\{r^3[(3\gamma-4)p]'+\omega^2\rho r^4\right\}\xi=0.}
$$

Hence $f(r)=\gamma pr^4$ and $g(r)=r^3[(3\gamma-4)p]'+\omega^2\rho r^4$ in the requested form. Multiplying by a real eigenfunction and integrating gives the boundary term $[\gamma pr^4\xi\xi']_0^R$. It vanishes for a regular centre and bounded admissible surface displacement and derivative, since $p(R)=0$. Therefore the [weighted stellar pulsation Rayleigh quotient](../../../../../weighted-stellar-pulsation-rayleigh-quotient.md) is

$$
\boxed{\omega^2=\frac KI,\quad
K=\int_0^R\left[\gamma pr^4(\xi')^2-r^3[(3\gamma-4)p]'\xi^2\right]dr,\quad
I=\int_0^R\rho r^4\xi^2\,dr>0.}
$$

Real coefficients and the symmetric endpoint conditions give the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md); the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) identifies its minimum with the lowest squared frequency. For complex amplitudes the corresponding quadratic forms use modulus squares, and the real eigenfunctions may be chosen for this calculation.

Integrate the second term of $K$ by parts. Its boundary term $-[(3\gamma-4)pr^3\xi^2]_0^R$ again vanishes. The remaining integrand is

$$
p r^2\left[\gamma a^2+(3\gamma-4)(3\xi^2+2a\xi)\right],\qquad a=r\xi'.
$$

Since $\chi=a+3\xi$, one has $3\xi^2+2a\xi=(\chi^2-a^2)/3$. Substitution proves the [positive-square radial pulsation energy](../../../../../positive-square-radial-pulsation-energy.md) identity

$$
\boxed{K=\frac13\int_0^Rpr^2\left[4r^2(\xi')^2+(3\gamma-4)\chi^2\right]dr.}
$$

If $\gamma\ge4/3$ throughout the positive-pressure interior, both terms are nonnegative for every admissible displacement. No negative squared frequency is then possible. Hence **radial dynamical instability requires $\gamma<4/3$ somewhere inside the star**.

For the opposite necessary condition, test the quotient with a nonzero constant $\xi=C$. It has $\chi=3C$ and

$$
K[C]=3C^2\int_0^R(3\gamma-4)pr^2\,dr.
$$

If $\gamma\le4/3$ everywhere and is strictly below $4/3$ on a positive-pressure interval, this is negative. The lowest eigenvalue is at most this negative trial quotient, proving instability. Strict dynamical stability requires the stronger weighted condition

$$
\boxed{\int_0^R(3\gamma-4)pr^2\,dr>0,}
$$

and in particular **$\gamma>4/3$ somewhere**. This is the [pressure-weighted radial instability criterion](../../../../../pressure-weighted-radial-instability-criterion.md) viewed as a necessary test for strict stability.

The word “stability” needs a marginal qualification: if $\gamma=4/3$ throughout, $\xi=C$ solves the pulsation equation with $\omega=0$. The star is marginally stable in this radial sense, so the strict $\gamma>4/3$ requirement applies to positive fundamental squared frequency, not to a definition that includes a zero-frequency neutral mode. There is no exponentially growing mode in this equality case, but the zero restoring force also permits a secular solution linear in time.

The conditions are useful as rapid tests, but local threshold crossings are not a complete criterion for a mixed exponent profile. If $\gamma\ge4/3$ everywhere and exceeds it on a positive-pressure interval, the square identity forces $K>0$ for every nonzero eigenfunction: zero energy would first force constant $\xi$ and then force that constant to vanish. If $\gamma\le4/3$ everywhere with strict inequality on an interval, the constant trial proves instability. When both types of region occur, $\gamma<4/3$ somewhere does not alone prove instability, and $\gamma>4/3$ somewhere does not alone prove stability. A negative pressure-weighted average proves instability, while a positive one tests only the homologous displacement; another radial shape may still have negative energy. Determining the mixed case requires minimizing the full [weighted stellar pulsation Rayleigh quotient](../../../../../weighted-stellar-pulsation-rayleigh-quotient.md) or solving the [radial stellar pulsation equation](../../../../../radial-stellar-pulsation-equation.md). These are radial adiabatic statements and do not rule out nonradial, convective or nonadiabatic instabilities.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
