# Second-order reaction

↑ **Parent:** [Order of reaction](order-of-reaction.md)

A [second-order reaction](second-order-reaction.md) has overall [order of reaction](order-of-reaction.md) two: a [rate law](rate-law.md) may depend on $[\mathrm A]^2$, or on $[\mathrm A][\mathrm B]$ with partial [orders of reaction](order-of-reaction.md) one and one. Doubling all relevant [reactant](reactant.md) [concentrations](concentration.md) multiplies the [reaction rate](reaction-rate.md) by four at fixed conditions. This experimentally determined dependence does not establish [molecularity](molecularity.md) or a unique [reaction mechanism](reaction-mechanism.md). For an [elementary reaction](elementary-reaction.md) obeying the [law of mass action](law-of-mass-action.md), [molecularity](molecularity.md) and overall [order of reaction](order-of-reaction.md) agree; a net [chemical equation](chemical-equation.md) alone cannot establish that the conversion is elementary.[Glossary of Terms Used in Physical Organic Chemistry, IUPAC Recommendations 1994, entry “order of reaction”, final paragraphs: elementary versus stepwise reactions](glossary-of-terms-used-in-physical-organic-chemistry-iupac-recommendations-1994-n-and-o-entries-by-international-union-of-pure-and-applied-chemistry.md)

For the single-[concentration](concentration.md) model, explicitly choose the [disappearance rate](disappearance-rate.md) convention

$$
-\frac{d[\mathrm A]}{dt}=k_{\mathrm{obs}}[\mathrm A]^2,\qquad [\mathrm A](0)=[\mathrm A]_0>0,\qquad k_{\mathrm{obs}}>0.
$$

Here $k_{\mathrm{obs}}$ is the coefficient for loss of A, held fixed at the specified [temperature](temperature-split.md) and other conditions. Its subscript labels the chosen observed [disappearance rate](disappearance-rate.md); it does not imply a [pseudo-first-order reaction](pseudo-first-order-reaction.md). Assume a uniformly mixed [closed system](closed-system.md), fixed [volume](volume.md), and no appreciable reverse or competing [chemical reactions](chemical-reaction-split.md). The [integrated rate law](integrated-rate-law.md) is

$$
\boxed{\frac1{[\mathrm A](t)}=\frac1{[\mathrm A]_0}+k_{\mathrm{obs}}t},\qquad
[\mathrm A](t)=\frac{[\mathrm A]_0}{1+k_{\mathrm{obs}}[\mathrm A]_0t}.
$$

The reciprocal-[concentration](concentration.md) plot is a straight line with slope $k_{\mathrm{obs}}$ and intercept $1/[\mathrm A]_0$. A brief derivation uses the [chain rule](chain-rule.md): $d(1/[\mathrm A])/dt=-[\mathrm A]^{-2}d[\mathrm A]/dt=k_{\mathrm{obs}}$, then applies the [initial condition](initial-condition.md). This is a hyperbolic decay, rather than the [exponential decay](exponential-decay.md) of a [first-order reaction](first-order-reaction.md).[§12.4, “Second-Order Reactions”, integrated equation and straight-line form; Table 12.2](chemistry-2e-by-paul-flowers-and-others.md)

As an original prescribed example, choose $[\mathrm A]_0=0.020\,\mathrm{mol\,L^{-1}}$ and $k_{\mathrm{obs}}=0.50\,\mathrm{L\,mol^{-1}\,s^{-1}}$. At $t=100\,\mathrm s$, the reciprocal-[concentration](concentration.md) calculation is $50+50=100\,\mathrm{L\,mol^{-1}}$, giving $[\mathrm A]=0.010\,\mathrm{mol\,L^{-1}}$. The initial [disappearance rate](disappearance-rate.md) is $0.50(0.020)^2=2.0\times10^{-4}\,\mathrm{mol\,L^{-1}\,s^{-1}}$; after $100\,\mathrm s$ it is $5.0\times10^{-5}\,\mathrm{mol\,L^{-1}\,s^{-1}}$. Halving the [concentration](concentration.md) quarters the [disappearance rate](disappearance-rate.md).

[Dimensional analysis](dimensional-analysis.md) checks every formula: $k_{\mathrm{obs}}[\mathrm A]^2$ has units $\mathrm{mol\,L^{-1}\,s^{-1}}$, $k_{\mathrm{obs}}t$ has units $\mathrm{L\,mol^{-1}}$, and $k_{\mathrm{obs}}[\mathrm A]_0t$ is a [dimensionless quantity](dimensionless-quantity.md). Changing [concentration](concentration.md) units changes the numerical [rate constant](rate-constant.md): the same example is $[\mathrm A]_0=20\,\mathrm{mol\,m^{-3}}$, $k_{\mathrm{obs}}=5.0\times10^{-4}\,\mathrm{m^3\,mol^{-1}\,s^{-1}}$, giving $[\mathrm A](100\,\mathrm s)=10\,\mathrm{mol\,m^{-3}}$.

<a id="image-second-order-concentration-and-reciprocal-time"></a>
![](second-order-concentration-and-reciprocal-time.png)

