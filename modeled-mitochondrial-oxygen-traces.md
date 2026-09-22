# Modeled mitochondrial oxygen traces

↑ **Parent:** [Isolated mitochondria respiration experiment](isolated-mitochondria-respiration-experiment.md)

The following original model chooses piecewise constant [oxygen](oxygen.md) consumption rates in a closed, well-mixed $2\,\mathrm{mL}$ suspension. It assumes no gas exchange, negligible addition [volume](volume-thermodynamics.md), a corrected sensor and sufficient [oxygen](oxygen.md) throughout. The curves are invented teaching examples, not measured traces, fitted data or a reconstruction of Figure 6.

<a id="image-modeled-oxygen-traces-a-faster-decline-need-not-mean-more-atp"></a>
![](mitochondrial-modeled-oxygen-and-control-readouts.png)

**[Figure 10](#image-modeled-oxygen-traces-a-faster-decline-need-not-mean-more-atp). MODELED oxygen traces: a faster decline need not mean more ATP**. Original piecewise linear [concentration](concentration.md) curve and corresponding consumption-rate plot. All rates and times are chosen. The finite first [ADP](adenosine-diphosphate.md) pulse is stipulated to be used by minute 2; the second supplies excess [ADP](adenosine-diphosphate.md). [Oligomycin](oligomycin.md) remains present after [FCCP](fccp.md). Substrate additions and intermediate chain interventions from the published protocol are omitted. The residual after [antimycin A](antimycin-a.md) is shown as background, not [ATP](adenosine-triphosphate.md) production.

Start at $c(0)=220\,\mathrm{\mu mol\,L^{-1}}$. On successive one-minute intervals, choose positive slope magnitudes $5,25,5,25,6,32,1\,\mathrm{\mu mol\,L^{-1}\,min^{-1}}$. Integration gives the endpoint [concentrations](concentration.md) $220,215,190,185,160,154,122,121\,\mathrm{\mu mol\,L^{-1}}$. This is just the recurrence $c_{i+1}=c_i-r_i\Delta t$, with $\Delta t=1\,\mathrm{min}$; the step plot shows $r_i=-dc/dt$. The trace remains above zero by construction.

During the second [ADP](adenosine-diphosphate.md) interval, the total consumption rate is

$$
q=-V\frac{dc_{\mathrm{O}_2}}{dt}
=(0.002\,\mathrm L)(25\,\mathrm{\mu mol\,L^{-1}\,min^{-1}})
=50\,\mathrm{nmol\,min^{-1}}.
$$

With a stipulated mitochondrial [protein](protein-split.md) mass of $0.20\,\mathrm{mg}$, that is $250\,\mathrm{nmol\,min^{-1}\,mg^{-1}}$. Using a denominator twice as large would halve this reported rate without changing the raw [oxygen](oxygen.md) trace. Comparisons therefore need both loading and the chosen denominator.

For a second bookkeeping check, the modeled post-[antimycin A](antimycin-a.md) slope of $1\,\mathrm{\mu mol\,L^{-1}\,min^{-1}}$ corresponds to $2\,\mathrm{nmol\,min^{-1}}$ background. If that background is additive and unchanged in earlier windows, subtraction gives $48$, $10$ and $62\,\mathrm{nmol\,min^{-1}}$ for excess [ADP](adenosine-diphosphate.md), [oligomycin](oligomycin.md) and [FCCP](fccp.md), respectively. The [oligomycin](oligomycin.md)-sensitive difference is $48-10=38\,\mathrm{nmol\,min^{-1}}$. It is a difference in [oxygen](oxygen.md) consumption under the chosen interventions, not an [ATP](adenosine-triphosphate.md) production rate. Converting it into one requires additional coupling assumptions or an independent [ATP](adenosine-triphosphate.md) measurement; the [FCCP](fccp.md) interval shows why slope alone cannot supply that conversion.

Across the whole seven-minute example, consumption is $V(c(0)-c(7))=198\,\mathrm{nmol}$, also the sum of the seven interval consumptions. This equality checks the rate-to-amount accounting independently of how the intervals are named. Actual records require attention to calibration, mixing transients, background stability and decreasing [oxygen](oxygen.md) availability; a line that steepens or flattens alone does not identify the cause.

## ↑ Ancestors (6)

1. [Isolated mitochondria respiration experiment](isolated-mitochondria-respiration-experiment.md)
2. [Mitochondria](mitochondria.md)
3. [Organelle](organelle.md)
4. [Biological cell](biological-cell-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)
