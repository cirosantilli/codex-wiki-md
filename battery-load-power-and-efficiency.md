# Battery load power and efficiency

↑ **Parent:** [Electric battery](electric-battery.md)

In the constant-parameter [battery internal resistance](battery-internal-resistance.md) model, the source's available electrical [power](power.md) splits between the [electrical load](electrical-load.md) and internal dissipation:

$$
\mathcal E I=\underbrace{V_LI}_{P_L}+\underbrace{I^2r}_{P_{\rm int}},\qquad
P_L=\frac{\mathcal E^2R}{(R+r)^2},\qquad
P_{\rm int}=\frac{\mathcal E^2r}{(R+r)^2}.
$$

The stipulated $3\,\mathrm V$, $1\,\Omega$, $4\,\Omega$ calculation gives $P_L=1.44\,\mathrm W$, $P_{\rm int}=0.36\,\mathrm W$, and $\mathcal E I=1.80\,\mathrm W$. A resistive [electrical load](electrical-load.md) converts its share to [Joule heating](joule-heating.md); another [electrical load](electrical-load.md) might convert some of it to mechanical [work](work.md) or [light](light.md). The source term is available electrical [work](work.md) per time, not a complete cell [heat](heat-split.md) budget: reaction [entropy](entropy-split.md) can also matter.

<a id="image-calculated-battery-terminal-voltage-power-and-delivery-efficiency-versus-load-resistance"></a>
![](battery-load-voltage-power-efficiency.png)

**[Figure 12](#image-calculated-battery-terminal-voltage-power-and-delivery-efficiency-versus-load-resistance). Calculated battery terminal voltage, power and delivery efficiency versus load resistance**. Original predictions for constant $\mathcal E=3\,\mathrm V$ and $r=1\,\Omega$. Circles mark $R=4\,\Omega$; dashed vertical lines mark $R=r$. The three panels have distinct vertical units. Delivery efficiency is $\eta=P_L/(\mathcal E I)$ for finite discharge [electric current](electric-current.md); its open-circuit limit is one although both input and output [power](power.md) vanish. The $R=0$ endpoint is a mathematical limiting model, not an experimental instruction. No measured data or copied source figure is used.

Define the delivery efficiency relative to the source's available electrical [work](work.md), rather than to all chemical [energy](energy-split.md) or to a complete charging cycle:

$$
\eta=\frac{P_L}{\mathcal E I}=\frac{V_L}{\mathcal E}=\frac{R}{R+r}.
$$

Here $\eta=0.80$. The largest load [power](power.md) occurs at $R=r$: since $(R+r)^2\geq4Rr$,

$$
P_L\leq\frac{\mathcal E^2}{4r},\qquad
P_L\big|_{R=r}=2.25\,\mathrm W,\qquad
\eta\big|_{R=r}=\frac12.
$$

Thus maximum load [power](power.md) and maximum delivery efficiency ask different questions. As $R\to\infty$, $V_L\to\mathcal E$ and $\eta\to1$, but $I\to0$ and $P_L\to0$: a high nearly unloaded voltage supplies almost no [power](power.md). As $R\to0$, the model gives $V_L\to0$, $P_L\to0$ and internal [power](power.md) tending to $\mathcal E^2/r$. Real high-current operation can invalidate constant $r$ and $\mathcal E$; the mathematical maximum does not establish a permissible operating point for an actual [battery](electric-battery.md).

## ↑ Ancestors (6)

1. [Electric battery](electric-battery.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
