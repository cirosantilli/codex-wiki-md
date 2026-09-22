<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Pound-Rebka experiment](../../../../../pound-rebka-experiment.md) measures a small [gravitational redshift](../../../../../gravitational-redshift.md) by comparing nuclear emission and resonant absorption at different heights in Earth's field. The $14.4\,\mathrm{keV}$ transition of iron-57 supplies the gamma-ray frequency standard. The [Mössbauer effect](../../../../../mossbauer-effect.md) permits recoil-free emission and absorption by nuclei bound in solids, giving a sufficiently narrow resonance. A source and absorber separated vertically by about $22.6\,\mathrm m$ have a predicted fractional frequency difference of order $2.5\times10^{-15}$. A calibrated [Doppler effect](../../../../../doppler-effect.md) from slow source motion measures the shift through its effect on resonant absorption. Interchanging the upper and lower arrangements reverses the gravitational contribution and helps separate it from intrinsic source-absorber offsets; temperature-dependent frequency shifts must also be controlled. The observed change agrees with the weak-field prediction.

The prediction follows either from an accelerating laboratory and the [Equivalence principle](../../../../../equivalence-principle.md), or directly from a static metric. With $x^0=ct$, write $g_{00}=N^2\simeq1+2\Phi/c^2$. The time-translation [Killing vector field](../../../../../killing-vector-field.md) gives a conserved photon energy $E_\xi=p_a\xi^a$, while a static observer has [four-velocity](../../../../../four-velocity.md) $u^a=\xi^a/N$ and measures $h\nu=E_\xi/N$. Thus

$$
\boxed{\frac{\nu_{\rm received}}{\nu_{\rm emitted}}
=\frac{N_{\rm emitted}}{N_{\rm received}}
\simeq1+\frac{\Phi_{\rm emitted}-\Phi_{\rm received}}{c^2}.}
$$

For an upward ray over height $H$, $\Delta\nu/\nu\simeq-gH/c^2$; downward propagation has the opposite sign. The equivalent compensating Doppler speed has magnitude $gH/c$, about $7.4\times10^{-7}\,\mathrm{m\,s^{-1}}$ for this baseline. Identical clocks at rest have $d\tau=N\,dt$, so a clock at higher potential runs faster relative to the common static coordinate time. This does not mean that the nuclear transition changes its locally measured frequency with height: the comparison involves transporting a photon between different local proper-time standards.

The [weak equivalence principle](../../../../../weak-equivalence-principle.md) asserts universal free fall for test bodies. The [Einstein equivalence principle](../../../../../einstein-equivalence-principle.md) adds [local Lorentz invariance](../../../../../local-lorentz-invariance.md) and [local position invariance](../../../../../local-position-invariance.md) for nongravitational experiments in a freely falling laboratory. The redshift comparison tests the clock aspect of local position invariance and supports a metric description of gravity. The [strong equivalence principle](../../../../../strong-equivalence-principle.md) extends these requirements to self-gravitating bodies and local gravitational experiments, including the contribution of gravitational binding energy. Their outcomes should be independent of the external location and motion of a freely falling laboratory when tidal effects are negligible. A nuclear redshift experiment is therefore not a test of the whole strong equivalence principle, and its success does not uniquely establish the gravitational field equations.

The geometrical realization uses the [Levi-Civita connection](../../../../../levi-civita-connection.md) of a spacetime metric. At any event, [normal coordinates](../../../../../normal-coordinates.md) make $g_{ab}=\eta_{ab}$ and the [Christoffel symbols](../../../../../christoffel-symbol.md) vanish. Freely falling test particles follow [geodesics](../../../../../geodesic.md); local nongravitational equations take their special-relativistic form at that event. The [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) need not vanish, so finite laboratories can measure tidal [geodesic deviation](../../../../../geodesic-deviation.md). The strong principle concerns removing a uniform external gravitational field locally, not removing curvature throughout an extended region.

