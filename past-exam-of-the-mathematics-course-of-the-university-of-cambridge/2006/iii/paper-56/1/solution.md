<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is obtained by varying the [scalar field](../../../../../scalar-field.md), integrating the [derivative](../../../../../derivative.md) terms by parts, and requiring the coefficient of an arbitrary compactly supported variation to vanish:

$$
\boxed{\phi_{tt}-\phi_{xx}+\sin\phi=0.}
$$

The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\phi_t$, so the [Hamiltonian density](../../../../../hamiltonian-density.md) and conserved [energy](../../../../../energy.md) are

$$
\mathcal E=\frac12\phi_t^2+\frac12\phi_x^2+1-\cos\phi,\qquad
\boxed{E=\int_{\mathbb R}\mathcal E\,dx.}
$$

Indeed,

$$
\partial_t\mathcal E=\phi_t(\phi_{tt}+\sin\phi)+\phi_x\phi_{xt}
=\partial_x(\phi_t\phi_x).
$$

Thus $dE/dt=[\phi_t\phi_x]_{-\infty}^{+\infty}=0$ for the finite-energy boundary conditions with no flux at infinity. The [scalar-field vacua](../../../../../scalar-field-vacuum.md) are the constant fields $2\pi m$, $m\in\mathbb Z$.

For a static field, multiply $\phi''=\sin\phi$ by $\phi'$ to obtain $\tfrac12\phi'^2+\cos\phi=C$. The vacuum limits fix $C=1$, so on the increasing interval $0<\phi<2\pi$,

$$
\phi'=2\sin(\phi/2),\qquad \log\tan(\phi/4)=x-a.
$$

Consequently

$$
\boxed{\phi_K(x)=4\arctan e^{x-a},\qquad a\in\mathbb R.}
$$

Its [derivative](../../../../../derivative.md) is $2\operatorname{sech}(x-a)$, and its [energy](../../../../../energy.md) is $\int4\operatorname{sech}^2(x-a)dx=8$. The increasing sign cannot change inside $(0,2\pi)$ because the [derivative](../../../../../derivative.md) does not vanish there. This proves uniqueness up to translation for the prescribed boundary conditions.

There are continuously many translated static solutions with those same endpoints, but only one modulo translations. In the full theory, the adjacent-vacuum [kinks](../../../../../scalar-field-kink.md) and [antikinks](../../../../../antikink.md) are

$$
\phi_{m,\sigma}(x)=2\pi m+\sigma\,4\arctan e^{x-a},\qquad m\in\mathbb Z,\quad \sigma=\pm1.
$$

Their endpoints are $2\pi m$ and $2\pi(m+\sigma)$. Thus there are countably many adjacent-vacuum boundary sectors, each with a continuous center parameter; [integer](../../../../../integer.md) field shifts and reflection relate their shapes. A [Lorentz boost](../../../../../lorentz-boost.md) gives moving [kinks](../../../../../scalar-field-kink.md), replacing $x-a$ by $(x-vt-a)/\sqrt{1-v^2}$, with [energy](../../../../../energy.md) $8/\sqrt{1-v^2}$. There is no finite static [kink](../../../../../scalar-field-kink.md) joining nonadjacent [scalar-field vacua](../../../../../scalar-field-vacuum.md): reaching an intermediate vacuum at finite $x$ would give both the equilibrium value and zero [derivative](../../../../../derivative.md), forcing a constant solution by uniqueness of the second-order [initial value problem](../../../../../initial-value-problem.md). Dynamical multisolitons are a different matter.

The printed [Sine-Gordon Bäcklund transformation](../../../../../sine-gordon-backlund-transformation.md) has a normalization error. With precisely the printed coordinates $\tau=x+t$, $\rho=x-t$,

$$
\partial_\tau\partial_\rho=\frac14(\partial_x^2-\partial_t^2),\qquad
\phi_{\tau\rho}=\frac14\sin\phi
$$

is the field equation. Put $s=(\phi_1+\phi_0)/2$, $d=(\phi_1-\phi_0)/2$. The printed relations give $d_\rho=b\sin s$ and $s_\tau=b^{-1}\sin d$, hence

$$
d_{\rho\tau}=\cos s\sin d,\qquad s_{\tau\rho}=\cos d\sin s.
$$

Adding and subtracting yields

$$
\phi_{1,\tau\rho}=\sin(s+d)=\sin\phi_1,\qquad
\phi_{0,\tau\rho}=\sin(s-d)=\sin\phi_0.
$$

These are the equations with mass squared four, not the unit-mass equation derived from the Lagrangian. A concrete counterexample is the seed $\phi_0=0$, parameter $b=1$, and transformed field $\phi_1=4\arctan e^{2x}$. It obeys both printed first-order relations but satisfies $\phi_{1,xx}=4\sin\phi_1$, so its unit-mass field-equation residual is $-3\sin\phi_1$, which is not identically zero. **The requested preservation claim is false with the printed normalization.**

There are two equivalent repairs. Keep the printed first-order coefficients but take $\tau=(x+t)/2$, $\rho=(x-t)/2$; then $\partial_\tau\partial_\rho=\partial_x^2-\partial_t^2$ and the preceding calculation proves preservation. Alternatively keep the printed coordinates and replace the coefficients $2b,2b^{-1}$ by $b,b^{-1}$. Then $d_\rho=(b/2)\sin s$, $s_\tau=(b^{-1}/2)\sin d$, and the differentiated equations carry a factor $1/4$, giving exactly $\phi_{j,\tau\rho}=\tfrac14\sin\phi_j$. This is the [light-cone normalization of the sine-Gordon Bäcklund transformation](../../../../../light-cone-normalization-of-the-sine-gordon-backlund-transformation.md). For a zero seed it gives $\phi_1=4\arctan\exp[(b\rho+b^{-1}\tau)/2]$; $b=1$ recovers the unit-width static [kink](../../../../../scalar-field-kink.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
