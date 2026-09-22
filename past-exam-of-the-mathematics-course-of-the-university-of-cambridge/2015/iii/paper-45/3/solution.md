<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the convention implied by the printed expansion, the truncated two-point quantity is the inverse connected propagator, or [one-particle-irreducible two-point vertex](../../../../../one-particle-irreducible-two-point-vertex.md):

$$
\boxed{\widetilde\Gamma(p)=\widetilde G(p)^{-1}.}
$$

It is the second functional derivative of the [quantum effective action](../../../../../effective-action.md) (or statistical Legendre effective action) about a translationally invariant zero-field equilibrium. The relation follows from the [inverse Hessian relation for a connected two-point function](../../../../../inverse-hessian-relation-for-a-connected-two-point-function.md). The subscript $c$ in $G$ already removes disconnected one-point products; the word “truncated” here is not a request to subtract that product a second time. Nor is a general [amputated connected correlation function](../../../../../amputated-connected-correlation-function.md) interchangeable with a [one-particle-irreducible correlation function](../../../../../one-particle-irreducible-correlation-function.md).

Use the [zero-momentum renormalized mass](../../../../../zero-momentum-renormalized-mass.md) $R=m^2(0,T)$ in the free propagator $\widetilde G_0(p)=(p^2+R)^{-1}$, and split the quadratic coupling into $R$ plus a [mass counterterm](../../../../../mass-counterterm.md) $\delta m^2=m^2(\Lambda,T)-R$. The [self-energy](../../../../../self-energy.md) $\Sigma(p)$ is the sum of loop 1PI insertions, excluding the separately displayed counterterm. Summing repeated insertions by [Dyson resummation](../../../../../dyson-resummation.md) gives

$$
\boxed{\widetilde\Gamma(p)=p^2+R+\delta m^2+\Sigma(p)
=\widetilde G_0(p)^{-1}+\delta m^2+\Sigma(p).}
$$

The sign convention is that a positive tadpole shifts the inverse propagator upwards. At first order, the [connected correlation function](../../../../../connected-correlation-function.md) correction is $-G_0^2\Sigma$, consistent with this inverse-propagator convention. A different split between the reference mass and counterterm produces the same renormalized result.

For the positive quartic interaction $g\phi^4/4!$, the one-loop [tadpole diagram](../../../../../tadpole-diagram.md) has no external-momentum dependence. Its symmetry factor is $1/2$: assigning the two external legs to four vertex fields gives $4\cdot3$ contractions, and division by $4!$ gives $1/2$. With the dimensionless statistical-action convention,

$$
\Sigma_1(p)=\frac g2 I_D(R),\qquad
I_D(R)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2+R}.
$$

The physical zero-momentum condition $\widetilde\Gamma(0)=R$ sets $\delta m^2+\Sigma_1(0)=0$, hence **the one-loop mass relation is**

$$
\boxed{m^2(0,T)=m^2(\Lambda,T)
+\frac g2\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}
\frac1{k^2+m^2(0,T)}.}
$$

Writing the internal line with $R$ is a renormalized or self-consistent one-loop convention. Away from critical infrared singularities it differs from a bare-mass insertion only at higher perturbative order. This equation does not by itself provide exact [critical exponents](../../../../../critical-exponent.md) once loop corrections become large.

For $D>2$, subtract the critical-temperature condition $0=m^2(\Lambda,T_C)+(g/2)I_D(0)$. Take $g$ and the regular coefficients at their critical values, absorbing smooth changes into a coefficient $A>0$. Since

$$
I_D(R)-I_D(0)=-R\,J_D(R),\qquad
J_D(R)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2(k^2+R)},
$$

the [one-loop critical-mass subtraction](../../../../../one-loop-critical-mass-subtraction.md) becomes

$$
\boxed{A(T-T_C)=R\left[1+\frac g2J_D(R)\right].}
$$

Let $K_D$ be the area of the unit $(D-1)$-sphere divided by $(2\pi)^D$. Radial integration gives $J_D(R)=K_D\int_0^\Lambda k^{D-3}(k^2+R)^{-1}dk$.

For $D>4$, $J_D(0)=K_D\Lambda^{D-4}/(D-4)$ is infrared finite, so it merely renormalises the coefficient and $R\propto T-T_C$ is consistent. For $2<D<4$, setting $k=\sqrt R\,x$ yields

