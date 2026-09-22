<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In units $\hbar=c=1$, the [action](../../../../../action.md) is dimensionless and a [Lagrangian density](../../../../../lagrangian-density.md) has [mass dimension](../../../../../mass-dimension.md) $d$. The kinetic term therefore gives $2+2[\phi]=d$. Requiring each interaction density $g_n\phi^n$ to have the same dimension gives

$$
\boxed{[\phi]=\frac d2-1,\qquad[g_n]=d_n=d-n\left(\frac d2-1\right)=n-d\left(\frac n2-1\right).}
$$

This is engineering dimension; quantum scaling can acquire an [anomalous dimension](../../../../../anomalous-dimension.md).

For a connected [Feynman diagram](../../../../../feynman-diagram.md) with no derivative interactions, each independent loop integration contributes $d$ powers of [momentum](../../../../../momentum.md), and each internal [scalar propagator](../../../../../scalar-propagator.md) contributes $-2$. Thus its [superficial degree of divergence](../../../../../superficial-degree-of-divergence.md) is $D=dL-2I$. Let $V=\sum_nV_n$. A connected graph has $L=I-V+1$ independent cycles, and counting the half-edges incident on vertices gives $2I+E=\sum_n nV_n$. Substitution proves the [scalar graph power-counting identity](../../../../../scalar-graph-power-counting-identity.md):

$$
\begin{aligned}
D&=d+(d-2)I-d\sum_nV_n\\
&=d-\left(\frac d2-1\right)E
+\sum_n\left[n\left(\frac d2-1\right)-d\right]V_n\\
&=\boxed{d-\left(\frac d2-1\right)E-\sum_n d_nV_n.}
\end{aligned}
$$

For a graph with $C$ connected components, the first $d$ is instead $dC$, since $L=I-V+C$. The printed expression therefore uses the usual connected-graph convention. This is the overall degree under simultaneous rescaling of all [loop momenta](../../../../../loop-momentum.md). Subgraphs can still have [ultraviolet divergences](../../../../../ultraviolet-divergence.md) when the whole graph has $D<0$, so their [counterterms](../../../../../counterterm.md) must be subtracted before declaring an integral finite.

When all retained couplings have nonnegative dimension, only finitely many external-leg/derivative structures can have nonnegative degree. Positive-dimensional [relevant couplings](../../../../../relevant-coupling.md) lower $D$ as vertices are added, giving superrenormalizable interactions. Zero-dimensional [marginal couplings](../../../../../marginal-coupling.md) give power-counting renormalizable interactions. Negative-dimensional [irrelevant couplings](../../../../../irrelevant-coupling.md) instead permit $D$ to grow with the number of vertices, generally requiring an unbounded list of [counterterms](../../../../../counterterm.md). Such [nonrenormalizable interactions](../../../../../nonrenormalizable-interaction.md) can still define an [effective field theory](../../../../../effective-field-theory.md) to any fixed order in a low-energy expansion.

In $d=4$, $d_n=4-n$: cubic interactions are superrenormalizable, quartic interactions are marginal and renormalizable, and powers $n\geq5$ are nonrenormalizable. In $d=3$, $d_n=3-n/2$: cubic, quartic and quintic interactions are superrenormalizable, sixth-order interactions are marginal and renormalizable, and $n\geq7$ are nonrenormalizable. This is a power-counting classification, not a guarantee that an odd highest-power potential is bounded below. All lower-dimensional operators allowed by the symmetries must be included when required by [renormalization](../../../../../renormalization.md); for example, odd interactions can require a linear [counterterm](../../../../../counterterm.md), whereas the quartic model's $\phi\mapsto-\phi$ symmetry excludes it.

[Dimensional regularization](../../../../../dimensional-regularization.md) defines convergent Euclidean loop integrals in a suitable domain of $\operatorname{Re}d$, then continues their parameter formulas meromorphically to complex $d$. The Gaussian identity supplies $(4\pi)^{-d/2}$ and [Schwinger parameterization](../../../../../schwinger-parameterization.md) supplies Gamma functions such as $\Gamma(n-d/2)$. Their poles encode the ultraviolet singularities near physical dimension. Noninteger complex $d$ is an analytic regulator of amplitudes, not a literal space with a noninteger number of coordinates. Masses or nonexceptional external momenta distinguish ultraviolet poles from infrared poles; scaleless integrals vanish in this convention and can hide that distinction.

For the quartic model let $d=4-\epsilon$, $\phi_0=Z^{1/2}\phi$, $m_0^2=Z_{m^2}m^2$ and $\lambda_0=\mu^\epsilon Z_\lambda\lambda$. In renormalized fields, the bare Lagrangian is

$$
\mathcal L_0=-\frac12Z(\partial\phi)^2-\frac12ZZ_{m^2}m^2\phi^2
-\frac{\mu^\epsilon\lambda}{4!}Z^2Z_\lambda\phi^4.
$$

