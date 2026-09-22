# Trapped-ion fluorescence count model

↑ **Parent:** [Electron shelving](electron-shelving.md)

For an original illustrative readout model, take detected [photon](photon.md) count $K$ in a fixed exposure to have a [Poisson distribution](poisson-distribution.md), with stipulated means $\lambda_B=12$ for a bright state and $\lambda_D=0.2$ for a dark state. Classify $K\ge3$ as bright. Direct summation gives

$$
P(\text{dark label}\mid B)=e^{-12}\left(1+12+\frac{12^2}{2}\right)\simeq0.0005223,
$$



$$
P(\text{bright label}\mid D)=1-e^{-0.2}\left(1+0.2+\frac{0.2^2}{2}\right)\simeq0.0011485.
$$

With equally likely preparations, the average misclassification [probability](probability.md) is $0.0008354$. These numbers describe only the chosen count model. Actual [fluorescence](fluorescence-split.md) includes short-time photon correlations, detector effects and possible state changes; it need not follow a fixed-rate [Poisson process](poisson-process-split.md). Longer exposure can improve separation of count distributions while increasing unwanted [optical pumping](optical-pumping.md), metastable decay or recoil.

If the prepared bright population is $p$, let $\alpha$ and $\beta$ denote the two conditional errors above. The observed bright-label [probability](probability.md) is $q=(1-\alpha)p+\beta(1-p)$, hence $p=(q-\beta)/(1-\alpha-\beta)$ when the denominator is nonzero. Known-state controls must estimate $\alpha,\beta$ in the actual apparatus; the formula cannot correct unknown drift. For $M$ independent preparations, the raw bright fraction has [variance](variance-split.md) $q(1-q)/M$. Counting uncertainty, preparation error, pulse error and state-detection bias therefore enter different parts of the inference. Repeating a biased measurement reduces its sampling uncertainty without removing its bias.

## ↑ Ancestors (7)

1. [Electron shelving](electron-shelving.md)
2. [Trapped-ion quantum control](trapped-ion-quantum-control.md)
3. [Ion trap](ion-trap.md)
4. [Atomic measurement methods](atomic-measurement-methods.md)
5. [Atomic physics](atomic-physics-split.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
