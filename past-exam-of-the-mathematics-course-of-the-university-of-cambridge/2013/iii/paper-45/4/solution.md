<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An **[effective field theory](../../../../../effective-field-theory.md) is a controlled description of specified low-energy degrees of freedom at a chosen accuracy**. It does not require knowing all physics at arbitrarily short distances. If new particles or strong dynamics enter at a scale $M$, processes with characteristic energy and momentum transfers $E\ll M$ can be described using the light fields and interactions consistent with their symmetries. In [natural units](../../../../../natural-units.md), four-dimensional [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md) organizes a local [Lagrangian](../../../../../lagrangian.md) as

$$
\mathcal L_{\mathrm{EFT}}=\mathcal L_{d\leq4}+\sum_{d>4}\sum_i\frac{C_i^{(d)}(\mu)}{M^{d-4}}\mathcal O_i^{(d)}.
$$

Here $\mathcal O_i^{(d)}$ has [mass dimension](../../../../../mass-dimension.md) $d$, the dimensionless $C_i^{(d)}$ are [Wilson coefficients](../../../../../wilson-coefficient.md), and $\mu$ is a [renormalization scale](../../../../../renormalization-scale.md). In a relativistic vacuum with canonical fields, a typical insertion of a dimension-$d$ interaction contributes an additional power $(E/M)^{d-4}$, multiplied by its couplings and any light mass ratios. Additional expansions, such as a loop expansion, must also be specified. Symmetry or on-shell identities can postpone a particular observable's first correction.

The theory is useful when its retained states and expansion parameters adequately describe the experiment. It ceases to be a reliable truncated local description near an omitted particle's production threshold, near a heavy propagator pole, or where the retained dynamics become too strongly coupled for an assumed perturbative expansion. A light particle cannot be removed merely because one wants fewer variables: its propagation can produce nonanalytic momentum dependence that must be represented by retained light fields. [Heavy-field decoupling](../../../../../heavy-field-decoupling.md) can shift renormalizable masses and couplings as well as generate suppressed interactions; those low-energy parameters must be measured or matched, not assumed unchanged. The [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) is an organizational scale, while a calculation may use a regulator other than a hard momentum cutoff.

Construction starts by identifying the light particles, the hierarchy of scales, and the exact or approximate symmetries relevant to the problem. Form all allowed [local field operators](../../../../../local-operator-physics.md) through the desired order in [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md). Choose an [operator basis in effective field theory](../../../../../operator-basis-in-effective-field-theory.md): remove equivalent terms by [integration by parts](../../../../../integration-by-parts.md), algebraic identities and allowed [field redefinitions](../../../../../field-redefinition.md). Operators proportional to lower-order [equations of motion](../../../../../equation-of-motion.md) can be [redundant operators](../../../../../redundant-operator.md) for on-shell amplitudes, provided coefficients are consistently transformed. This reduces bookkeeping without imposing additional physics assumptions.

If an [ultraviolet completion](../../../../../ultraviolet-completion.md) is known, determine the [Wilson coefficients](../../../../../wilson-coefficient.md) by [matching in effective field theory](../../../../../matching-in-effective-field-theory.md): calculate low-energy amplitudes or appropriate correlation functions in both descriptions using the same infrared conventions, and adjust coefficients so they agree to the chosen order. Equivalently, [integrating out a field](../../../../../integrating-out-a-field.md) performs its [path integral](../../../../../path-integral.md) while retaining the light fields as backgrounds. Heavy propagators have an analytic expansion below their singularities, producing a [derivative expansion](../../../../../derivative-expansion.md); heavy loops also generate local terms and logarithms in their coefficients. Without a specified [ultraviolet completion](../../../../../ultraviolet-completion.md), the coefficients are parameters to be constrained by data.

An [effective field theory](../../../../../effective-field-theory.md) remains predictive even when it contains [nonrenormalizable interactions](../../../../../nonrenormalizable-interaction.md). At each fixed order in energy and loops there are finitely many required coefficients and [counterterms](../../../../../counterterm.md). [Renormalization](../../../../../renormalization.md) absorbs divergences into that order's allowed operators. The [renormalization group](../../../../../renormalization-group.md) evolves the [Wilson coefficients](../../../../../wilson-coefficient.md) between matching and measurement scales, compensating scale dependence in matrix elements and, when appropriate, resumming large logarithms. The [truncation error in effective field theory](../../../../../truncation-error-in-effective-field-theory.md) is estimated from the first omitted orders, under a stated coupling-size assumption; it is separate from parameter uncertainty and cannot be inferred merely by writing down infinitely many terms.

