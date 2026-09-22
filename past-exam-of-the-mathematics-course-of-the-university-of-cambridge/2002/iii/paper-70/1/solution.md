<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) signature $(+,-)$ and put $\kappa=|\lambda|>0$. The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) for the real [scalar field](../../../../../scalar-field.md) is

$$
\boxed{\phi_{tt}-\phi_{xx}+2\kappa^2\phi(\phi^2-1)=0.}
$$

Indeed, differentiating the potential $U(\phi)=\kappa^2(\phi^2-1)^2/2$ gives $U'=2\kappa^2\phi(\phi^2-1)$, while the kinetic term contributes $\partial_\mu\partial^\mu\phi$.

Translation invariance gives the symmetric [stress-energy tensor](../../../../../stress-energy-tensor.md)

$$
T^{\mu\nu}=\partial^\mu\phi\,\partial^\nu\phi
-\eta^{\mu\nu}\mathcal L.
$$

Its divergence is $(\partial_\mu\partial^\mu\phi+U')\partial^\nu\phi$, which vanishes by the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md). Consequently the conserved [energy](../../../../../energy.md) and physical spatial [momentum](../../../../../momentum.md) are

$$
\boxed{E=\int_{\mathbb R}\left[\frac12\phi_t^2+\frac12\phi_x^2+
\frac{\kappa^2}{2}(\phi^2-1)^2\right]dx,\qquad
P=-\int_{\mathbb R}\phi_t\phi_x\,dx.}
$$

The minus sign in $P=\int T^{01}dx$ follows from $\partial^1=-\partial_x$. Conservation assumes the associated stress-energy fluxes vanish at spatial infinity, as they do for the localized fields below.

A static [finite-energy field configuration](../../../../../finite-energy-field-configuration.md) approaches vacua $\phi=\pm1$. Multiplying $\phi''=U'(\phi)$ by $\phi'$ gives

$$
\frac12\phi'^2-U(\phi)=\text{constant}=0,
$$

where the vacuum limits fix the constant. For a [kink](../../../../../scalar-field-kink.md) increasing from $-1$ to $1$, $\phi'=\kappa(1-\phi^2)$. Integration gives $\operatorname{artanh}\phi=\kappa(x-X)$ and hence

$$
\boxed{\phi_{\mathrm K}(x)=\tanh[\kappa(x-X)].}
$$

Its negative is the [antikink](../../../../../antikink.md). The arbitrary center $X$ is a translational [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md). The static [kink](../../../../../scalar-field-kink.md) mass is its rest [energy](../../../../../energy.md); using $\phi'^2=2U$ and $y=\kappa(x-X)$ gives

$$
M=\int_{\mathbb R}\phi'^2dx
=\kappa\int_{-\infty}^{\infty}\operatorname{sech}^4y\,dy
=\kappa\int_{-1}^{1}(1-z^2)\,dz
=\boxed{\frac{4\kappa}{3}}.
$$

Equivalently, completing the static [energy](../../../../../energy.md) into a square gives $E=\frac12\int[\phi'-\kappa(1-\phi^2)]^2dx+\kappa[\phi-\phi^3/3]_{-\infty}^{\infty}$, so this [kink](../../../../../scalar-field-kink.md) saturates its [Bogomolny bound](../../../../../bogomolny-bound.md).

A [Lorentz boost](../../../../../lorentz-boost.md) with velocity $v$ gives

$$
\boxed{\phi(t,x)=\tanh[\kappa\gamma(x-X-vt)],
\qquad \gamma=(1-v^2)^{-1/2}.}
$$

Writing $z=\gamma(x-X-vt)$, the derivatives are $\phi_t=-\gamma v\phi_{\mathrm K}'(z)$ and $\phi_x=\gamma\phi_{\mathrm K}'(z)$. The [momentum](../../../../../momentum.md) integral therefore becomes

$$
P=\gamma^2v\int\phi_{\mathrm K}'(z)^2\,\frac{dz}{\gamma}
=\boxed{\gamma Mv}.
$$

The boosted [energy](../../../../../energy.md) is

$$
E=\frac12\left[\gamma(1+v^2)+\gamma^{-1}\right]
\int\phi_{\mathrm K}'(z)^2dz
=\boxed{\gamma M},
$$

because $\gamma^{-1}=\gamma(1-v^2)$. Thus $E^2-P^2=M^2$ and $P/E=v$, exactly the [energy–momentum relation](../../../../../energy-momentum-relation.md) of a relativistic particle of rest mass $4\kappa/3$. This is the [relativistic energy and momentum of a phi-four kink](../../../../../relativistic-energy-and-momentum-of-a-phi-four-kink.md). If $\lambda=0$, the double-well potential disappears and there is no localized static kink connecting these vacua.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
