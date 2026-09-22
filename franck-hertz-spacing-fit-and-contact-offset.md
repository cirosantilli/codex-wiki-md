# Franck-Hertz spacing fit and contact offset

↑ **Parent:** [Franck-Hertz energy-loss model](franck-hertz-energy-loss-model.md)

Fit the positions of successive, consistently defined troughs by [linear regression](linear-regression-split.md), $V_n=b+nd+\epsilon_n$. A constant intercept $b$ absorbs the [contact potential difference](contact-potential-difference.md), collection phase and initial [energy](energy-split.md) effects; $d$ estimates the repeated loss expressed as a voltage. Subtracting successive positions cancels $b$. A line fit uses every position and leaves residuals that can reveal curvature or a misidentified trough. It still assumes that the phase is constant over the fitted range and that all troughs belong to the same loss channel.

For an original numerical example, choose $n=1,2,3,4,5$ and synthetic positions $V_n=(6.62,11.46,16.48,21.30,26.14)\,\mathrm V$. Their successive spacings are $(4.84,5.02,4.82,4.84)\,\mathrm V$. The [ordinary least squares](ordinary-least-squares.md) formulas give

$$
\widehat d=\frac{\sum_n(n-\bar n)(V_n-\bar V)}{\sum_n(n-\bar n)^2}=4.888\,\mathrm V,\qquad
\widehat b=\bar V-\widehat d\,\bar n=1.736\,\mathrm V.
$$

The fitted residuals are $(-0.004,-0.052,0.080,0.012,-0.036)\,\mathrm V$, with zero sum and zero index-weighted sum. Their [residual sum of squares](residual-sum-of-squares.md) is $0.01056\,\mathrm V^2$. If independent, equal-[variance](variance-split.md), zero-mean errors describe these positions, the residual variance estimate is $s^2=0.01056/(5-2)=0.00352\,\mathrm V^2$ and the slope [standard error](standard-error.md) is $s/\sqrt{10}=0.01876\,\mathrm V$. Thus the inferred model loss is $4.888\,\mathrm{eV}$ with conditional [standard error](standard-error.md) $0.01876\,\mathrm{eV}$. These errors summarize only the chosen position scatter; a voltage-scale error or a drifting collection phase is not included. Adjacent spacings share a position error and are therefore correlated even when position errors are independent.

The offset has a sharper [identifiability](identifiability.md) limitation. Even if a constant-phase model were exact, an initial beam [kinetic energy](kinetic-energy.md) $E_0$ shifts the troughs by $-E_0/e$. For the symmetric illustrative curve, $b=V_c-E_0/e+V_r/2$. The transformation $V_c\mapsto V_c+\alpha$, $E_0\mapsto E_0+e\alpha$ leaves every trough position unchanged. Measuring $b$ alone therefore cannot determine the [contact potential difference](contact-potential-difference.md). Relabeling $n\mapsto n+m$ also changes $b$ by $-md$ without changing $d$. An independent offset calibration and a justified collection model are needed before turning a first trough into an excitation threshold. Varying $V_r$ tests this model's predicted half-voltage shift of the trough centers; it is a diagnostic prediction of this chosen curve, not a universal correction for experimental minima.

## ↑ Ancestors (8)

1. [Franck-Hertz energy-loss model](franck-hertz-energy-loss-model.md)
2. [Franck-Hertz experiment](franck-hertz-experiment.md)
3. [Excited state](excited-state.md)
4. [Energy eigenvalue](energy-eigenvalue-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
