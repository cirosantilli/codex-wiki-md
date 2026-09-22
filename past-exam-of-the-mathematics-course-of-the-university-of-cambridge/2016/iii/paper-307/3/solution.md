<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The renormalizable action for [chiral superfields](../../../../../chiral-superfield.md) $\Phi_i$ and [vector superfields](../../../../../vector-superfield.md) $V$ has the [superspace integration](../../../../../superspace-integration.md) form

$$
S=\int d^4x\,d^4\theta\,K(\Phi^\dagger e^{2V},\Phi)
+\left[\int d^4x\,d^2\theta\left(W(\Phi)+\frac14 f_{ab}\mathcal W^{a\alpha}\mathcal W^b_\alpha\right)+\mathrm{h.c.}\right],
$$

where $K$ is a real [Kähler potential](../../../../../kahler-potential.md), $\mathcal W_\alpha$ is the [chiral field-strength superfield](../../../../../chiral-field-strength-superfield.md), and $W$ is a gauge-invariant [holomorphic function](../../../../../holomorphic-function.md). For the renormalizable theory choose canonical positive kinetic terms, a polynomial $W$ of degree at most three, and field-independent gauge kinetic coefficients $f_{ab}$. We prove the [non-renormalization theorem](../../../../../non-renormalization-theorem.md) for the local [Wilsonian effective action](../../../../../wilsonian-effective-action.md), with a nonzero infrared cutoff and a regulator preserving [supersymmetry](../../../../../supersymmetry-split.md). The elementary [chiral superfields](../../../../../chiral-superfield.md) are retained; this is not a claim that eliminating whole massive fields leaves the same polynomial.

Write $W=\sum_A\lambda_A\mathcal O_A(\Phi)$, treating masses and interaction coefficients alike as background chiral [spurions](../../../../../spurion.md). A local [F-term](../../../../../f-term.md) is chiral even when these backgrounds vary, so its coefficient depends holomorphically on $\Phi,\lambda_A$ and the holomorphic gauge couplings. Dependence on $\bar\lambda_A$ would not be chiral. Such dependence can enter [D-terms](../../../../../d-term.md) or terms with supercovariant derivatives instead. With the infrared cutoff kept fixed, the perturbative local coefficients are regular power series around vanishing masses and interactions. This removes the inverse-mass and infrared singular terms that would spoil the following [spurion selection rule for perturbative non-renormalization](../../../../../spurion-selection-rule-for-perturbative-non-renormalization.md).

Assign every elementary $\Phi_i$ [R-charge](../../../../../r-charge.md) zero, every $\lambda_A$ [R-charge](../../../../../r-charge.md) two, and $\theta$ [R-charge](../../../../../r-charge.md) one. The [superpotential](../../../../../superpotential.md) must have [R-charge](../../../../../r-charge.md) two because $d^2\theta$ has [R-charge](../../../../../r-charge.md) minus two. Holomorphy excludes the conjugate [spurions](../../../../../spurion.md), so regularity and this formal [R-symmetry](../../../../../r-symmetry.md) require exactly one factor of a superpotential [spurion](../../../../../spurion.md) in any perturbative candidate. Thus $W_{\mathrm{eff}}$ is linear in the $\lambda_A$, with the ordinary flavor [spurion](../../../../../spurion.md) charges fixing the permitted field monomials. An anomalous formal [R-symmetry](../../../../../r-symmetry.md) is implemented by also transforming the holomorphic gauge coupling; its anomaly must not simply be ignored.

Gauge interactions cannot provide a perturbative coefficient modifying this conclusion. With $\tau=\vartheta/(2\pi)+4\pi i/g^2$, perturbative diagrams are independent of the topological angle $\vartheta$. A holomorphic coefficient invariant under continuous real shifts of $\tau$ is constant, by the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). This is [perturbative gauge-coupling independence of the Wilsonian superpotential](../../../../../perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential.md). Contributions involving $e^{2\pi i\tau}$ are nonperturbative and are outside this argument. For an Abelian factor the same angle-independent holomorphy argument applies. Hence a putative perturbative coefficient linear in $\lambda_A$ is independent of the gauge coupling and can be evaluated as that coupling tends to zero.

In this free-gauge limit, an interacting chiral loop needs additional superpotential vertices: the free chiral propagator connects $\Phi$ to $\Phi^\dagger$, so a single holomorphic vertex alone cannot produce a loop correcting its local [F-term](../../../../../f-term.md). Extra vertices introduce extra [spurions](../../../../../spurion.md) or their conjugates, both excluded by the preceding charge and holomorphy argument. The surviving coefficient is its tree value. Therefore

$$
\boxed{W_{\mathrm{Wilsonian}}^{\mathrm{pert}}(\Phi)=W_{\mathrm{tree}}(\Phi)}.
$$

For an explicit charge check, take $W=m\Phi^2/2+g\Phi^3/3$ in the [Wess–Zumino model](../../../../../wess-zumino-model.md). Give $(\Phi,m,g)$ ordinary charges $(1,-2,-3)$ and [R-charges](../../../../../r-charge.md) $(1,0,-1)$. A holomorphic monomial $m^a g^b\Phi^n$ of the required charges satisfies $n-2a-3b=0$ and $n-b=2$, giving $a=1-b$, $n=b+2$. Perturbative regularity requires $a,b\ge0$, hence only $(a,b,n)=(1,0,2)$ and $(0,1,3)$ survive. The free limit fixes their coefficients to $1/2$ and $1/3$; there is no room for a coupling-dependent loop correction. This illustrates the [holomorphy argument for superpotential non-renormalization](../../../../../holomorphy-argument-for-superpotential-non-renormalization.md) explicitly.

The [Kähler potential](../../../../../kahler-potential.md) can acquire [wave-function renormalization](../../../../../wave-function-renormalization.md). Restoring [canonical field normalization](../../../../../canonical-field-normalization.md) changes physical masses and [Yukawa couplings](../../../../../yukawa-interaction.md), so their running does not contradict the boxed statement about holomorphic coordinates. Gauge kinetic [F-terms](../../../../../f-term.md) have their own renormalization and are not the [superpotential](../../../../../superpotential.md). Infrared effects in the one-particle-irreducible [quantum effective action](../../../../../effective-action.md), tree-level elimination of retained fields, and genuine nonperturbative effects must likewise be distinguished from this perturbative [Wilsonian effective action](../../../../../wilsonian-effective-action.md) theorem.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
