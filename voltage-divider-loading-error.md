# Voltage divider loading error

↑ **Parent:** [Voltage divider](voltage-divider.md)

For $R_1,R_2,R_L>0$ and $V_s\ne0$, define the fractional shortfall in output magnitude from the unloaded value by

$$
e=\frac{|V_0|-|V_{\mathrm{out}}|}{|V_0|}
=1-\frac{V_{\mathrm{out}}}{V_0}
=\frac{R_{\mathrm{th}}}{R_L+R_{\mathrm{th}}},\qquad
R_{\mathrm{th}}=\frac{R_1R_2}{R_1+R_2}.
$$

This is a loading bias relative to the unloaded target, not the uncertainty of an instrument's measurement of the connected circuit. The equality with the signed ratio also holds for negative $V_s$, because the output retains its sign. The [Thévenin resistance](thevenin-resistance.md) $R_{\mathrm{th}}=R_1\parallel R_2$ summarizes the divider's susceptibility: the relevant comparison is $R_L/R_{\mathrm{th}}$, not merely a large absolute $R_L$.

Set $a=R_1/R_2>0$ and $x=R_L/R_2>0$. Then

$$
e=\frac{a}{a+(a+1)x},\qquad
\frac{de}{dx}=-\frac{a(a+1)}{\bigl(a+(a+1)x\bigr)^2}<0.
$$

The [derivative](derivative.md) proves that increasing the load [electrical resistance](electrical-resistance.md) always reduces this error. For equal divider arms, $e=1/(1+2x)$: $x=1$ gives $33\tfrac13\%$, $x=10$ gives $100/21\%=4.7619\ldots\%$, and $x=100$ gives $100/201\%=0.497512\ldots\%$. Thus a “ten times the lower resistor” rule does not guarantee one-percent agreement with the unloaded target.

<a id="image-fractional-loading-error-falls-continuously-as-the-load-resistance-grows-relative-to-the-lower-divider-arm"></a>
![](voltage-divider-loading-error-versus-load-ratio.png)

**[Figure 13](#image-fractional-loading-error-falls-continuously-as-the-load-resistance-grows-relative-to-the-lower-divider-arm). Fractional loading error falls continuously as the load resistance grows relative to the lower divider arm**. [Source](voltage-divider-loading-error-versus-load-ratio.py). Original exact resistance-only predictions for three $R_1/R_2$ ratios. The logarithmic axes show the equal-arm examples $R_L/R_2=1,10,100$, including the stipulated $1\,\mathrm{M\Omega}$ load on a $10\,\mathrm{k\Omega}$ lower arm. No points represent measurements.

A quantitative design requirement follows without a rule of thumb. For a specified $0<\epsilon<1$,

$$
e\le\epsilon\quad\Longleftrightarrow\quad
R_L\ge R_{\mathrm{th}}\frac{1-\epsilon}{\epsilon}.
$$

For equal $10\,\mathrm{k\Omega}$ arms, $R_{\mathrm{th}}=5\,\mathrm{k\Omega}$, so one-percent loading error requires $R_L\ge495\,\mathrm{k\Omega}$. Reducing both divider [electrical resistances](electrical-resistance.md) reduces loading but increases unloaded supply [electric current](electric-current.md) and [Joule heating](joule-heating.md): $P=V_s^2/(R_1+R_2)$. The stipulated equal-arm example dissipates $5\,\mathrm{mW}$ in total when unloaded. This tradeoff explains why the ratio alone does not determine a useful divider.

## ↑ Ancestors (3)

1. [Voltage divider](voltage-divider.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Resistor tolerance](resistor-tolerance.md)
- [Voltmeter loading](voltmeter-loading.md)