$$
J_D(R)\sim K_D R^{(D-4)/2}\int_0^\infty\frac{x^{D-3}}{1+x^2}dx,
$$

with a finite positive dimensionless integral. The correction is singular relative to the term $R$, invalidating the finite-coefficient linear-mass assumption. At $D=4$,

$$
J_4(R)=\frac{K_4}{2}\log\frac{\Lambda^2+R}{R},
$$

so the boundary is logarithmically marginal. For $D\leq2$, even the subtraction using $I_D(0)$ needs an infrared regulator; it cannot be used to restore a finite linear critical expansion. Thus **the ordinary [upper critical dimension](../../../../../upper-critical-dimension.md) is**

$$
\boxed{D_C=4.}
$$

A fixed-coupling self-consistent one-loop formula is not the full marginal [renormalization group](../../../../../renormalization-group.md) analysis, but its logarithm already shows why an uncorrected linear power law is not generic at $D=4$.

At a [tricritical point](../../../../../tricritical-point.md), both the quadratic and quartic scaling directions must be tuned; the leading stabilising interaction is sextic. With canonical scalar-field [engineering dimension](../../../../../engineering-dimension.md) $(D-2)/2$, the sextic coupling has eigenvalue $D-6(D-2)/2=6-2D$. It becomes marginal at $D=3$, giving

$$
\boxed{D_C^{\mathrm{tricritical}}=3.}
$$

Lower even couplings generated by coarse-graining must remain tuned. This is why using an untuned quartic tadpole to diagnose a [tricritical point](../../../../../tricritical-point.md) would give the wrong boundary. The [tricritical sextic beta function](../../../../../tricritical-sextic-beta-function.md) supplies marginal logarithmic corrections at three dimensions.

For a general [multicritical even Landau potential](../../../../../multicritical-even-landau-potential.md), assume the lower stabilising even terms have been tuned away and the first remaining one is $A_{2n}M^{2n}$, with $n\geq2$ and $A_{2n}>0$. Minimising the potential on its ordered branch gives

$$
\boxed{M^{2n-2}=\frac{a_2|t|}{nA_{2n}},\qquad
M^2\propto |t|^{1/(n-1)}.}
$$

Its curvature at the minimum is $4(n-1)a_2|t|$. For a finite positive gradient stiffness $c$, the longitudinal [correlation length](../../../../../correlation-length.md) therefore scales as $\xi\propto |t|^{-1/2}$. The [Ginzburg criterion](../../../../../ginzburg-criterion.md) compares the order-parameter fluctuation averaged over a [correlation volume](../../../../../correlation-volume.md) with this squared mean-field value. Keeping momenta of order $\xi^{-1}$ or less,

$$
\langle(\delta M)^2\rangle_\xi
\sim k_BT\int_{|p|\lesssim\xi^{-1}}\frac{d^Dp}{(2\pi)^D}
\frac1{cp^2+c\xi^{-2}}
\propto\frac{k_BT}{c}\xi^{2-D}.
$$

Consequently the [multicritical Ginzburg ratio](../../../../../multicritical-ginzburg-ratio.md) behaves as

$$
\boxed{\frac{\langle(\delta M)^2\rangle_\xi}{M^2}
\propto |t|^{(D-2)/2-1/(n-1)}.}
$$

Only for a positive exponent do these relative fluctuations vanish on approaching the critical point. Thus **the general [upper critical dimension](../../../../../upper-critical-dimension.md) is**

$$
\boxed{D_C=2+\frac2{n-1}=\frac{2n}{n-1}.}
$$

Equivalently the interaction eigenvalue $y_{2n}=2n-(n-1)D$ vanishes there. The cases $n=2$ and $n=3$ reproduce 4 and 3 respectively.

For $D<D_C$, the ratio diverges and the mean-field assumptions lose self-consistency arbitrarily close to the transition. At $D=D_C$ the [marginal Ginzburg criterion](../../../../../marginal-ginzburg-criterion.md) is scale-independent at this leading estimate, rather than tending to zero; the criterion alone does not prove a divergence or force new power indices. Marginal interactions require a [renormalization group](../../../../../renormalization-group.md) calculation and generally give logarithmic corrections, as for the quartic and sextic cases above. **The boundary case is marginal, not a strict power-law divergence.** This qualifies the printed wording at equality while recovering the requested upper critical dimensions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
