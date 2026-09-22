# First-order reaction

↑ **Parent:** [Order of reaction](order-of-reaction.md)

A [first-order reaction](first-order-reaction.md) has a [reaction rate](reaction-rate.md) proportional to one [reactant](reactant.md) [concentration](concentration.md) in the simple single-species case. For an irreversible $\mathrm A\longrightarrow\mathrm B$ in a [closed system](closed-system.md) at fixed [volume](volume.md), take $[\mathrm A](0)=A_0$, $[\mathrm B](0)=0$, and constant [rate constant](rate-constant.md) $k>0$. Its [rate equation](rate-equation.md) and solution are

$$
\frac{d[\mathrm A]}{dt}=-k[\mathrm A],\qquad
[\mathrm A](t)=A_0e^{-kt},\qquad
[\mathrm B](t)=A_0(1-e^{-kt}),\qquad
v(t)=kA_0e^{-kt}.
$$

A short check is enough: differentiating $A_0e^{-kt}$ gives $-kA_0e^{-kt}$, and the two [concentrations](concentration.md) sum to $A_0$, as required by the one-to-one [stoichiometry](stoichiometry.md). Thus the same [exponential decay](exponential-decay.md) describes both remaining [reactant](reactant.md) and decreasing [reaction rate](reaction-rate.md). Fixed $k$ means a fixed fractional loss per unit time, not a fixed absolute consumption rate.

Choose illustrative values $A_0=1\,\mathrm{mol\,L^{-1}}$ and $k=0.2\,\mathrm{s^{-1}}$, with $t$ measured in seconds. Then $[\mathrm A]=e^{-0.2t}\,\mathrm{mol\,L^{-1}}$, $[\mathrm B]=(1-e^{-0.2t})\,\mathrm{mol\,L^{-1}}$, and $v=0.2e^{-0.2t}\,\mathrm{mol\,L^{-1}\,s^{-1}}$. The [half-life](half-life.md) is

$$
t_{1/2}=\frac{\ln2}{k}=\frac{\ln2}{0.2}\,\mathrm s\approx3.4657\,\mathrm s.
$$

At each successive [half-life](half-life.md), half the remaining [reactant](reactant.md) is consumed; $t_{1/2}$ is independent of $A_0$ for this [first-order reaction](first-order-reaction.md). At $t=10\,\mathrm s$, the calculated values are $[\mathrm A]\approx0.135335\,\mathrm{mol\,L^{-1}}$, $[\mathrm B]\approx0.864665\,\mathrm{mol\,L^{-1}}$, and $v\approx0.027067\,\mathrm{mol\,L^{-1}\,s^{-1}}$. These are model predictions for chosen parameters, rather than experimental measurements.

<a id="image-illustrative-first-order-reaction-reactant-loss-reaction-product-formation-and-declining-reaction-rate-for-k-0-2-mathrm-s-1"></a>
![](chemical-first-order-reaction.png)

**[Figure 14](#image-illustrative-first-order-reaction-reactant-loss-reaction-product-formation-and-declining-reaction-rate-for-k-0-2-mathrm-s-1). Illustrative first-order reaction: reactant loss, reaction product formation, and declining reaction rate for $k=0.2\,\mathrm{s^{-1}}$**.

The left panel tracks the two [concentrations](concentration.md); the right tracks their instantaneous conversion [reaction rate](reaction-rate.md). Their different vertical units matter: $v=k[\mathrm A]$, so the numerical curves need not have the same height. This gives a practical way to translate a measured [concentration](concentration.md) into a forecast of both conversion and waiting time.

**Table of contents**

- [First-order rate constant](first-order-rate-constant.md)

## ↑ Ancestors (7)

1. [Order of reaction](order-of-reaction.md)
2. [Rate law](rate-law.md)
3. [Reaction rate](reaction-rate.md)
4. [Chemical kinetics](chemical-kinetics-split.md)
5. [Chemical reaction](chemical-reaction-split.md)
6. [Chemistry](chemistry-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Activation energy](activation-energy.md)
- [Apparent activation energy](apparent-activation-energy.md)
- [Arrhenius equation](arrhenius-equation.md)
- [Catalyst](catalyst.md)
- [Catalytic selectivity](catalytic-selectivity.md)
- [Conductometric determination of activation energy](conductometric-determination-of-activation-energy.md)
- [Consecutive first-order reaction mechanism](consecutive-first-order-reaction-mechanism.md)
- [Elementary reaction](elementary-reaction.md)
- [First-order reaction](first-order-reaction.md)
- [Morphogen gradient](morphogen-gradient.md)
- [Order of reaction](order-of-reaction.md)
- [Parallel first-order reaction mechanism](parallel-first-order-reaction-mechanism.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/4/a/iii/solution.md)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3/3/a/solution.md)
- [Pre-exponential factor](pre-exponential-factor.md)
- [Pseudo-first-order reaction](pseudo-first-order-reaction.md)
- [Rate constant](rate-constant.md)
- [Reversible catalytic relaxation](reversible-catalytic-relaxation.md)
- [Second-order reaction](second-order-reaction.md)
- [Selective biochemical reaction pathways](selective-biochemical-reaction-pathways.md)
