# Wheatstone bridge detector loading

↑ **Parent:** [Wheatstone bridge](wheatstone-bridge.md)

A real [voltmeter](voltmeter.md) has finite input [electrical resistance](electrical-resistance.md) $R_d$; a [galvanometer](galvanometer.md) also has a finite winding [electrical resistance](electrical-resistance.md). Away from balance, its [electric current](electric-current.md) changes both intermediate [electric potentials](electric-potential.md). This is [voltmeter loading](voltmeter-loading.md) when the detector is a [voltmeter](voltmeter.md). Model the detector as a passive [resistor](resistor.md), with no offset or injected [electric current](electric-current.md). [Thévenin's theorem](thevenin-s-theorem.md) supplies the full response without pretending the connected bridge remains two independent [voltage dividers](voltage-divider.md).

With the detector removed, the equivalent source is $V_{\mathrm{oc}}$. Replace the ideal supply by a wire to calculate the source [electrical resistance](electrical-resistance.md) seen between $B,C$: nodes $A,D$ merge, making $R_1,R_2$ parallel and $R_3,R_x$ parallel. Consequently

$$
R_{\mathrm{th}}=\frac{R_1R_2}{R_1+R_2}+\frac{R_3R_x}{R_3+R_x},\qquad
I_d=\frac{V_{\mathrm{oc}}}{R_{\mathrm{th}}+R_d},\qquad
V_d=I_dR_d=V_{\mathrm{oc}}\frac{R_d}{R_{\mathrm{th}}+R_d}.
$$

Since the attenuation factor is strictly positive for $R_d>0$, the null remains $R_2R_3=R_1R_x$. A smaller detector [electrical resistance](electrical-resistance.md) reduces the measured [electric potential difference](electric-potential-difference.md) off balance but does not shift the ideal null. Its [electric current](electric-current.md) sensitivity instead depends on $1/(R_{\mathrm{th}}+R_d)$; detector gain and resolution also matter in deciding how closely a null can be located.

<a id="wheatstone-bridge-detector-voltage-and-loading"></a>
![](wheatstone-bridge-detector-voltage-and-loading.png)

**[Figure 2](#wheatstone-bridge-detector-voltage-and-loading). Finite detector resistance reduces bridge voltage sensitivity while preserving the null**. [Source](wheatstone-bridge-detector-voltage-and-loading.py). Calculated curves use $V_s=5\,\mathrm V$ and $R_1=R_2=R_3=1\,\mathrm{k\Omega}$. All cross zero at $R_x=1\,\mathrm{k\Omega}$; the inset resolves their different slopes. These curves are a model, not measured data.

In the plotted example, $R_x=1.100\,\mathrm{k\Omega}$ gives $V_{\mathrm{oc}}=-119.048\,\mathrm{mV}$ and $R_{\mathrm{th}}=1.02381\,\mathrm{k\Omega}$. A detector with $R_d=1.000\,\mathrm{k\Omega}$ instead reads $V_d=-58.824\,\mathrm{mV}$. Using that loaded reading in the unloaded [voltage divider](voltage-divider.md) formula would underestimate the deviation of $R_x$ from $1\,\mathrm{k\Omega}$. Balancing the bridge avoids this particular systematic [measurement error](measurement-error.md).

The local [derivative](derivative.md) makes the sensitivity explicit. For $R_1=R_2=R_3=R$ and $R_x=R+\delta R$, the first-order [Taylor expansion](taylor-expansion.md) is

$$
V_d=-\frac{V_s}{4R}\frac{R_d}{R+R_d}\,\delta R+O((\delta R)^2).
$$

At the plotted null, the open-circuit slope is $-1.25\,\mathrm{mV/\Omega}$, compared with $-0.625\,\mathrm{mV/\Omega}$ for $R_d=1\,\mathrm{k\Omega}$. Increasing the supply improves this ideal sensitivity but also increases [Joule heating](joule-heating.md). A finite source [electrical resistance](electrical-resistance.md) requires recomputing $R_{\mathrm{th}}$; the displayed parallel-pair expression assumes an ideal supply.

## ↑ Ancestors (5)

1. [Wheatstone bridge](wheatstone-bridge.md)
2. [Resistance bridge](resistance-bridge.md)
3. [Electrical measurement](electrical-measurement.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thévenin's theorem](thevenin-s-theorem.md)
