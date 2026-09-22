# Selective biochemical reaction pathways

↑ **Parent:** [Biochemistry](biochemistry-split.md)

An [enzyme](enzyme-split.md) accelerates particular [chemical reactions](chemical-reaction-split.md), with [catalytic selectivity](catalytic-selectivity.md) arising from recognition and from the relative ease of the subsequent chemistry. Strong binding alone does not guarantee fast conversion. Nor does [catalysis](catalysis.md) change the [chemical equilibrium](chemical-equilibrium.md) for an unchanged net [chemical reaction](chemical-reaction-split.md). These distinctions explain how [enzymes](enzyme-split.md) can direct the flow of material without creating an extra source of [free energy](thermodynamic-free-energy.md).[§12.7, opening paragraphs and Enzyme Structure and Function: alternative mechanisms, regeneration and specificity](chemistry-2e-by-paul-flowers-and-others.md)

For an original model of competing routes, let a [substrate](substrate-biochemistry.md) $S$ become either a desired [reaction product](product-chemistry.md) $P$ or another [reaction product](product-chemistry.md) $Q$:

$$
S\xrightarrow{k_P}P,\qquad S\xrightarrow{k_Q}Q.
$$

The labels represent hypothetical [chemical species](chemical-species.md) with the same elemental composition, not molecular structures. Assume fixed volume, irreversible [first-order reactions](first-order-reaction.md), constant effective [rate constants](rate-constant.md), and initially $100\,\mathrm{\mu mol}$ of $S$ with neither [reaction product](product-chemistry.md) present. The model approximates a limited operating regime; real [enzyme kinetics](enzyme-kinetics.md) can include saturation and reverse reactions.

<a id="image-selective-acceleration-changes-the-split-between-competing-biochemical-reaction-products"></a>
![](biochemical-competing-reaction-routes.png)

**[Figure 3](#image-selective-acceleration-changes-the-split-between-competing-biochemical-reaction-products). Selective acceleration changes the split between competing biochemical reaction products**. Original illustrative [chemical reaction network](chemical-reaction-network.md) and limiting product amounts from $100\,\mathrm{\mu mol}$ of hypothetical $S$. Chosen effective [rate constants](rate-constant.md) are $k_P=0.08$ or $0.32\,\mathrm{min^{-1}}$ and $k_Q=0.02\,\mathrm{min^{-1}}$. The boxes label [chemical species](chemical-species.md); they are not molecular structures. The bars are model limits, not experimental data.

The [reaction-rate equations](rate-equation.md) give $dn_S/dt=-(k_P+k_Q)n_S$, $dn_P/dt=k_Pn_S$ and $dn_Q/dt=k_Qn_S$, where $n$ denotes [amount of substance](amount-of-substance.md). Consequently,

$$
n_S=n_0e^{-(k_P+k_Q)t},\qquad
n_P=\frac{k_P}{k_P+k_Q}(n_0-n_S),\qquad
n_Q=\frac{k_Q}{k_P+k_Q}(n_0-n_S).
$$

With $k_P=0.08$ and $k_Q=0.02\,\mathrm{min^{-1}}$, the eventual split is $80\,\mathrm{\mu mol}$ of $P$ and $20\,\mathrm{\mu mol}$ of $Q$. At ten minutes, the calculated amounts are approximately $36.8$, $50.6$ and $12.6\,\mathrm{\mu mol}$ for $S$, $P$ and $Q$. Selectively increasing $k_P$ fourfold changes the eventual desired fraction to $0.32/0.34=16/17\approx94.1\%$. Increasing both [rate constants](rate-constant.md) fourfold instead preserves the $80\%$ split and only shortens the conversion time. Speed and selectivity answer different questions.

The bookkeeping matters independently of that model. In ideal [alcoholic fermentation](ethanol-fermentation.md), complete conversion of $3\,\mathrm{mmol}$ of [glucose](glucose.md) yields $6\,\mathrm{mmol}$ each of [ethanol](ethanol.md) and [carbon dioxide](carbon-dioxide.md). Of the initial $18\,\mathrm{mmol}$ of [carbon](carbon.md) [chemical atoms](atom-physics.md), $12$ remain in [ethanol](ethanol.md) and $6$ enter [carbon dioxide](carbon-dioxide.md). This is a chosen material-balance example using the net [stoichiometry](stoichiometry.md) explained under [Saccharomyces cerevisiae](saccharomyces-cerevisiae.md); it gives neither an observed yield nor the mechanism of the individual steps. Equal amounts of the two [reaction products](product-chemistry.md) also do not mean equal [masses](mass.md).

## ↑ Ancestors (3)

1. [Biochemistry](biochemistry-split.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)
