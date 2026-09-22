# Calibrated two-wire charge centroid

↑ **Parent:** [Multiwire proportional chamber](multiwire-proportional-chamber.md)

Can two readout values locate a hit between wires? **Only with a specified response model.** Place two readout wires at $0$ and $p$, put $u=x/p\in[0,1]$, and stipulate calibrated, noiseless [electric charges](electric-charge-split.md)

$$
q_L=Q(1-u),\qquad q_R=Qu,\qquad Q>0.
$$

These are assumptions for a toy sensor response, not the natural response law of adjacent [anode](anode.md) wires. Under these assumptions the [centroid](centroid.md)

$$
\widehat x=\frac{0q_L+pq_R}{q_L+q_R}=pu=x
$$

recovers position exactly. The apparent gain in precision comes from adding calibrated analogue information. Taking the mean of two fired wire addresses without their [electric charges](electric-charge-split.md) would instead give the fixed midpoint $p/2$.

For a chosen noise model, replace the two [electric charges](electric-charge-split.md) by $q_L+n_L$ and $q_R+n_R$, with [independent random variables](independent-random-variables.md) $n_L,n_R$ of zero [expected value](expected-value-split.md) and common [standard deviation](standard-deviation.md) $s$. Assume $s/Q\ll1$ and no threshold censoring. First-order expansion of the ratio gives

$$
\delta x\simeq\frac{p}{Q}\bigl[(1-u)n_R-un_L\bigr],\qquad
\sigma_{\mathrm{lin}}(u)=\frac{ps}{Q}\sqrt{(1-u)^2+u^2}.
$$

For stipulated $p=2\,\mathrm{mm}$ and $s/Q=0.02$, this approximation gives $0.0283\,\mathrm{mm}$ at the midpoint and $0.0400\,\mathrm{mm}$ at either endpoint. The endpoint values describe uncensored signed channel readouts, including small negative values after baseline subtraction. They do not assume that both channels would pass a positive threshold. A ratio with a fluctuating denominator also need not have exactly zero bias; this is a local small-noise approximation.

Three original counterexamples show why calibration and selection matter:

- If the right channel retains a relative gain $g=1.10$, then $\widehat x/p=gu/(1-u+gu)$. At $u=1/2$, the bias is $p/42=0.0476\,\mathrm{mm}$ for the chosen pitch, larger than the midpoint noise estimate above.
- Suppose symmetric electronic leakage transforms the normalized right signal to $v=\epsilon+(1-2\epsilon)u$. Treating $v$ as $u$ gives a position bias $p\epsilon(1-2u)$. A known $\epsilon\ne1/2$ permits inversion; $\epsilon=1/2$ destroys position information entirely. This is a stipulated crosstalk model, not a measurement.
- Requiring both noiseless channels to exceed $0.1Q$ accepts only $0.1<u<0.9$: $80\%$ of uniformly distributed hits. Computing a position spread after that cut describes a selected sample. It does not establish improved [spatial resolution](spatial-resolution.md) for all incident hits.

Likewise, two equal hits at $u=1/4$ and $u=3/4$ have exactly the same total two-channel response as one hit at $u=1/2$ with twice the [electric charge](electric-charge-split.md). A [centroid](centroid.md) can hide multiplicity even when each charge measurement is exact.

[Diffusion](diffusion.md) enabled the lecture's Orsay interpolation, without establishing this model's linear response.[p. 30](electronic-imaging-of-ionizing-radiation-with-limited-avalanches-in-gases-by-georges-charpak.md)

## ↑ Ancestors (5)

1. [Multiwire proportional chamber](multiwire-proportional-chamber.md)
2. [Particle detector](particle-detector.md)
3. [Particle detection](particle-detection-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
