# Parallel first-order reaction mechanism

↑ **Parent:** [Reaction mechanism](reaction-mechanism.md)

A [parallel first-order reaction mechanism](parallel-first-order-reaction-mechanism.md) consumes the same [reactant](reactant.md) through competing routes. Extend the product-split idea in [catalytic selectivity](catalytic-selectivity.md) by following both [reaction products](product-chemistry.md) over time. Stipulate irreversible [first-order reactions](first-order-reaction.md) $\mathrm A\xrightarrow{k_P}\mathrm P$ and $\mathrm A\xrightarrow{k_Q}\mathrm Q$ in a uniformly mixed [closed system](closed-system.md) of fixed [volume](volume.md) and [temperature](temperature-split.md). Initially only A is present, with [concentration](concentration.md) $A_0$. With $K=k_P+k_Q$,

$$
[\mathrm A]=A_0e^{-Kt},\qquad
[\mathrm P]=A_0\frac{k_P}{K}(1-e^{-Kt}),\qquad
[\mathrm Q]=A_0\frac{k_Q}{K}(1-e^{-Kt}).
$$

Here $K$ abbreviates a sum of [rate constants](rate-constant.md), not an [equilibrium constant](equilibrium-constant.md). The [rate equations](rate-equation.md) are $-d[\mathrm A]/dt=K[\mathrm A]$, $d[\mathrm P]/dt=k_P[\mathrm A]$, and $d[\mathrm Q]/dt=k_Q[\mathrm A]$. Integrating the last two after solving the first proves the expressions and their conserved total $[\mathrm A]+[\mathrm P]+[\mathrm Q]=A_0$.

Choose two alternative models: model U has $(k_P,k_Q)=(0.30,0.10)\,\mathrm{s^{-1}}$; model V has $(0.10,0.30)\,\mathrm{s^{-1}}$. Both have $K=0.40\,\mathrm{s^{-1}}$, so every measurement of A alone is identical, even with no [measurement error](measurement-error.md). Yet their P-to-Q [concentration](concentration.md) ratios at any $t>0$ are $3$ and $1/3$, respectively. This is a precise failure of [identifiability](identifiability.md) from that one observable. A calibrated measurement distinguishing P from Q resolves it within the stipulated two-route model.

<a id="image-parallel-reaction-hidden-product-split"></a>
![](parallel-reaction-hidden-product-split.png)

**[Figure 5](#image-parallel-reaction-hidden-product-split). Identical reactant disappearance can hide opposite product splits in a parallel first-order reaction mechanism**. Original chosen models U and V share $k_P+k_Q=0.40\,\mathrm{s^{-1}}$ and $A_0=1.00\,\mathrm{mmol\,L^{-1}}$, but exchange the two route [rate constants](rate-constant.md). Left: indistinguishable A traces. Right: different predicted P and Q [concentrations](concentration.md) at $t=5.00\,\mathrm s$; each pair sums to the same total converted A. No curves or bars are experimental measurements.

At $t=5.00\,\mathrm s$, both models give $[\mathrm A]=e^{-2}A_0\approx0.135335\,\mathrm{mmol\,L^{-1}}$. Model U gives $([\mathrm P],[\mathrm Q])\approx(0.648499,0.216166)\,\mathrm{mmol\,L^{-1}}$; model V exchanges these. Measuring only the summed [reaction product](product-chemistry.md) [concentration](concentration.md) would also fail to distinguish them. Product-specific observations therefore answer a question that total conversion cannot. As with any [reaction mechanism](reaction-mechanism.md), fitting these observables still does not rule out a more elaborate untested route.

## ↑ Ancestors (5)

1. [Reaction mechanism](reaction-mechanism.md)
2. [Chemical kinetics](chemical-kinetics-split.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Parallel first-order reaction mechanism](parallel-first-order-reaction-mechanism.md)
- [Reaction mechanism](reaction-mechanism.md)
