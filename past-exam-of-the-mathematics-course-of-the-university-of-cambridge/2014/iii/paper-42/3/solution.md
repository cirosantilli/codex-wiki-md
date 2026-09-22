<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The parameters of a cutoff [statistical field theory](../../../../../statistical-field-theory.md) describe only the retained modes. Changing the [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) changes which fluctuations have already been integrated out, so its effective mass, interaction coefficients and gradient normalization must change to preserve the same long-distance physics. They are not separately cutoff-independent observables. Because the source's weight is $e^{-H}$, its [statistical Hamiltonian](../../../../../statistical-hamiltonian.md) is dimensionless, with the physical inverse-temperature factor already absorbed.

For example split the [scalar field](../../../../../scalar-field.md) into slow modes $\phi_<$ with $|p|<\Lambda/b$ and shell modes $\phi_>$ with $\Lambda/b<|p|<\Lambda$. Define the [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md) step by

$$
e^{-H_{\Lambda/b}^{\rm eff}[\phi_<]}=\int\mathcal D\phi_>\,e^{-H_\Lambda[\phi_<+\phi_>]}.
$$

This integrates out short-wavelength fluctuations exactly if all generated terms are retained. The new Hamiltonian can be expanded in local symmetry-allowed operators when the retained external momenta are well below the shell scale. A [cumulant expansion of a coarse-grained free energy](../../../../../cumulant-expansion-of-a-coarse-grained-free-energy.md) gives perturbative coefficients. Restoring the cutoff with $x'=x/b$ and, for a canonical gradient term, $\phi'(x')=b^{(D-2)/2}\phi_<(bx')$, gives $m^{2\prime}=b^2m^2+\cdots$ and $g'=b^{4-D}g+\cdots$. Interaction corrections also change the field normalization. Repeating the step produces the effective theory at successively longer distances.

To obtain the [LG theory](../../../../../landau-ginzburg-theory.md), assume a short-range scalar theory, slowly varying retained fields, analytic local couplings, positive gradient stiffness and stability, and a regime in which fluctuation corrections at the remaining scales are small. Keeping the leading gradient, quadratic and quartic operators gives a local [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md) functional. Its equilibrium in the [Landau approximation](../../../../../landau-approximation.md) is a uniform minimum, with a quadratic coefficient proportional to $T-T_c$ after the critical mass has been tuned. The [RG](../../../../../renormalization-group.md) explains why this is asymptotically consistent for the ordinary transition above four dimensions: the quartic interaction is irrelevant near the [Gaussian fixed point](../../../../../gaussian-fixed-point.md), while it must still be retained to stabilize the ordered phase. Below four dimensions it cannot be dropped in the asymptotic critical region; an interacting [Wilson-Fisher fixed point](../../../../../wilson-fisher-fixed-point.md) rather than the elementary saddle generally controls the transition. At four dimensions the interaction is marginal and produces logarithmic corrections. Tuning a quartic coefficient through zero requires a sextic stabilizing term and leads to tricriticality.

More concretely, in the Gaussian scaling regime let $u=g/6$ so the local quartic term is $u\phi^4/4$. At a total blocking scale $\ell$, the leading couplings are $r'=\ell^2r$, $u'=\ell^{4-D}u$, $h'=\ell^{(D+2)/2}h$. Apply the saddle approximation to the blocked potential and multiply its minimum by $\ell^{-D}$ to convert back to original volume units. Rescaling the saddle field by $(|r'|/u')^{1/2}$ gives

