# Finite calcium-store release model

↑ **Parent:** [IP3-sensitive calcium store](ip3-sensitive-calcium-store.md)

For an original [mathematical model](mathematical-model.md), imagine a sustained, imposed release pathway, with no store refill during the plotted interval. Let $S$ be releasable store [amount of substance](amount-of-substance.md), $X$ excess freely dissolved cytosolic [calcium](calcium.md) [amount of substance](amount-of-substance.md), and $Q$ the cumulative amount removed from $X$ into a separate sink. Choose $S(0)=1\,\mathrm{amol}$, $X(0)=Q(0)=0$, cytosolic [volume](volume.md) $V_c=1\,\mathrm{pL}$, release [rate constant](rate-constant.md) $k=0.4\,\mathrm{s^{-1}}$ and clearance [rate constant](rate-constant.md) $h=0.8\,\mathrm{s^{-1}}$. These are stipulated values, not physiological measurements or a model of [IP3 receptor](inositol-trisphosphate-receptor.md) gating.

Assume fixed [volume](volume.md), uniform mixing, no binding, no reverse transfer, no outside entry and first-order loss from each donating compartment. Then

$$
\frac{dS}{dt}=-kS,\qquad \frac{dX}{dt}=kS-hX,\qquad \frac{dQ}{dt}=hX,\qquad S+X+Q=S(0).
$$

The last equality is [conservation of mass](mass-conservation.md) for the tracked [calcium](calcium.md) across the store, mobile excess and sink together; it does not assert conservation inside a [biological cell](biological-cell-split.md) if the sink represents export. A constant background $c_b=0.1\,\mathrm{\mu M}$ is held separate from this excess bookkeeping. Since $1\,\mathrm{amol}/1\,\mathrm{pL}=1\,\mathrm{\mu M}$, the response is $c=c_b+X/V_c$.

<a id="image-declining-store-release-rate-and-a-delayed-cytosolic-calcium-peak"></a>
![](ip3-finite-store-release-and-cytosolic-response.png)

**[Figure 4](#image-declining-store-release-rate-and-a-delayed-cytosolic-calcium-peak). Declining store-release rate and a delayed cytosolic calcium peak**. Original analytic toy-model curves with $S(0)=1\,\mathrm{amol}$, $V_c=1\,\mathrm{pL}$, $k=0.4\,\mathrm{s^{-1}}$, $h=0.8\,\mathrm{s^{-1}}$ and background $c_b=0.1\,\mathrm{\mu M}$. The left panel plots release rate $kS$; the right plots $c_b+X/V_c$. Sustained effective release permeability is imposed even as the store empties. These are different quantities with different units, not reconstructed experimental data or physiological timings. The sink receives all cleared excess; refill, binding and [IP3 receptor](inositol-trisphosphate-receptor.md) regulation are omitted.

Solving these [ordinary differential equations](ordinary-differential-equation.md) gives

$$
S=S(0)e^{-kt},\qquad X=\frac{kS(0)}{h-k}\left(e^{-kt}-e^{-ht}\right),\qquad Q=S(0)-S-X.
$$

Release $kS$ declines from the start, yet $X$ initially rises because delivery exceeds clearance. Its peak occurs when $kS=hX$, at $t_*=\log(h/k)/(h-k)=\log(2)/0.4\approx1.73\,\mathrm{s}$. There $X=0.25\,\mathrm{amol}$ and $c=0.35\,\mathrm{\mu M}$. Ultimately $S$ and $X$ tend to zero, $Q$ tends to $1\,\mathrm{amol}$ and $c$ returns to $c_b$. The delayed peak is a consequence of material balance, even though this model has no delayed channel activation.

This distinction guides interpretation: a large released amount need not mean a large simultaneous free cytosolic [concentration](concentration.md). Clearance and [volume](volume.md) intervene. Real [biological cells](biological-cell-split.md) add binding, store refilling, [IP3](inositol-trisphosphate.md) turnover and [IP3 receptor](inositol-trisphosphate-receptor.md) regulation; the two plotted curves isolate one finite-store effect rather than explaining every [calcium](calcium.md) response.

## ↑ Ancestors (6)

1. [IP3-sensitive calcium store](ip3-sensitive-calcium-store.md)
2. [Inositol trisphosphate](inositol-trisphosphate.md)
3. [Second messenger](second-messenger.md)
4. [Signal transduction](signal-transduction-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)
