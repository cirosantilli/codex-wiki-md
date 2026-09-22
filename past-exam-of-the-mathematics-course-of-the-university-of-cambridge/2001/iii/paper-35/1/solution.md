<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\tau=t-t_0$, let $R$ be the [scale factor](../../../../../scale-factor-cosmology.md), $H=\dot R/R$ the [Hubble parameter](../../../../../hubble-parameter.md), and $\mu=\sqrt{\Lambda/3}$ the asymptotic expansion rate for the positive [cosmological constant](../../../../../cosmological-constant.md). The [continuity equation](../../../../../continuity-equation.md) for a homogeneous [Hubble flow](../../../../../hubble-flow.md) gives $\rho R^3=\rho_0$. Isotropy and the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) give a relative acceleration proportional to displacement from any chosen origin:

$$
\mathbf g=-\frac{4\pi G\rho-\Lambda}{3}\mathbf r.
$$

This uses the local relative [gravitational acceleration](../../../../../gravitational-acceleration.md), rather than trying to sum an absolutely convergent potential over an infinite universe. A fluid element with constant comoving coordinate $\mathbf x$ has $\mathbf r=R\mathbf x$. The spatially uniform [pressure](../../../../../pressure.md) has no gradient, so the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) give

$$
\boxed{\ddot R=-\frac{4\pi G\rho_0}{3R^2}+\frac{\Lambda}{3}R.}
$$

Multiply by $2\dot R$ and integrate. With $A=8\pi G\rho_0/3$, the resulting [first integral](../../../../../first-integral.md) is

$$
\boxed{\dot R^2=A/R+\mu^2R^2-\kappa.}
$$

For an expanding branch that reaches arbitrarily large $R$, $\dot R/R\to\mu$; more precisely, $H=\mu+O(R^{-2})$ and the correction to $\ln R-\mu t$ is integrable. Therefore $R\sim C e^{\mu t}$. Positive $\Lambda$ alone does not make every initially expanding branch escape: sufficiently large positive $\kappa$ can give a turning point or a limiting static radius. Under the stated vacuum-dominance inequalities at $R=1$, however, $A/R$ and $|\kappa|$ remain small compared with $\mu^2R^2$ for the future expanding branch, and $R\simeq e^{\mu\tau}$ is the required approximation.

To derive the [linear cosmological density perturbation](../../../../../linear-cosmological-density-perturbation-split.md) equation, write $\delta=\rho'/\rho$ and $\mathbf v=H\mathbf r+\mathbf u$, where $\mathbf u$ is the [peculiar velocity](../../../../../peculiar-velocity.md). At fixed $\mathbf x=\mathbf r/R$, the linearized [continuity equation](../../../../../continuity-equation.md), [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) and perturbation [Poisson equation](../../../../../poisson-equation.md) are

$$
\dot\delta+R^{-1}\nabla_x\cdot\mathbf u=0,\qquad
\dot{\mathbf u}+H\mathbf u=-R^{-1}\nabla_x(c_s^2\delta+\phi),\qquad
\nabla_x^2\phi=4\pi G R^2\rho\delta.
$$

Taking a [divergence](../../../../../divergence.md) of the second equation and differentiating the first eliminates the [peculiar velocity](../../../../../peculiar-velocity.md). For a [Fourier mode](../../../../../fourier-mode.md) of comoving [wavenumber](../../../../../wavenumber.md) $k$, this gives

$$
\ddot\varepsilon+2H\dot\varepsilon+\left(\frac{c_s^2k^2}{R^2}-4\pi G\rho\right)\varepsilon=0.
$$

The [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) for the four-thirds [polytropic equation of state](../../../../../polytropic-equation-of-state.md) is $c_s^2=dp/d\rho\propto\rho^{1/3}=\rho_0^{1/3}/R$, hence $c_s^2=c_0^2/R$. Both the restoring [pressure](../../../../../pressure.md) term and the gravitational term are proportional to $R^{-3}$. Thus, in the exponential approximation,

$$
\boxed{\ddot\varepsilon+2\mu\dot\varepsilon+\eta^2e^{-3\mu\tau}\varepsilon=0,\qquad
\eta^2=c_0^2k^2-4\pi G\rho_0.}
$$

The sign of $\eta^2$ is the [Jeans instability](../../../../../jeans-instability.md) distinction, but exponential expansion makes the total subsequent amplification finite.

Remove [Hubble friction](../../../../../hubble-friction.md) by setting $\varepsilon=e^{-\mu\tau}y$. The standard-form equation is

$$
y''+Q(\tau)y=0,\qquad Q=\eta^2e^{-3\mu\tau}-\mu^2.
$$

Where $Q>0$ and $|Q'|\ll Q^{3/2}$, the [WKB approximation](../../../../../wkb-approximation.md) gives

$$
\varepsilon\simeq e^{-\mu\tau}Q^{-1/4}
\left[A\cos\!\left(\int^\tau\sqrt Q\,ds\right)+B\sin\!\left(\int^\tau\sqrt Q\,ds\right)\right].
$$

Where $Q<0$, put $q=\sqrt{-Q}$; away from a turning point the corresponding [WKB approximation](../../../../../wkb-approximation.md) is

$$
\varepsilon\simeq e^{-\mu\tau}q^{-1/2}
\left[A e^{\int^\tau q\,ds}+B e^{-\int^\tau q\,ds}\right],\qquad |q'|\ll q^2.
$$

