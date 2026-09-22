# Lamb shift line-centre model

↑ **Parent:** [Lamb-Retherford experiment](lamb-retherford-experiment.md)

Consider an original illustrative resonance model, with all numerical settings chosen here. On one isolated branch approximate the transition [frequency](frequency.md) by $\nu(B)=\nu_0+aB$, with known slope $a=20\ \mathrm{MHz/mT}$ and drive [frequency](frequency.md) $\nu_d=1300\ \mathrm{MHz}$. Choose $\nu_0=1100\ \mathrm{MHz}$, hence resonance field $B_r=10\ \mathrm{mT}$. This local linear model omits [hyperfine structure](hyperfine-structure.md) and nonlinear level mixing; it is not the historical hydrogen [Zeeman splitting](zeeman-splitting.md) calculation.

Use a [Lorentzian line shape](lorentzian-line-shape.md) for a weak-drive current dip,

$$
I(B)=C-\frac{A}{1+4(B-B_r)^2/w_B^2},\qquad
w_B=\frac{w_\nu}{|a|}.
$$

Choose baseline $C=1$, depth $A=0.25$ in arbitrary detector signal units, and [full width at half maximum](full-width-at-half-maximum.md) $w_\nu=100\ \mathrm{MHz}$, so $w_B=5\ \mathrm{mT}$. The half-depth points are $B_r\pm w_B/2$; this checks the factor of four. If an exponential decay with lifetime $\tau$ alone set this width, [natural linewidth](natural-linewidth.md) would give $w_\nu=1/(2\pi\tau)$ and $\tau\simeq1.59\ \mathrm{ns}$. The chosen width is an explanatory input, not a measurement of a historical lifetime.

Generate 65 equally spaced fields from $2$ to $18\ \mathrm{mT}$ and add independent [Gaussian noise](gaussian-noise.md) with known [standard deviation](standard-deviation.md) $\sigma_I=0.004$ signal units. A simultaneous [nonlinear regression](nonlinear-regression.md) fit of $C,A,B_r,w_B$ gives $B_r\simeq10.0007\ \mathrm{mT}$, $w_B\simeq4.9305\ \mathrm{mT}$ and $\nu_0\simeq1099.986\ \mathrm{MHz}$. With residual derivatives $J_{ik}=\partial I(B_i)/\partial\theta_k$ and $\theta=(C,A,B_r,w_B)$, the local [covariance matrix](covariance-matrix.md) estimate is

$$
\operatorname{Cov}(\hat\theta)\simeq\sigma_I^2(J^{\mathsf T}J)^{-1}.
$$

It gives centre [standard deviation](standard-deviation.md) $0.01427\ \mathrm{mT}$, or $0.285\ \mathrm{MHz}$ in the inferred intercept. This uses the stipulated noise variance and a local linear approximation, rather than treating the width as the centre error. Repeated noisy samples can locate a broad line's centre much more closely than its width.

<a id="image-chosen-resonance-line-fit-and-zero-field-intercept"></a>
![](lamb-shift-chosen-resonance-line-fit.png)

**[Figure 2](#image-chosen-resonance-line-fit-and-zero-field-intercept). Chosen resonance line fit and zero-field intercept**. Original synthetic data and fitted Lorentzian current dip, with a separate linear field-to-frequency construction. All frequencies, fields, widths, signal units and noise are chosen for this example. The zero-field intercept is not a measured Lamb splitting. The displayed uncertainties are standard deviations under the stated model.

Include a common magnetic calibration offset with [standard deviation](standard-deviation.md) $u_b=0.020\ \mathrm{mT}$, a fractional gain error $u_g=0.001$, and independent drive-frequency error $u_d=0.100\ \mathrm{MHz}$. To first order the inferred [variance](variance-split.md) is

$$
u^2(\nu_0)\simeq a^2u^2(B_r)+a^2u_b^2+(aB_r)^2u_g^2+u_d^2.
$$

Here $u$ denotes a [standard uncertainty](standard-uncertainty.md), not a [frequency](frequency.md). The four contributions in $\mathrm{MHz}$ are $0.285$, $0.400$, $0.200$, and $0.100$; adding their squares gives $u(\nu_0)\simeq0.540\ \mathrm{MHz}$. The calibration offset shifts all sampled fields together, so increasing the sample count cannot average it away. Uncertainty in $a$, unresolved components, asymmetric line distortion, and errors in the assumed field dependence would require additional terms or a richer model. The historical inference requires the appropriate [Zeeman splitting](zeeman-splitting.md) branches, rather than simply drawing a straight line through one resonance.

## ↑ Ancestors (5)

1. [Lamb-Retherford experiment](lamb-retherford-experiment.md)
2. [Lamb shift](lamb-shift.md)
3. [Atomic physics](atomic-physics-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
