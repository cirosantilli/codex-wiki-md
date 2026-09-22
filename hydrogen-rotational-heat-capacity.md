# Hydrogen rotational heat capacity

↑ **Parent:** [Rotational partition functions of hydrogen](rotational-partition-functions-of-hydrogen.md)

Let $u_s=\langle\epsilon\rangle_s$ and $v_s=\operatorname{Var}_s(\epsilon)$ for the conditional distributions of [parahydrogen](parahydrogen.md) and [orthohydrogen](orthohydrogen.md), with $s=\mathrm p,\mathrm o$. Differentiating the normalized [Boltzmann factors](boltzmann-factor.md) gives $du_s/dt=v_s/t^2$. Thus the rotational [heat capacity at constant volume](heat-capacity-at-constant-volume.md) per [molecule](molecule-split.md) of a composition frozen at $x$ is

$$
\frac{c_{\rm fr}}{k_{\rm B}}=\frac{(1-x)v_{\rm p}+xv_{\rm o}}{t^2}.
$$

At conversion equilibrium, the [law of total variance](law-of-total-variance.md) adds a nonnegative contribution from the changing species populations:

$$
\frac{c_{\rm eq}}{k_{\rm B}}=
\frac{(1-x_{\rm o}^{\rm eq})v_{\rm p}+x_{\rm o}^{\rm eq}v_{\rm o}
+x_{\rm o}^{\rm eq}(1-x_{\rm o}^{\rm eq})(u_{\rm o}-u_{\rm p})^2}{t^2}.
$$

The last term is the contribution from conversion. Compare the first two terms with a frozen sample at the same instantaneous composition; a frozen $3:1$ sample generally has different weights too. This formula follows directly from the [variance](variance-split.md) of a mixture: subtract the overall mean inside each species, expand the square, and the cross terms vanish because each conditional deviation has zero mean. It also proves nonnegative rotational [heat capacity](heat-capacity.md) in either model.

<a id="image-hydrogen-equilibrium-and-frozen-rotational-heat-capacity"></a>
![](hydrogen-equilibrium-and-frozen-rotational-heat-capacity.png)

**[Figure 8](#image-hydrogen-equilibrium-and-frozen-rotational-heat-capacity). Hydrogen rotational heat capacity: equilibrating and frozen spin populations**. Original numerical sums of the stated [linear rigid rotor](linear-rigid-rotor.md) model through $J=100$. The upper panel compares the equilibrium [orthohydrogen](orthohydrogen.md) fraction with frozen [normal hydrogen](normal-hydrogen.md); the lower panel also shows pure [parahydrogen](parahydrogen.md). These are dimensionless predictions, not experimental curves. Only internal [molecular rotation](molecular-rotation.md) contributes: [translation](translation-geometry.md), [molecular vibration](molecular-vibration.md), interactions between [molecules](molecule-split.md), and external-field splittings are omitted.

For an original worked example at $t=1/2$, summing the allowed ladders gives $q_{\rm p}\approx1.00003072$, $q_{\rm o}\approx0.05494692$, and $x_{\rm o}^{\rm eq}\approx0.14150982$. The calculated rotational [heat capacities](heat-capacity.md) are $c_{\rm eq}/k_{\rm B}\approx1.94719633$ and $c_{\rm fr}/k_{\rm B}\approx0.00110733$ for frozen [normal hydrogen](normal-hydrogen.md). The contrast is large because changing species accesses the $J=0$ to $J=1$ separation, whereas fixed species must use the larger $J=0$ to $2$ or $J=1$ to $3$ separations. These are model numbers at a chosen dimensionless [temperature](temperature-split.md), not measured hydrogen data.

Both rotational [heat capacities](heat-capacity.md) approach zero as $t\to0$, although frozen [normal hydrogen](normal-hydrogen.md) retains nonzero rotational [internal energy](internal-energy-split.md). Both approach $k_{\rm B}$ as $t\to\infty$ within the rotor model. The high-[temperature](temperature-split.md) limit is a formal limit with all other excitations suppressed; actual [molecular hydrogen](molecular-hydrogen.md) eventually needs [molecular vibration](molecular-vibration.md), nonrigidity, and dissociation. Multiplying the per-[molecule](molecule-split.md) result by the [Avogadro constant](avogadro-constant.md) gives rotational [molar heat capacity](molar-heat-capacity.md) in units of the [molar gas constant](molar-gas-constant.md) $R$. A dilute classical [ideal gas](ideal-gas-split.md) additionally contributes $3R/2$ from [translation](translation-geometry.md) to its [heat capacity at constant volume](heat-capacity-at-constant-volume.md).

## ↑ Ancestors (8)

1. [Rotational partition functions of hydrogen](rotational-partition-functions-of-hydrogen.md)
2. [Spin isomers of hydrogen](spin-isomers-of-hydrogen.md)
3. [Homonuclear diatomic molecule](homonuclear-diatomic-molecule.md)
4. [Diatomic molecule](diatomic-molecule.md)
5. [Linear molecule](linear-molecule.md)
6. [Molecule](molecule-split.md)
7. [Chemistry](chemistry-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Hydrogen rotational heat capacity](hydrogen-rotational-heat-capacity.md)