For $\eta^2=-s^2<0$, $q=(\mu^2+s^2e^{-3\mu\tau})^{1/2}$ never vanishes. The exponential [integral](../../../../../integral.md) can be evaluated explicitly:

$$
\int_0^\tau q(t)\,dt=\frac{2}{3\mu}\bigl[\Psi(q(0))-\Psi(q(\tau))\bigr],\qquad
\Psi(q)=q+\frac{\mu}{2}\ln\frac{q-\mu}{q+\mu}.
$$

Differentiate this expression, using $q'=-3\mu(q^2-\mu^2)/(2q)$, to verify it. Early on, if coefficients change little over the interval considered, the two local exponents for $\varepsilon$ are $-\mu\pm\sqrt{\mu^2+s^2}$: one increases and one decreases. At late times $q\to\mu$ and the displayed [integral](../../../../../integral.md) is $\mu\tau+O(1)$. The nominally growing [WKB approximation](../../../../../wkb-approximation.md) branch of $y$ therefore becomes a constant branch of $\varepsilon$, while the other branch decays like $e^{-2\mu\tau}$. The [WKB approximation](../../../../../wkb-approximation.md) is not automatically accurate at all intermediate times; its stated derivative criterion must be checked.

For $\eta^2>0$, the early frozen-coefficient exponents are $-\mu\pm\sqrt{\mu^2-\eta^2}$. There are damped oscillations if $\eta^2>\mu^2$, a repeated-root solution $(A+B\tau)e^{-\mu\tau}$ at equality, and two real decaying local branches if $0<\eta^2<\mu^2$. In the oscillatory case $Q$ vanishes at $\tau_t=\ln(\eta^2/\mu^2)/(3\mu)$: the ordinary [WKB approximation](../../../../../wkb-approximation.md) breaks down there, and a turning-point connection is needed. After that transition the solutions again approach a constant or decay. A positive pressure-minus-gravity restoring term does not imply indefinitely continuing oscillation; its physical [frequency](../../../../../frequency.md) is redshifted away.

The limiting conclusion does not depend on the accuracy of [WKB approximation](../../../../../wkb-approximation.md). With $x=2|\eta|e^{-3\mu\tau/2}/(3\mu)$, the equation for $y$ is

$$
x^2y_{xx}+xy_x+\left(\operatorname{sgn}(\eta^2)x^2-\frac49\right)y=0.
$$

For $\eta^2>0$ its basis is $J_{2/3}(x),Y_{2/3}(x)$, the [Bessel functions of the first kind](../../../../../bessel-function-of-the-first-kind.md) and [Bessel functions of the second kind](../../../../../bessel-function-of-the-second-kind.md). For $\eta^2<0$ use $I_{2/3}(x),K_{2/3}(x)$, the [Modified Bessel functions of the first kind](../../../../../modified-bessel-function-of-the-first-kind.md) and [modified Bessel functions of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md). Their small-$x$ branches are proportional to $x^{2/3}$ and $x^{-2/3}$. Multiplication by $e^{-\mu\tau}$ gives the decaying and constant branches respectively. At $\eta^2=0$ the exact solution is $A+B e^{-2\mu\tau}$. Thus [Bessel density modes during exponential expansion](../../../../../bessel-density-modes-during-exponential-expansion.md) prove

$$
\boxed{\varepsilon(\tau)\longrightarrow\varepsilon_\infty\quad\text{for every finite initial pair and every real }\eta^2,\ \Lambda>0.}
$$

The same conclusion holds in the full four-thirds perturbation equation on an exponentially escaping background: $(R^2\dot\varepsilon)'=-\eta^2R^{-1}\varepsilon$. Its integrated equation has an absolutely integrable Volterra kernel, bounded by a constant times $e^{-3\mu\tau}$. The [Gronwall inequality](../../../../../gronwall-inequality.md) first bounds $\varepsilon$; then $R^{-1}\varepsilon$ is integrable and $\dot\varepsilon=O(R^{-2})$ is integrable. A finite limiting amplitude follows without setting $H$ exactly constant. This argument requires positive $\Lambda$ and the escaping branch; it is not a claim about $\Lambda=0$ or recollapse.

The requested strict increase of that limit needs an initial-velocity qualification. For $\eta^2=-s^2<0$,

$$
\left(e^{2\mu\tau}\dot\varepsilon\right)'=s^2e^{-\mu\tau}\varepsilon.
$$

If $\varepsilon(0)>0$ and $\dot\varepsilon(0)\geq0$, this identity prevents a first loss of positivity and makes the amplitude strictly increase for $\tau>0$. Integrating it twice gives

$$
\varepsilon_\infty=\varepsilon(0)+\frac{\dot\varepsilon(0)}{2\mu}
+\frac{s^2}{2\mu}\int_0^\infty e^{-3\mu\tau}\varepsilon(\tau)\,d\tau
>\varepsilon(0).
$$

This is [monotone Jeans growth with positive cosmological constant](../../../../../monotone-jeans-growth-with-positive-cosmological-constant.md). Without the extra initial condition the printed assertion is false: $\varepsilon=e^{-\mu\tau}I_{2/3}(2s e^{-3\mu\tau/2}/(3\mu))$ is positive at $\tau=0$ and tends to zero. An arbitrarily small multiple remains an infinitesimal [linear cosmological density perturbation](../../../../../linear-cosmological-density-perturbation-split.md), so linearity does not remove the counterexample.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
