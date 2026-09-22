# Reversible catalytic relaxation

↑ **Parent:** [Catalysis](catalysis.md)

Here is an explicitly stipulated elementary kinetic model, not experimental data. A well-mixed ideal [closed system](closed-system.md) has constant [temperature](temperature-split.md) and [volume](volume.md). Alongside an uncatalysed [elementary reaction](elementary-reaction.md), allow an illustrative catalytic encounter that returns C immediately:

$$
\begin{aligned}
\mathrm A&\rightleftharpoons\mathrm B,
& k_f^u&=0.030\,\mathrm{s^{-1}},
& k_r^u&=0.010\,\mathrm{s^{-1}},\\
\mathrm A+\mathrm C&\rightleftharpoons\mathrm B+\mathrm C,
& \alpha_f&=270\,\mathrm{L\,mol^{-1}\,s^{-1}},
& \alpha_r&=90\,\mathrm{L\,mol^{-1}\,s^{-1}}.
\end{aligned}
$$

Both channels obey the [law of mass action](law-of-mass-action.md). In the second, the forward [reaction rate](reaction-rate.md) is $\alpha_f[\mathrm A][\mathrm C]$ and the reverse [reaction rate](reaction-rate.md) is $\alpha_r[\mathrm B][\mathrm C]$. C cancels in each encounter, so its free [concentration](concentration.md) $c_C$ stays constant without an external supply. This toy [elementary reaction](elementary-reaction.md) encodes regeneration without binding; it is not a claim that real [catalytic cycles](catalytic-cycle.md) universally consist of one encounter. A binding cycle can accumulate a [reaction intermediate](reaction-intermediate.md), in which case constant total C does not imply constant free $c_C$.

Adding the parallel [reaction rates](reaction-rate.md) gives effective [first-order reaction](first-order-reaction.md) [rate constants](rate-constant.md)

$$
k_f=k_f^u+\alpha_f c_C,
\qquad k_r=k_r^u+\alpha_r c_C.
$$

Because $k_f^u/k_r^u=\alpha_f/\alpha_r=3$, each channel balances at the same $[\mathrm B]/[\mathrm A]=3$, and so does their sum. At $c_C=0$ the pair is $(0.030,0.010)\,\mathrm{s^{-1}}$; at $c_C=0.001\,\mathrm{mol\,L^{-1}}$ it is $(0.300,0.100)\,\mathrm{s^{-1}}$. Both give $K=3$ with ideal [thermodynamic activities](thermodynamic-activity.md) and a common concentration [standard state](standard-state.md). At $T=300\,\mathrm K$ their compatible standard reaction change in [Gibbs free energy](gibbs-free-energy.md) is $\Delta_rG^\circ=-RT\ln3\approx-2.7403\,\mathrm{kJ\,mol^{-1}}$. Choosing an unrelated reverse [rate constant](rate-constant.md) would break this consistency.

Let $S=[\mathrm A]+[\mathrm B]$ be the conserved [concentration](concentration.md), and define the [dimensionless quantity](dimensionless-quantity.md) $x=[\mathrm B]/S$. Then

$$
\frac{dx}{dt}=k_f(1-x)-k_rx
=-(k_f+k_r)(x-x_{\mathrm{eq}}),
\qquad
x_{\mathrm{eq}}=\frac{k_f}{k_f+k_r}=\frac34.
$$

Solving this [first-order linear differential equation](first-order-linear-differential-equation.md) gives

$$
x(t)=\frac34+\left(x_0-\frac34\right)e^{-(k_f+k_r)t},
\qquad
\tau=\frac{1}{k_f+k_r}.
$$

The [chemical relaxation time](chemical-relaxation-time.md) is $25\,\mathrm s$ without C and $2.5\,\mathrm s$ with the chosen C. From either $x_0=0$ or $x_0=1$, the [exponential decay](exponential-decay.md) of the deviation leads to the same [chemical equilibrium](chemical-equilibrium.md) $x=3/4$. Reducing that deviation to one percent takes $\ln(100)\tau$: about $115.13\,\mathrm s$ versus $11.51\,\mathrm s$.

<a id="image-catalysis-reversible-equilibrium-relaxation"></a>
![](catalysis-reversible-equilibrium-relaxation.png)

**[Figure 8](#image-catalysis-reversible-equilibrium-relaxation). Two initial compositions and two kinetic speeds approach the same chemical equilibrium**. Exact curves from the stipulated [reversible catalytic relaxation](reversible-catalytic-relaxation.md) model. Solid curves include $0.001\,\mathrm{mol\,L^{-1}}$ of C; dashed curves omit C. Blue starts entirely as A and orange entirely as B. Both panels use the same equations; the right panel resolves the first $15\,\mathrm s$. The common dotted line is $[\mathrm B]/([\mathrm A]+[\mathrm B])=3/4$, not a fitted plateau or an experimental measurement.

At this [chemical equilibrium](chemical-equilibrium.md), conversion continues in both directions. For $S=1\,\mathrm{mol\,L^{-1}}$, the uncatalysed channel has equal forward and reverse [reaction rates](reaction-rate.md) $0.0075\,\mathrm{mol\,L^{-1}\,s^{-1}}$. Adding C gives total directional [reaction rates](reaction-rate.md) $0.075\,\mathrm{mol\,L^{-1}\,s^{-1}}$ each, yet zero net [reaction rate](reaction-rate.md). Faster molecular exchange and unchanged composition coexist. This exact calculation explains how [catalysis](catalysis.md) can matter enormously within an observation window while leaving the final [equilibrium constant](equilibrium-constant.md) intact.

## ↑ Ancestors (5)

1. [Catalysis](catalysis.md)
2. [Chemical kinetics](chemical-kinetics-split.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Catalytic barriers and reaction free energy](catalytic-barriers-and-reaction-free-energy.md)
- [Reversible catalytic relaxation](reversible-catalytic-relaxation.md)
