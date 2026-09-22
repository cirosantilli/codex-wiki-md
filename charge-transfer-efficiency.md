# Charge-transfer efficiency

↑ **Parent:** [Charge-coupled device](charge-coupled-device.md)

The [charge-transfer efficiency](charge-transfer-efficiency.md) is the fraction of a packet delivered into its intended next site or time slot in one transfer, under stated conditions. It is distinct from [quantum efficiency](quantum-efficiency.md), which concerns conversion of incident [photons](photon.md) into collected [charge carriers](charge-carrier.md). Define the complementary inefficiency as $\epsilon=1-\eta_{\rm tr}$.

In an original model with constant $0\leq\eta_{\rm tr}\leq1$, let $N_j$ denote the mean number of original packet [electrons](electron.md) still delivered on time after $j$ transfers. Assuming no reinjection into that packet,

$$
N_{j+1}=\eta_{\rm tr}N_j,\qquad N_{\rm out}=N_{\rm in}\eta_{\rm tr}^{n}.
$$

Repeated substitution proves the result; for different efficiencies the fraction is $\prod_{j=1}^{n}\eta_j$. For $\epsilon\ll1$, a [Taylor expansion](taylor-expansion.md) of $\ln(1-\epsilon)$ gives $\eta_{\rm tr}^n\simeq e^{-n\epsilon}$, while the simpler $1-n\epsilon$ requires $n\epsilon\ll1$.

Choose $N_{\rm in}=10000$ and $n=2000$. For $\eta_{\rm tr}=0.9999$, the expected on-time output is $8187.23$ [electrons](electron.md); for $\eta_{\rm tr}=0.99999$, it is $9801.99$. These are model means, so fractional [electron](electron.md) counts do not describe an individual packet. Even a small per-transfer imperfection can imprint distance-dependent image errors.

If every original [electron](electron.md) independently stays on time with [probability](probability.md) $p=\eta_{\rm tr}^n$, a fixed initial count gives a [binomial distribution](binomial-distribution.md) with [variance](variance-split.md) $N_{\rm in}p(1-p)$. An initial [Poisson distribution](poisson-distribution.md) with mean $\mu$ instead gives an on-time [Poisson distribution](poisson-distribution.md) with mean and [variance](variance-split.md) $\mu p$, by [Poisson thinning](poisson-thinning.md). A deterministic attenuation formula alone does not specify noise. Real trapping can correlate packets and depends on timing, illumination and [temperature](temperature-split.md); the independent constant-efficiency model then fails.

## ↑ Ancestors (7)

1. [Charge-coupled device](charge-coupled-device.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [CCD clocked charge transfer](ccd-clocked-charge-transfer.md)
- [Charge-transfer efficiency](charge-transfer-efficiency.md)
- [Early CCD charge-transfer experiment](early-ccd-charge-transfer-experiment.md)
