# Nuclear pore transport balance

↑ **Parent:** [Nuclear pore complex](nuclear-pore-complex.md)

Nuclear accumulation should compare [concentrations](concentration.md), not just total cargo. In an original constructed example, a [cell nucleus](cell-nucleus.md) occupies one [volume](volume-thermodynamics.md) unit and the accessible [cytosol](cytosol.md) occupies nine. Of $130$ tracer units, $40$ are nuclear and $90$ are cytosolic. With $n_n,n_c$ the amounts and $V_n,V_c$ the accessible [volume](volume-thermodynamics.md), the [concentration](concentration.md) ratio is

$$
C_n=\frac{n_n}{V_n}=40,\qquad C_c=\frac{n_c}{V_c}=10,\qquad R=\frac{C_n}{C_c}=4.
$$

Only $40/130=4/13\approx30.8\%$ of the cargo is nuclear, yet nuclear [concentration](concentration.md) is four times cytosolic [concentration](concentration.md). A majority outside the [cell nucleus](cell-nucleus.md) does not rule out nuclear enrichment.

For comparison, freely exchanging nonbinding cargo at equal [concentrations](concentration.md) would have $n_n=13,n_c=117$: the nuclear fraction would equal the nuclear fraction of accessible [volume](volume-thermodynamics.md), $1/10$. These are constructed amounts, not measurements from the [nuclear pore localization experiment](nuclear-pore-localization-experiment.md). Binding, unequal recovery or cargo degradation would require additional accounting before interpreting an assay.

A minimal two-compartment [ordinary differential equation](ordinary-differential-equation.md) makes the distinction precise. Assume fixed accessible [volume](volume-thermodynamics.md), no synthesis or degradation, and effective first-order exchange rates $a,b>0$:

$$
\frac{dn_n}{dt}=a n_c-b n_n,\qquad n_c=N-n_n,\qquad \frac{dn_c}{dt}=-\frac{dn_n}{dt}.
$$

Total cargo $N=n_n+n_c$ is conserved. Setting the [derivative](derivative.md) to zero gives

$$
n_n^*=\frac{aN}{a+b},\qquad \frac{C_n^*}{C_c^*}=\frac{aV_c}{bV_n}.
$$

For symmetric passive exchange with conductance $P$, $a=P/V_c$ and $b=P/V_n$, so the [concentration](concentration.md) ratio is one even when the amounts differ. Choosing instead $a=4/9$ and $b=1$ in reciprocal model-time units gives $n_n^*=40$ for $N=130,V_n=1,V_c=9$. The exact [ordinary differential equation](ordinary-differential-equation.md) solution is

$$
n_n(t)=n_n^*+\bigl(n_n(0)-n_n^*\bigr)e^{-(a+b)t}.
$$

Substitution verifies the solution, and $a+b>0$ makes departures decay. This effective model can describe an asymmetric exchange balance, but does not by itself identify a [nuclear localization sequence](nuclear-localization-sequence.md), transport receptor or source of [energy](energy-split.md).

The usefulness of the [nuclear pore complex](nuclear-pore-complex.md) is precisely this combination of separation and exchange: a [cell nucleus](cell-nucleus.md) can maintain a distinctive [protein](protein-split.md) population while receiving new cargo and exporting [RNA](ribonucleic-acid.md). The [nuclear pore localization experiment](nuclear-pore-localization-experiment.md) asks what feature controls entry; the [nuclear pore transport balance](nuclear-pore-transport-balance.md) asks what an accumulation readout actually means.

## ↑ Ancestors (6)

1. [Nuclear pore complex](nuclear-pore-complex.md)
2. [Nuclear envelope](nuclear-envelope.md)
3. [Cell nucleus](cell-nucleus.md)
4. [Biological cell](biological-cell-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Nuclear pore transport balance](nuclear-pore-transport-balance.md)
