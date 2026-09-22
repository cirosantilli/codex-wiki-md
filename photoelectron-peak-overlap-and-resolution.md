# Photoelectron peak overlap and resolution

↑ **Parent:** [Chemical shift in photoelectron spectroscopy](chemical-shift-in-photoelectron-spectroscopy.md)

Choose two hypothetical environments A and B of one [chemical element](chemical-element.md), with line centers $\mu_A=284\,\mathrm{eV}$ and $\mu_B=286\,\mathrm{eV}$. Model each line by a normalized [Gaussian function](gaussian-function.md) with common [standard deviation](standard-deviation.md) $\sigma$, and stipulate integrated count weights $w_A=3/4$, $w_B=1/4$. On the [binding energy](binding-energy.md) axis $E$, the normalized count density is

$$
G(E;\mu,\sigma)=\frac{1}{\sqrt{2\pi}\sigma}
\exp\left[-\frac{(E-\mu)^2}{2\sigma^2}\right],
\qquad
I(E)=\frac34G(E;284,\sigma)+\frac14G(E;286,\sigma).
$$

All energies in this expression use [electronvolts](electronvolt.md). Each component's integrated [area](surface-area.md) equals its count weight, and $\int I(E)\,dE=1$. There is no background, statistical counting fluctuation, or additional emission feature in this stipulated model. These choices deliberately isolate [photoelectron peak overlap and resolution](photoelectron-peak-overlap-and-resolution.md).

<a id="image-photoelectron-chemical-shift-resolution"></a>
![](photoelectron-chemical-shift-resolution.png)

**[Figure 10](#image-photoelectron-chemical-shift-resolution). Two chemical components can blend into one maximum**. Original arbitrary normalized data, not a measured spectrum. The chosen [Gaussian mixture distribution](gaussian-mixture-distribution.md) has centers $284$ and $286\,\mathrm{eV}$ and integrated count weights $0.75$ and $0.25$. Changing the common [standard deviation](standard-deviation.md) from $0.25$ to $1.00\,\mathrm{eV}$ changes the number of maxima from two to one, while leaving the centroid at $284.5\,\mathrm{eV}$. These count weights are not [mole fractions](mole-fraction.md); a chemical abundance inference requires [cross section](cross-section-physics.md) and analyzer-response calibration.

Direct integration, or the [law of total expectation](law-of-total-expectation.md) applied to the component label, gives the centroid

$$
\bar E=w_A\mu_A+w_B\mu_B=284.5\,\mathrm{eV}.
$$

The centroid lies between the chemical environments and is not either component's [binding energy](binding-energy.md). Expanding $(E-\bar E)^2$ within each component, the odd cross term integrates to zero. The resulting [variance](variance-split.md) is

$$
\operatorname{Var}(E)=\sigma^2+w_Aw_B(\mu_B-\mu_A)^2
=\sigma^2+0.75\,\mathrm{eV}^2.
$$

For $\sigma=0.25\,\mathrm{eV}$ the [variance](variance-split.md) is $0.8125\,\mathrm{eV}^2$ and the two maxima are separated. For $\sigma=1.00\,\mathrm{eV}$ it is $1.7500\,\mathrm{eV}^2$ and there is one maximum. Each Gaussian's [full width at half maximum](full-width-at-half-maximum.md) is $2\sqrt{2\ln2}\,\sigma$, approximately $0.589$ and $2.355\,\mathrm{eV}$ respectively. The chemical separation remains $2\,\mathrm{eV}$ in both cases. The number of visible maxima therefore does not equal the number of chemical components.

One interpretation of this change is additional independent Gaussian instrument blur. The [convolution of probability densities](convolution-of-independent-random-variables.md) adds the [variances](variance-split.md), so broadening $\sigma=0.25$ to $1$ requires response [standard deviation](standard-deviation.md) $\sqrt{1-0.25^2}=\sqrt{15}/4\simeq0.968246\,\mathrm{eV}$. A normalized response with zero mean preserves the centroid and integrated counts. Real line shapes and backgrounds can depart from this model, and separating hidden components is an [inverse problem](inverse-problem-split.md); a plausible fit does not alone establish uniqueness.

Finally, count weights describe detection. In a simple response model, let $n_i$ denote the number of emitting sites sampled in environment $i$, $s_i$ its effective [photoionization](photoionization.md) [cross section](cross-section-physics.md), and $T_i$ the probability that its emitted [electron](electron.md) contributes to the selected measured line. Then

$$
A_i=Cn_i s_iT_i,\qquad
w_i=\frac{n_i s_iT_i}{\sum_jn_js_jT_j}.
$$

The common factor $C$ includes exposure. Here $T_i$ includes escape from the sample, analyzer transmission and detection. Count weights equal site fractions only if the relevant response factors are equal or corrected. They are not automatically molecular [mole fractions](mole-fraction.md); different [molecules](molecule-split.md) can supply different numbers of the selected emitting sites. In an original example, equal site numbers with $s_A T_A=3s_B T_B$ give the plotted $3:1$ count ratio despite a $1:1$ site ratio.

## ↑ Ancestors (6)

1. [Chemical shift in photoelectron spectroscopy](chemical-shift-in-photoelectron-spectroscopy.md)
2. [X-ray photoelectron spectroscopy](x-ray-photoelectron-spectroscopy.md)
3. [Photoemission spectroscopy](photoemission-spectroscopy.md)
4. [Physical chemistry](physical-chemistry-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Photoelectron peak overlap and resolution](photoelectron-peak-overlap-and-resolution.md)
- [X-ray photoelectron spectroscopy](x-ray-photoelectron-spectroscopy.md)