A concrete example is [heavy scalar exchange in effective field theory](../../../../../heavy-scalar-exchange-in-effective-field-theory.md). Take a light real [scalar field](../../../../../scalar-field.md) $\varphi$ and a heavy real [scalar field](../../../../../scalar-field.md) $S$, with

$$
\mathcal L_{\mathrm{UV}}=\frac12(\partial\varphi)^2-\frac{m^2}{2}\varphi^2-\frac\lambda{4!}\varphi^4
+\frac12(\partial S)^2-\frac{M^2}{2}S^2-\frac a2 S\varphi^2,\qquad M\gg m,E.
$$

The coupling $a$ has mass dimension one. The light-field symmetry is $\varphi\mapsto-\varphi$. For $m^2\geq0$ and $\lambda>3a^2/M^2$, the displayed [scalar potential](../../../../../scalar-potential.md) is bounded below: completing the square in $S$ leaves a positive light quartic. Thus the example can be treated as a stable theory around $S=\varphi=0$, with weak enough couplings for the tree approximation.

At tree level the heavy [equation of motion](../../../../../equation-of-motion.md) is $(M^2+\Box)S=-a\varphi^2/2$. Substitute its solution back into the action, including both its quadratic and source terms, to obtain

$$
\Delta\mathcal L_{\mathrm{eff}}=\frac{a^2}{8}\varphi^2\frac1{M^2+\Box}\varphi^2
=\frac{a^2}{8M^2}\varphi^4-\frac{a^2}{8M^4}\varphi^2\Box\varphi^2+\frac{a^2}{8M^6}\varphi^2\Box^2\varphi^2+\cdots.
$$

This is a [derivative expansion](../../../../../derivative-expansion.md) valid for small momentum transfers, not an exact local replacement near the pole. The first term gives **$\lambda_{\mathrm{eff}}=\lambda-3a^2/M^2$** in the $-\lambda_{\mathrm{eff}}\varphi^4/4!$ convention. After [integration by parts](../../../../../integration-by-parts.md), the next term is $+a^2(\partial_\mu\varphi^2)(\partial^\mu\varphi^2)/(8M^4)$; it is a dimension-six local operator. Writing $a=g_*M$ puts its coefficient in the usual $g_*^2/M^2$ form. These coefficients are a tree-level [matching in effective field theory](../../../../../matching-in-effective-field-theory.md) result.

One can directly check the matching through the on-shell [scattering amplitude](../../../../../scattering-amplitude.md) for $\varphi\varphi\to\varphi\varphi$. With $s,t,u$ the [Mandelstam variables](../../../../../mandelstam-variables.md), the full theory has three heavy-exchange channels:

$$
\mathcal M_{\mathrm{UV}}=-\lambda+a^2\left(\frac1{M^2-s}+\frac1{M^2-t}+\frac1{M^2-u}\right).
$$

For $|s|,|t|,|u|\ll M^2$,

$$
\mathcal M_{\mathrm{UV}}=-\lambda+\frac{3a^2}{M^2}+\frac{a^2(s+t+u)}{M^4}
+\frac{a^2(s^2+t^2+u^2)}{M^6}+\cdots.
$$

The [effective field theory](../../../../../effective-field-theory.md) reproduces these terms in order: a shifted quartic, then local derivative interactions. Since $s+t+u=4m^2$ on shell, the first derivative correction is a light-mass-dependent constant; it vanishes for $m=0$. This illustrates why an [operator basis in effective field theory](../../../../../operator-basis-in-effective-field-theory.md) can trade some derivative operators for mass-dependent or higher-field interactions using [field redefinitions](../../../../../field-redefinition.md). For massless external particles, the first nonconstant correction in this four-point tree amplitude starts at the following order.

**The example exhibits the central logic: keep the light field, encode virtual heavy exchange in matched local coefficients, and control the error by expanding in momentum divided by the heavy scale.** No heavy particle is actually produced in the domain of the approximation. Near $s=M^2$, the full propagator is resonant and the truncated [effective field theory](../../../../../effective-field-theory.md) fails; retaining $S$ or adopting a different description is then necessary. Light loops are computed within the [effective field theory](../../../../../effective-field-theory.md), while higher-order matching supplies the corresponding heavy corrections.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