For a [perfect fluid](../../../../../perfect-fluid.md), local rest-frame isotropy and the absence of heat flux or viscosity give $T^{\hat a\hat b}=\operatorname{diag}(\rho,p,p,p)$, where $\rho$ is rest-frame energy density. With the PDF's signature $(+---)$, $u^au_a=1$ and $h^{ab}=g^{ab}-u^au^b$ projects spatially. Its covariant form is

$$
\boxed{T^{ab}=\rho u^au^b-ph^{ab}=(\rho+p)u^au^b-pg^{ab}.}
$$

The pressure sign follows from the negative spatial metric; it gives positive diagonal stresses in the rest frame. Local [stress-energy conservation](../../../../../stress-energy-conservation.md), $\nabla_aT^{ab}=0$, produces the two projections

$$
u^a\nabla_a\rho+(\rho+p)\nabla_au^a=0,\qquad
(\rho+p)u^a\nabla_au^b=(g^{ba}-u^bu^a)\nabla_ap.
$$

The first is the energy equation, including pressure work; the second is the [relativistic Euler equation](../../../../../relativistic-euler-equation.md). Its rest-frame spatial pressure force is $-\nabla p$.

Further assumptions are needed to derive the [Einstein field equations](../../../../../einstein-field-equations.md). Take a local generally covariant metric equation, linear in curvature and of second differential order, and demand compatibility with [stress-energy conservation](../../../../../stress-energy-conservation.md). The available rank-two tensors are $R_{ab}$, $Rg_{ab}$ and a constant multiple of $g_{ab}$. Defining $R_{ab}=R^c{}_{acb}$, the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) gives $\nabla^aR_{ab}=\tfrac12\nabla_bR$. Hence the combination $R_{ab}+\alpha Rg_{ab}$ is identically divergence-free only when $\alpha=-\tfrac12$. This determines the [Einstein tensor](../../../../../einstein-tensor.md) $G_{ab}=R_{ab}-Rg_{ab}/2$; a [cosmological constant](../../../../../cosmological-constant.md) term remains allowed.

The coupling sign must be matched to the actual curvature convention. Here $R^a{}_{bcd}$ represents $[\nabla_d,\nabla_c]$, and a static weak field has $R_{00}\simeq-\nabla^2\Phi/c^2$. With negligible pressure and cosmological term, a trial equation $G_{ab}=C T_{ab}$ implies $R_{00}\simeq C\rho_{\rm mass}c^2/2$. Comparing with the [Poisson equation](../../../../../poisson-equation.md) $\nabla^2\Phi=4\pi G\rho_{\rm mass}$ fixes $C=-8\pi G/c^4$. Thus the [Einstein equation in the sequential-derivative curvature convention](../../../../../einstein-equation-in-the-sequential-derivative-curvature-convention.md) is

$$
\boxed{G_{ab}+\Lambda g_{ab}=-\frac{8\pi G}{c^4}\left[(\rho+p)u_au_b-pg_{ab}\right].}
$$

Equivalently, $R_{ab}=\Lambda g_{ab}-(8\pi G/c^4)(T_{ab}-Tg_{ab}/2)$, with $T=\rho-3p$. Pressure therefore gravitates as well as supplying a material force. The cosmological constant is not fixed by the local Newtonian matching.

Setting $c=1$ for the action normalization, the same metric equation follows from the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) $S_g=(2\kappa)^{-1}\int\sqrt{-g}(R-2\Lambda)\,d^4x$, where $\kappa=8\pi G$, together with a matter action obeying $\delta S_m=\tfrac12\int\sqrt{-g}T_{ab}\delta g^{ab}\,d^4x$. After the metric boundary term is removed or supplied separately, the bulk variation is proportional to $G_{ab}+\Lambda g_{ab}+\kappa T_{ab}$. This also makes the sign convention explicit. General covariance, the field equation and the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) are mutually consistent with the fluid conservation laws. The experiment motivates the local metric description; the curvature and conservation assumptions, plus the Newtonian limit, supply the additional route to the field equation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
