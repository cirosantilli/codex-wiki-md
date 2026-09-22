# Constant-entropy magnetic cooling example

↑ **Parent:** [Two-level paramagnetic cooling model](two-level-paramagnetic-cooling-model.md)

Choose a fictional two-level refrigerant with $\mu/k_B=1\,\mathrm{K\,T^{-1}}$, where the upright $\mathrm T$ denotes [tesla](tesla-unit.md). This chosen moment is a convenient model parameter, not a fitted property of the historical salt. At bath [temperature](temperature-split.md) $T_b=1\,\mathrm K$, raise $B$ from $0.20\,\mathrm T$ to $1.00\,\mathrm T$. Then $x$ increases from $0.20$ to $1.00$, so

$$
s(0.20)=0.673540\ldots,\qquad s(1)=0.365334\ldots,
\qquad \frac{Q_{\rm in}}{Nk_BT_b}=s(1)-s(0.20)=-0.308206\ldots.
$$

The last equality assumes a reversible [isothermal process](isothermal-process.md) of [magnetization](magnetization.md); negative $Q_{\rm in}$ means the refrigerant rejects [heat](heat-split.md). The bath gains $0.308206\ldots Nk_B$ of [entropy](entropy-split.md), balancing the stage's loss in this reversible limit. An appreciable [temperature](temperature-split.md) difference during real [heat transfer](heat-transfer.md) adds [entropy production](entropy-production.md).

Now open the [heat switch](heat-switch.md) and reduce $B$ from $1.00\,\mathrm T$ to $0.10\,\mathrm T$. Constant $x=1$ gives $T_f=0.10\,\mathrm K$. Throughout this ideal cooling leg, $p_-=0.880797\ldots$, $p_+=0.119203\ldots$, and $S_{\rm mag}=0.365334\ldots Nk_B$. Neither state becomes more probable. Field reduction shrinks the [energy](energy-split.md) gap by ten while preserving the [Boltzmann distribution](boltzmann-distribution.md)'s dimensionless ratio of gap to [temperature](temperature-split.md).

<a id="paramagnetic-entropy-cooling-curves"></a>
![](paramagnetic-entropy-cooling-curves.png)

**[Figure 2](#paramagnetic-entropy-cooling-curves). Magnetic entropy curves and an original isothermal process followed by cooling**. [Source](paramagnetic-entropy-cooling-curves.py). Left: the calculated two-level [magnetic entropy](magnetic-entropy.md) at three chosen [magnetic fields](magnetic-field-split.md). Right: constant-[entropy](entropy-split.md) curves in the positive field–[temperature](temperature-split.md) plane. A to B exports [entropy](entropy-split.md) to a bath at $1\,\mathrm K$; B to C keeps $x=1$. All curves are ideal-model calculations, with no experimental points.

There is a subtle [energy](energy-split.md) check. For the spin [Hamiltonian](hamiltonian.md) convention used here, external-field interaction [energy](energy-split.md) belongs to $U_{\rm mag}$, so reversible [work](work.md) done on the spin subsystem is $\delta W_{\rm on}=-m\,dB$ and

$$
dU_{\rm mag}=T\,dS_{\rm mag}-m\,dB.
$$

On the isolated leg, $Q=0$ but $U_{\rm mag}$ increases from $-0.761594\ldots Nk_B\,\mathrm K$ to $-0.0761594\ldots Nk_B\,\mathrm K$, becoming less negative as the gap shrinks. Integrating $-m\,dB$ at constant $x=1$ supplies exactly $+0.685435\ldots Nk_B\,\mathrm K$. Cooling therefore need not decrease this chosen spin [internal energy](internal-energy-split.md). An account of [work](work.md) exchanged with a magnet circuit must specify where field interaction [energy](energy-split.md) is assigned before comparing signs. The occupation ratio and [temperature](temperature-split.md) prediction do not depend on that bookkeeping choice.

For the isothermal preparation, direct integration gives $W_{\rm on}/(Nk_BT_b)=-\ln[\cosh(1)/\cosh(0.20)]=-0.413913\ldots$. The endpoint [internal energy](internal-energy-split.md) difference is $-0.722119\ldots Nk_BT_b$, equal to $Q_{\rm in}+W_{\rm on}$. This independently checks both the rejected [heat](heat-split.md) and the magnetic-work sign in the chosen convention.

## ↑ Ancestors (9)

1. [Two-level paramagnetic cooling model](two-level-paramagnetic-cooling-model.md)
2. [Magnetic entropy](magnetic-entropy.md)
3. [Adiabatic demagnetization](adiabatic-demagnetization.md)
4. [Temperature](temperature-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
