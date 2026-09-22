# Charge lattice inference from oil drops

↑ **Parent:** [Oil drop experiment](oil-drop-experiment.md)

An [integer](integer-split.md) pattern must survive the stated [measurement uncertainty](measurement-uncertainty.md). For an original simulated example, choose a reference [electric charge](electric-charge-split.md) $Q_*>0$, define $y_i=|q_i|/Q_*$, and stipulate state means

$$
\mathbf y=(2.03,\ 2.96,\ 5.02,\ 3.99),\qquad
\sigma_i=0.08.
$$

Here each $\sigma_i$ is an independent [standard uncertainty](standard-uncertainty.md) of a state mean, before shared calibration effects. The generator constructs repeated noisy observations with these means; the numbers are deliberately chosen, not historical data. There is no conversion of $Q_*$ to [coulombs](coulomb.md) and no measured value of the [elementary charge](elementary-charge.md) in this example.

For a candidate spacing $a>0$ in units of $Q_*$ and proposed [integers](integer-split.md) $n_i$, use [weighted least squares](weighted-least-squares.md):

$$
\chi^2(a,\mathbf n)=\sum_i\frac{(y_i-n_i a)^2}{\sigma_i^2},\qquad
\widehat a=\frac{\sum_i n_i y_i/\sigma_i^2}{\sum_i n_i^2/\sigma_i^2},\qquad
u(\widehat a)=\left(\sum_i\frac{n_i^2}{\sigma_i^2}\right)^{-1/2}.
$$

The last two expressions follow by differentiating the quadratic in $a$ and propagating the independent errors. They are conditional on fixed, correct [integer](integer-split.md) assignments and the stated error model. They do not include uncertainty from choosing those assignments. For $\mathbf n=(2,3,5,4)$, they give $\widehat a=1$, $u(\widehat a)\simeq0.01089$, and $\chi^2=0.46875$. Such a small residual is compatible with this chosen error scale; it is not evidence that the errors vanish. A [chi-squared distribution](chi-squared-distribution.md) interpretation additionally needs the appropriate [normal distribution](normal-distribution.md) error model and allowance for the fitted parameter; searching many assignments changes that interpretation.

<a id="oil-drop-charge-lattice-identifiability"></a>
![](oil-drop-charge-lattice-identifiability.png)

**[Figure 4](#oil-drop-charge-lattice-identifiability). Finite noisy electric charges fit a candidate unit and its subdivisions**. Original calculation for the simulated state means above. Horizontal bars show one [standard uncertainty](standard-uncertainty.md). Both spacings $a=1$ and $a=1/2$ have exactly the same fitted locations and residuals when the [integer](integer-split.md) labels double. The lower curve minimizes over [integers](integer-split.md) separately at every candidate spacing; a low residual alone cannot identify the [elementary charge](elementary-charge.md).

The obstruction is [identifiability](identifiability.md): replacing $(a,n_i)$ by $(a/m,mn_i)$ for any positive [integer](integer-split.md) $m$ leaves every predicted reading unchanged. In particular, an $e$-spaced pattern also fits an $e/2$ lattice using even indices. Even the coarsest well-fitting spacing need not be the physical unit: a dataset containing only even charge states can have twice that unit. Worse, if arbitrarily fine spacings and unrestricted [integers](integer-split.md) are allowed, rounding each $y_i/a$ gives

$$
\min_{\mathbf n}\chi^2(a,\mathbf n)
\leq\frac{a^2}{4}\sum_i\frac1{\sigma_i^2}\longrightarrow0
\quad\text{as }a\longrightarrow0.
$$

Consequently a finite fit cannot prove a minimal transferable [electric charge](electric-charge-split.md). Reproducible smallest observed jumps supply additional evidence; interpreting them as single-carrier transfers requires independent physical support. One visibly abrupt transition could contain several unresolved transfers. In the simulation the successive differences are $0.93$, $2.06$, and $-1.03$, each with [standard uncertainty](standard-uncertainty.md) $\sqrt2(0.08)\simeq0.1131$. These support changes near $a,2a,-a$ conditional on that unit; they equally support $2,4,-2$ units of $a/2$. Neighboring differences share a state reading and are therefore correlated, even though the state means were stipulated independent.

A shared scale error can preserve every apparent [integer](integer-split.md) relation. To first order, an independent fractional scale [standard uncertainty](standard-uncertainty.md) $s$ adds $s^2a^2n_i n_j$ to the [covariance matrix](covariance-matrix.md) of the $y_i$. For the simulation, stipulating $s=0.02$ changes the conditional uncertainty of $\widehat a$ to approximately $\sqrt{0.01089^2+0.02^2}=0.02277$, despite the same residual pattern. Repeating timings cannot average away this common scale contribution. In the uncorrected continuum model in [elementary charge](elementary-charge.md), holding the other measured inputs fixed gives $|q|\propto\eta^{3/2}$, so a small fractional error in air [dynamic viscosity](dynamic-viscosity-split.md) causes $3/2$ times that fractional error in inferred [electric charge](electric-charge-split.md). The [gas slip correction to Stokes drag](gas-slip-correction-to-stokes-drag.md) requires its own propagation. Pattern agreement, drop-stability controls and absolute [measurement calibration](measurement-calibration.md) together make the inference persuasive within resolution.

## ↑ Ancestors (7)

1. [Oil drop experiment](oil-drop-experiment.md)
2. [Elementary charge](elementary-charge.md)
3. [Electric charge](electric-charge-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
