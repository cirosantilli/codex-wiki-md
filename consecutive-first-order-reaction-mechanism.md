# Consecutive first-order reaction mechanism

↑ **Parent:** [Reaction mechanism](reaction-mechanism.md)

A [consecutive first-order reaction mechanism](consecutive-first-order-reaction-mechanism.md) passes material through a [reaction intermediate](reaction-intermediate.md). Consider a stipulated [chemical reaction network](chemical-reaction-network.md) $\mathrm A\xrightarrow{k_1}\mathrm I\xrightarrow{k_2}\mathrm P$, with constant positive [rate constants](rate-constant.md), fixed [temperature](temperature-split.md) and [volume](volume.md), uniform mixing, and no reverse or competing [chemical reactions](chemical-reaction-split.md). All three labels carry one conserved unit of material. Set $[\mathrm A](0)=A_0>0$ and $[\mathrm I](0)=[\mathrm P](0)=0$. The [law of mass action](law-of-mass-action.md) gives

$$
\frac{d[\mathrm A]}{dt}=-k_1[\mathrm A],\qquad
\frac{d[\mathrm I]}{dt}=k_1[\mathrm A]-k_2[\mathrm I],\qquad
\frac{d[\mathrm P]}{dt}=k_2[\mathrm I].
$$

Adding the three [rate equations](rate-equation.md) proves $[\mathrm A]+[\mathrm I]+[\mathrm P]=A_0$. Each step has a [first-order reaction](first-order-reaction.md) [rate law](rate-law.md); this does not make all three [concentrations](concentration.md) simple [exponential decays](exponential-decay.md).

For $k_1\ne k_2$, the exact solution is

$$
[\mathrm A]=A_0e^{-k_1t},\qquad
[\mathrm I]=A_0\frac{k_1}{k_2-k_1}\left(e^{-k_1t}-e^{-k_2t}\right),\qquad
[\mathrm P]=A_0-[\mathrm A]-[\mathrm I].
$$

To derive the middle expression, substitute the first into the [first-order linear differential equation](first-order-linear-differential-equation.md) for I and multiply by the [integrating factor](integrating-factor.md) $e^{k_2t}$. Then $d(e^{k_2t}[\mathrm I])/dt=k_1A_0e^{(k_2-k_1)t}$, which can be integrated directly with the stated [initial condition](initial-condition.md). The material balance supplies P without another integration.

The apparent division by zero at equal [rate constants](rate-constant.md) is removable. For $k_1=k_2=k$, the same [integrating factor](integrating-factor.md) gives

$$
[\mathrm I]=A_0kte^{-kt},\qquad
[\mathrm P]=A_0\bigl[1-(1+kt)e^{-kt}\bigr].
$$

This is also the [limit](limit-of-a-function.md) of the unequal-[rate constant](rate-constant.md) expression. Initially $[\mathrm P]/A_0=(kt)^2/2+O((kt)^3)$, so [reaction product](product-chemistry.md) formation begins with zero slope despite immediate [reactant](reactant.md) loss. By contrast, a direct $\mathrm A\longrightarrow\mathrm P$ [first-order reaction](first-order-reaction.md) with the same $k$ has $[\mathrm P]/A_0=1-e^{-kt}$ and nonzero initial slope. Their A traces agree exactly; their P traces do not.

<a id="image-consecutive-reaction-intermediate-time-profiles"></a>
![](consecutive-reaction-intermediate-time-profiles.png)

**[Figure 4](#image-consecutive-reaction-intermediate-time-profiles). An accumulating reaction intermediate delays reaction product formation in a consecutive first-order reaction mechanism**. Original chosen model with $k_1=k_2=0.20\,\mathrm{s^{-1}}$ and $A_0=1.00\,\mathrm{mmol\,L^{-1}}$. Solid curves follow the exact three-species [rate equations](rate-equation.md); the dashed P curve is a separate direct A-to-P model with the same A trace. These are model predictions, not measurements or an identified molecular [reaction mechanism](reaction-mechanism.md).

For the chosen equal-[rate constant](rate-constant.md) example, I peaks at $t=1/k=5.00\,\mathrm s$, because $d[\mathrm I]/dt=A_0ke^{-kt}(1-kt)$. At that time $[\mathrm A]=[\mathrm I]=A_0/e\approx0.367879\,\mathrm{mmol\,L^{-1}}$ and $[\mathrm P]\approx0.264241\,\mathrm{mmol\,L^{-1}}$; the direct model would already have $[\mathrm P]\approx0.632121\,\mathrm{mmol\,L^{-1}}$. The peak means formation and consumption of I are momentarily equal, not that the whole system has reached [chemical equilibrium](chemical-equilibrium.md).

More generally the peak is at $t_*=\ln(k_2/k_1)/(k_2-k_1)$, which is positive for either ordering of the two positive [rate constants](rate-constant.md) and tends to $1/k$ as they coincide. When $k_2\gg k_1$, a brief initial adjustment can be followed by $[\mathrm I]\approx(k_1/k_2)[\mathrm A]$ and approximately equal formation and consumption [reaction rates](reaction-rate.md). The exact solution states when this small-intermediate approximation can be reasonable. It is inappropriate for the illustrated equal-[rate constant](rate-constant.md) case: at the peak, over one third of the conserved material is I. Such timing matters if the goal is to collect a useful [reaction intermediate](reaction-intermediate.md) before it becomes the final [reaction product](product-chemistry.md).

## ↑ Ancestors (5)

1. [Reaction mechanism](reaction-mechanism.md)
2. [Chemical kinetics](chemical-kinetics-split.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Consecutive first-order reaction mechanism](consecutive-first-order-reaction-mechanism.md)
- [Elementary reaction](elementary-reaction.md)
- [Reaction intermediate](reaction-intermediate.md)
- [Reaction mechanism](reaction-mechanism.md)