$$
\ell^{-D}\frac{r'^2}{u'}f_\pm\left(\frac{h'\sqrt{u'}}{|r'|^{3/2}}\right)
=\boxed{\frac{r^2}{u}f_\pm\left(\frac{h\sqrt u}{|r|^{3/2}}\right)}.
$$

All blocking-scale factors cancel. This explicitly recovers [mean-field scalar free-energy scaling](../../../../../mean-field-scalar-free-energy-scaling.md) with $r\propto t$. Although $u'\to0$ above four dimensions, the saddle [free energy](../../../../../thermodynamic-free-energy.md) is proportional to $1/u'$; setting it to zero before minimization would remove the ordered phase. This is the [dangerously irrelevant coupling](../../../../../dangerously-irrelevant-coupling.md) mechanism rather than homogeneous two-variable hyperscaling.

For the perturbative calculation make the source's kinetic convention explicit. Write $K=\alpha^{-1}>0$. The [canonical normalization of a scalar gradient term](../../../../../canonical-normalization-of-a-scalar-gradient-term.md) uses $\psi=\sqrt K\phi$, so the canonical quadratic and quartic coefficients are $r/K$ and $g/K^2$. In what follows $m^2,g$ denote those canonical coefficients; then the reference propagator has denominator $p^2+M^2$. Without this normalization the propagator denominator is $Kp^2+r$, and the unmodified printed integral would not apply. At one loop the quartic tadpole is momentum independent, so it produces no gradient renormalization at this order.

In the convention fixed by the displayed equation, the truncated two-point function is the [one-particle-irreducible two-point vertex](../../../../../one-particle-irreducible-two-point-vertex.md), not the connected two-point cumulant itself. If $W[J]=\log Z[J]$ and $\Gamma[\varphi]=\int J\varphi-W[J]$ is the [Legendre transform](../../../../../convex-conjugate.md), then its second derivative is the inverse of $W^{(2)}=G$. For a translation-invariant background,

$$
\boxed{\widetilde\Gamma(p)=\widetilde G(p)^{-1}.}
$$

Decompose the canonically normalized [statistical Hamiltonian](../../../../../statistical-hamiltonian.md) into a Gaussian part of mass $M^2$, a mass counterterm $\delta m^2=m^2(\Lambda,T)-M^2$, and the quartic interaction $g\phi^4/4!$. With the Euclidean sign convention in which a positive mass correction increases the inverse propagator, the [self-energy](../../../../../self-energy.md) expansion is

$$
\boxed{\widetilde\Gamma(p)=\widetilde G_0^{-1}(p)+\delta m^2+\Sigma(p),\qquad
\widetilde G_0(p)=\frac1{p^2+M^2}.}
$$

Here $\Sigma$ contains loop corrections from proper two-point diagrams, excluding the separately displayed mass counterterm. The corresponding connected propagator begins $G=G_0-G_0(\delta m^2+\Sigma)G_0+\cdots$. This fixes the sign, which would be reversed if “[self-energy](../../../../../self-energy.md)” instead denoted the insertion added with a plus sign inside a Dyson series.

The one-loop proper diagram is the [tadpole diagram](../../../../../tadpole-diagram.md). Attaching two external fields to the quartic vertex gives $4\cdot3$ contractions, divided by $4!$, so its symmetry factor is $1/2$. With the loop momentum restricted by the cutoff,

$$
\Sigma^{(1)}(p)=\frac g2I_D(M^2;\Lambda),\qquad
I_D(R;\Lambda)=\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{q^2+R}.
$$

It is independent of external momentum. Impose the zero-momentum mass condition $M^2=\widetilde\Gamma(0)=m^2(0,T)$. This gives $\delta m^2+(g/2)I_D(M^2;\Lambda)=0$, hence

$$
\boxed{m^2(0,T)=m^2(\Lambda,T)+\frac g2\int_{|p|<\Lambda}\frac{d^Dp}{(2\pi)^D}\frac1{p^2+m^2(0,T)}.}
$$

This is the one-loop relation using a renormalized mass in the reference propagator, or the corresponding self-consistent tadpole approximation if solved without expanding in $g$. It is not an exact all-orders gap equation. Away from the critical infrared problem, replacing the loop mass by the bare one changes a strict perturbative result only at higher order.

Take $g>0$ smooth and nonzero for an ordinary stable quartic transition. To test the assumed linear thermal mass, work from the disordered side and put $R=m^2(0,T)>0$. For $D>2$, $I_D(0;\Lambda)$ is infrared finite. The critical bare mass is shifted, not generically zero: $m^2(\Lambda,T_c)=-(g/2)I_D(0;\Lambda)$. Absorb the smooth temperature dependence of couplings into an analytic thermal tuning $\tau=A_t(T-T_c)+\cdots$, with $A_t>0$. Critical subtraction gives the [one-loop critical-mass subtraction](../../../../../one-loop-critical-mass-subtraction.md)

$$
\tau=R+\frac g2\{I_D(0;\Lambda)-I_D(R;\Lambda)\}
=R\left[1+\frac g2J_D(R)\right],
$$

where

$$
J_D(R)=K_D\int_0^\Lambda\frac{p^{D-3}\,dp}{p^2+R},\qquad
K_D=\frac{S_{D-1}}{(2\pi)^D}>0.
$$

The [infrared asymptotics of the critical-mass subtraction](../../../../../infrared-asymptotics-of-the-critical-mass-subtraction.md) now distinguish the dimensions. For $D>4$, $J_D(0)=K_D\Lambda^{D-4}/(D-4)$ is finite, so

$$
R\sim\frac{\tau}{1+(g/2)J_D(0)}\propto T-T_c.
$$

For $D=4$, $J_4(R)=(K_4/2)\log[(\Lambda^2+R)/R]$ diverges logarithmically. For $2<D<4$, substitution $p=\sqrt R\,q$ gives

$$
J_D(R)\sim K_DR^{(D-4)/2}\int_0^\infty\frac{q^{D-3}\,dq}{1+q^2},
$$

so the correction to $\tau$ scales as $R^{(D-2)/2}$ and dominates the analytic linear term. **Pure mean-field linear mass scaling is therefore consistent only above**

$$
\boxed{D_c=4\quad\text{for the ordinary scalar quartic transition}.}
$$

At the boundary dimension logarithms modify the simple power law. Below it this calculation diagnoses the failure of the Gaussian expansion; the exponent obtained by treating the self-consistent one-loop equation as exact is not automatically the exponent of the interacting scalar theory. For $D\leq2$, the massless subtraction itself has an infrared divergence, so this perturbative argument cannot establish absence of a transition. In particular it does not rule out the two-dimensional Ising critical point.

The same upper dimension follows by [engineering dimension](../../../../../engineering-dimension.md) counting: a canonical [scalar field](../../../../../scalar-field.md) has dimension $(D-2)/2$, so $[g]=D-4(D-2)/2=4-D$. For a [tricritical point](../../../../../tricritical-point.md) tune the renormalized quadratic and quartic terms to zero and retain a positive sextic interaction $v\phi^6$. Its [engineering dimension](../../../../../engineering-dimension.md) is

$$
[v]=D-6(D-2)/2=6-2D.
$$

It is marginal at **$D_c=3$**, irrelevant above three, and relevant below three. More generally the [upper critical dimension of an even scalar interaction](../../../../../upper-critical-dimension-of-an-even-scalar-interaction.md) $\phi^{2n}$ is $2n/(n-1)$.

A [Ginzburg criterion](../../../../../ginzburg-criterion.md) check gives the same result: at tricritical mean-field scaling $m_0^2\sim|t|^{1/2}$ and $\xi\sim|t|^{-1/2}$, whereas fluctuations in a correlation volume scale as $\xi^{2-D}\sim|t|^{(D-2)/2}$. Their ratio to $m_0^2$ is $|t|^{(D-3)/2}$, which tends to zero only for $D>3$. Thus

$$
\boxed{D_c^{\rm ordinary}=4,\qquad D_c^{\rm tricritical}=3.}
$$

The tricritical tuning concerns renormalized couplings: shell contractions of a sextic term can regenerate quadratic and quartic terms even when their bare coefficients vanish. At three dimensions the marginal sextic coupling produces logarithmic corrections rather than a strictly fluctuation-free mean-field limit.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