Separate the terms with each $Z$ equal to one from their differences. The differences are field, [mass](../../../../../mass.md) and quartic [counterterms](../../../../../counterterm.md). After subtracting divergent subgraphs, the remaining ultraviolet pole of a proper graph is a local polynomial in its external momenta. In four-dimensional [phi-fourth theory](../../../../../quartic-interaction.md), power counting and reflection symmetry restrict these local terms to $(\partial\phi)^2$, $\phi^2$, $\phi^4$ and a field-independent constant. Choosing the Laurent coefficients of the three [renormalization](../../../../../renormalization.md) factors recursively cancels these poles at every perturbative order. The constant vacuum term is removed by the zero-source normalization. This is an order-by-order finite renormalized expansion, not a claim of convergence of the perturbation series.

The [source renormalization of a scalar generating functional](../../../../../source-renormalization-of-a-scalar-generating-functional.md) follows directly from rewriting the [source](../../../../../source-quantum-field-theory.md) coupling in bare variables:

$$
\mu^{-\epsilon/2}h\phi=h_0\phi_0,\qquad
\boxed{h_0=\mu^{-\epsilon/2}Z^{-1/2}h.}
$$

A general [source](../../../../../source-quantum-field-theory.md) attached to a single elementary field needs this field [renormalization](../../../../../renormalization.md); its connected correlations are the ordinary renormalized Green functions. Normalizing the [path integral](../../../../../path-integral.md) at $h=0$ cancels source-independent vacuum diagrams. Subject to a separate infrared/volume prescription, their source-dependent [generating functional](../../../../../generating-functional.md) $F$ is consequently ultraviolet finite order by order. For a constant [source](../../../../../source-quantum-field-theory.md), this statement is interpreted as a formal connected expansion or a vacuum density, not as an automatically finite total logarithm in infinite [spacetime](../../../../../spacetime.md).

Changing integration variables from $\phi$ to $\phi_0$ introduces a source-independent constant Jacobian that cancels between the numerator and its normalization. The resulting normalized integral depends only on $\lambda_0,m_0^2,h_0$ and fixed physical boundary/volume data. Thus

$$
\left.\mu\frac{dF}{d\mu}\right|_{\lambda_0,m_0^2,h_0}=0.
$$

Define all scale derivatives at these fixed bare quantities:

$$
\widehat\beta(\lambda)=\mu\frac{d\lambda}{d\mu},\qquad
\gamma_{m^2}(\lambda)=\mu\frac{d\log m^2}{d\mu},\qquad
\widehat\gamma_h(\lambda)=\mu\frac{d\log h}{d\mu}.
$$

In a mass-independent subtraction scheme, logarithmic differentiation of the bare relations gives

$$
\boxed{\widehat\beta=-\frac{\epsilon\lambda}{1+\lambda\partial_\lambda\log Z_\lambda},\qquad
\gamma_{m^2}=-\widehat\beta\,\partial_\lambda\log Z_{m^2},\qquad
\widehat\gamma_h=\frac\epsilon2+\frac{\widehat\beta}{2}\partial_\lambda\log Z.}
$$

The factors contain regulator poles, but the combinations determining the physical [renormalization group](../../../../../renormalization-group.md) functions have finite limits. In particular $\widehat\beta=-\epsilon\lambda+\beta(\lambda)$ and $\widehat\gamma_h=\epsilon/2+\gamma_\phi(\lambda)$. The [chain rule](../../../../../chain-rule.md) now gives the requested equation:

$$
\boxed{\left(\mu\partial_\mu+\widehat\beta\partial_\lambda
+\gamma_{m^2}m^2\partial_{m^2}+\widehat\gamma_hh\partial_h\right)F=0.}
$$

As a sign check, minimal subtraction gives $Z_{m^2}=1+\lambda/(16\pi^2\epsilon)+O(\lambda^2)$ and $Z_\lambda=1+3\lambda/(16\pi^2\epsilon)+O(\lambda^2)$, with $Z=1+O(\lambda^2)$. Hence $\beta=3\lambda^2/(16\pi^2)+O(\lambda^3)$, $\gamma_{m^2}=\lambda/(16\pi^2)+O(\lambda^2)$, and $\gamma_\phi$ starts at two loops. The positive signs agree with the tadpole subtraction and the three four-point channels.

The dimensional rewriting needs care. The chosen [source](../../../../../source-quantum-field-theory.md) normalization gives $[h]=3$, $[m^2]=2$, and $[\lambda]=0$, so $m^2/\mu^2$ and $h/\mu^3$ are the natural dimensionless parameters. For the full [source](../../../../../source-quantum-field-theory.md) [functional](../../../../../functional.md), [spacetime](../../../../../spacetime.md) arguments must also be rescaled: with $y=\mu x$, write $\phi(x)=\mu^{(d-2)/2}\psi(y)$ and $\widetilde h(y)=\mu^{-3}h(y/\mu)$. The dimensionless [functional](../../../../../functional.md) then depends on $\lambda,m^2/\mu^2$, the rescaled [source](../../../../../source-quantum-field-theory.md) profile, and the rescaled integration domain.