**[Figure 15](#image-second-order-concentration-and-reciprocal-time). Second-order reaction concentration decay and reciprocal-concentration lines for three prescribed starting concentrations**. Original model curves, not measured data. All use the [disappearance rate](disappearance-rate.md) coefficient $k_{\mathrm{obs}}=0.50\,\mathrm{L\,mol^{-1}\,s^{-1}}$. The reciprocal lines share a slope while their intercepts differ; marked points give each run's first [half-life](half-life.md).

For an [elementary reaction](elementary-reaction.md) $2\mathrm A\longrightarrow\mathrm P$, instead define the stoichiometrically normalized [reaction rate](reaction-rate.md) $r=k[\mathrm A]^2$. Two A entities disappear per P formed, so

$$
r=-\frac12\frac{d[\mathrm A]}{dt}=\frac{d[\mathrm P]}{dt}=k[\mathrm A]^2,\qquad
-\frac{d[\mathrm A]}{dt}=2k[\mathrm A]^2,\qquad k_{\mathrm{obs}}=2k.
$$

Consequently the reciprocal-[concentration](concentration.md) slope is $2k$, not $k$. In the prescribed example, the normalized [rate constant](rate-constant.md) would be $k=0.25\,\mathrm{L\,mol^{-1}\,s^{-1}}$; initially $r=1.0\times10^{-4}\,\mathrm{mol\,L^{-1}\,s^{-1}}$ while the [disappearance rate](disappearance-rate.md) is twice that. With $[\mathrm P](0)=0$, [stoichiometry](stoichiometry.md) gives $[\mathrm P](100\,\mathrm s)=([\mathrm A]_0-[\mathrm A])/2=0.0050\,\mathrm{mol\,L^{-1}}$. Both [rate constants](rate-constant.md) have the same dimensions, so a units check alone cannot catch their factor-of-two difference. The symbol $r$ denotes the same normalization as $v$ in [reaction rate](reaction-rate.md).

The [half-life](half-life.md), meaning the time to reach half a specified starting [concentration](concentration.md), follows by setting $[\mathrm A]=[\mathrm A]_0/2$:

$$
\boxed{t_{1/2}=\frac1{k_{\mathrm{obs}}[\mathrm A]_0}}.
$$

For $r=k[\mathrm A]^2$ in $2\mathrm A\longrightarrow\mathrm P$, this becomes $t_{1/2}=1/(2k[\mathrm A]_0)$. Its units are seconds because $k_{\mathrm{obs}}[\mathrm A]_0$ has units $\mathrm{s^{-1}}$. Doubling the starting [concentration](concentration.md) halves the first [half-life](half-life.md); a quoted [half-life](half-life.md) needs its starting [concentration](concentration.md). This differs from a [first-order reaction](first-order-reaction.md), whose [half-life](half-life.md) is independent of starting [concentration](concentration.md).[§12.4, “Half-Life of a Reaction”, second-order derivation and Table 12.2](chemistry-2e-by-paul-flowers-and-others.md)

Within the prescribed run, $[\mathrm A]$ reaches $0.010$, $0.0050$, and $0.0025\,\mathrm{mol\,L^{-1}}$ at $100$, $300$, and $700\,\mathrm s$. The successive halving intervals are $100$, $200$, and $400\,\mathrm s$: each begins at a smaller [concentration](concentration.md). More generally, reaching fraction $f$ of the initial [concentration](concentration.md), with $0<f<1$, requires $t=(f^{-1}-1)/(k_{\mathrm{obs}}[\mathrm A]_0)$, so $90\%$ consumption takes nine initial [half-lives](half-life.md), rather than a fixed sequence of equal waiting times.

<a id="image-second-order-halving-intervals-and-initial-concentration"></a>
![](second-order-halving-intervals-and-initial-concentration.png)

**[Figure 16](#image-second-order-halving-intervals-and-initial-concentration). Lengthening second-order reaction halving intervals and the dependence of the first half-life on initial concentration**. Original model predictions, not measurements. Left: the prescribed $0.020\,\mathrm{mol\,L^{-1}}$ run. Right: $t_{1/2}=1/(k_{\mathrm{obs}}[\mathrm A]_0)$ at fixed $k_{\mathrm{obs}}=0.50\,\mathrm{L\,mol^{-1}\,s^{-1}}$, compared with a [first-order reaction](first-order-reaction.md) chosen to have $t_{1/2}=100\,\mathrm s$. That comparison uses $k_1=\ln2/(100\,\mathrm s)$, with different units from $k_{\mathrm{obs}}$.

A straight reciprocal-[concentration](concentration.md) plot tests this particular single-[concentration](concentration.md) [rate equation](rate-equation.md). It does not uniquely identify a [reaction mechanism](reaction-mechanism.md), nor does curvature rule out every [second-order reaction](second-order-reaction.md): two independently changing [reactant](reactant.md) [concentrations](concentration.md) require their own [integrated rate law](integrated-rate-law.md). At low [concentration](concentration.md), a small [measurement error](measurement-error.md) $\delta[\mathrm A]$ becomes approximately $-\delta[\mathrm A]/[\mathrm A]^2$ in the reciprocal, magnifying late-time errors. Use the line as a diagnostic; a [nonlinear regression](nonlinear-regression.md) of the original [concentrations](concentration.md) can retain their measurement scale and explicit error model.

**Table of contents**

- [Unequal-concentration second-order integration](unequal-concentration-second-order-integration.md)
- [Conductometric saponification assay](conductometric-saponification-assay.md)

## ↑ Ancestors (7)

1. [Order of reaction](order-of-reaction.md)
2. [Rate law](rate-law.md)
3. [Reaction rate](reaction-rate.md)
4. [Chemical kinetics](chemical-kinetics-split.md)
5. [Chemical reaction](chemical-reaction-split.md)
6. [Chemistry](chemistry-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Arrhenius equation](arrhenius-equation.md)
- [Elementary reaction](elementary-reaction.md)
- [Integrated rate law](integrated-rate-law.md)
- [Order of reaction](order-of-reaction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-a/8/solution.md)
- [Pseudo-first-order reaction](pseudo-first-order-reaction.md)
- [Rate constant](rate-constant.md)
- [Saponification](saponification.md)
- [Second-order reaction](second-order-reaction.md)