For a literal uniform [source](../../../../../source-quantum-field-theory.md) in a fixed physical [spacetime](../../../../../spacetime.md) volume $\mathcal V_d$, the [uniform-source vacuum functional and spacetime volume](../../../../../uniform-source-vacuum-functional-and-spacetime-volume.md) relation is instead

$$
\boxed{F=\mathcal V_d\mu^d f\left(\lambda,\frac{m^2}{\mu^2},\frac h{\mu^3}\right).}
$$

For example, even at $\lambda=0$ and $m^2>0$, completing the square for the constant mode gives

$$
F_0=\frac{\mathcal V_d\mu^{-\epsilon}h^2}{2m^2}
=\frac{\mathcal V_d\mu^d}{2}\frac{(h/\mu^3)^2}{m^2/\mu^2}.
$$

Thus the printed three-argument rewriting of the total $F$ suppresses necessary volume/source-profile data. It is valid as a dimensional shorthand only with those data understood; a dimensionless density has the three arguments, while its scale equation includes its engineering dimension. At infinite volume, the total constant-source logarithm is generally extensive and infinite even after ultraviolet [renormalization](../../../../../renormalization.md).

The [massless renormalization-group characteristics with a source](../../../../../massless-renormalization-group-characteristics-with-a-source.md) solve the requested flow directly, independently of this notational issue. Since the [mass](../../../../../mass.md) flow is proportional to $m^2$, its zero value remains zero. Starting at a reference scale $\mu_*$, solve

$$
\frac{d\lambda(\mu)}{d\log\mu}=\widehat\beta(\lambda(\mu)),\qquad
\frac{dh(\mu)}{d\log\mu}=\widehat\gamma_h(\lambda(\mu))h(\mu).
$$

Then

$$
\boxed{F(\lambda(\mu),0,h(\mu);\mu)=F(\lambda(\mu_*),0,h(\mu_*);\mu_*),}
$$

with any physical volume or source-shape data retained. Where $\widehat\beta\ne0$, the running quantities are determined by

$$
\log\frac\mu{\mu_*}=\int_{\lambda_{\rm ref}}^{\lambda(\mu)}\frac{dg}{\widehat\beta(g)},\qquad
h(\mu)=h_{\rm ref}\exp\left(\int_{\lambda_{\rm ref}}^{\lambda(\mu)}\frac{\widehat\gamma_h(g)}{\widehat\beta(g)}\,dg\right).
$$

These equations transport matching data at one scale to any other scale on the same flow trajectory. At a zero of the beta function use the differential equations themselves, rather than divide by zero.

For the uniform-source density, set $y=h/\mu^3$ and $m^2=0$. At $d=4$ the corrected dimensionless equation and its local characteristic solution are

$$
\left[\beta(\lambda)\partial_\lambda+(\gamma_h(\lambda)-3)y\partial_y+4\right]f(\lambda,y)=0,
$$



$$
f(\lambda,y)=\exp\left[-\int^{\lambda}\frac{4\,dg}{\beta(g)}\right]
\Psi\left(y\exp\left[-\int^{\lambda}\frac{\gamma_h(g)-3}{\beta(g)}\,dg\right]\right).
$$

The arbitrary function $\Psi$ is fixed by boundary/matching data. If the volume is retained as a dimensionless argument $v=\mu^4\mathcal V_4$, the full dimensionless [functional](../../../../../functional.md) obeys the same transport operator with $4v\partial_v$ in place of the additive $4$ term; extensivity makes the two statements equivalent. Massless zero-momentum [source](../../../../../source-quantum-field-theory.md) expansions can also have infrared singularities, so this RG solution is formal until an infrared prescription or a suitable background expansion is chosen.

An [ultraviolet fixed point](../../../../../ultraviolet-fixed-point.md) is a zero of the beta functions approached by the dimensionless couplings as $\mu\to\infty$. Near a single-coupling fixed point $\lambda_*$, perturbations obey $\delta\lambda\propto\mu^{\beta'(\lambda_*)}$, so $\beta'<0$ gives attraction in that direction. In four-dimensional quartic scalar theory, the positive one-loop beta function makes positive small coupling grow toward the ultraviolet: $1/\lambda(\mu)=1/\lambda(\mu_*)-[3/(16\pi^2)]\log(\mu/\mu_*)$. This exhibits a perturbative [Landau pole](../../../../../landau-pole.md), not an interacting [ultraviolet fixed point](../../../../../ultraviolet-fixed-point.md). A perturbative result does not exclude hypothetical strong-coupling behavior beyond its regime.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
