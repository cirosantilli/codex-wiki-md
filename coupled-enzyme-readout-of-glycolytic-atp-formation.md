# Coupled-enzyme readout of glycolytic ATP formation

↑ **Parent:** [Glycolysis](glycolysis.md)

The final [substrate-level phosphorylation](substrate-level-phosphorylation.md) in [glycolysis](glycolysis.md) provides a useful experimental handle: [pyruvate kinase](pyruvate-kinase.md) transfers a [phosphate](phosphate.md) group from [phosphoenolpyruvate](phosphoenolpyruvate.md) to [ADP](adenosine-diphosphate.md), producing [pyruvate](pyruvate.md) and [ATP](adenosine-triphosphate.md). Adding [lactate dehydrogenase](lactate-dehydrogenase.md) couples each [pyruvate](pyruvate.md) formed to consumption of one [NADH](nadh.md):

$$
\begin{aligned}
\mathrm{phosphoenolpyruvate}+\mathrm{ADP}+\mathrm H^+
&\longrightarrow\mathrm{pyruvate}+\mathrm{ATP},\\
\mathrm{pyruvate}+\mathrm{NADH}+\mathrm H^+
&\longrightarrow\mathrm{lactate}+\mathrm{NAD}^{+}.
\end{aligned}
$$

These equations select free ionic forms consistently: [phosphoenolpyruvate](phosphoenolpyruvate.md) has charge $-3$, [ADP](adenosine-diphosphate.md) $-3$, [ATP](adenosine-triphosphate.md) $-4$, and [pyruvate](pyruvate.md) and [lactate](lactate.md) each $-1$; [NAD+](nad-plus.md) has one more positive charge than [NADH](nadh.md). Each line conserves charge. Cancelling [pyruvate](pyruvate.md) gives one [NADH](nadh.md) consumed per [ATP](adenosine-triphosphate.md) formed in this coupled system. A whole-pathway [NADH](nadh.md) measurement has a different meaning, because the earlier [glycolysis](glycolysis.md) [redox](redox.md) step produces [NADH](nadh.md).

The published An Optimized Enzyme-Coupled Spectrophotometric Method for Measuring Pyruvate Kinase Kinetics reports recombinant [pyruvate kinase](pyruvate-kinase.md) prepared in [Escherichia coli](escherichia-coli.md), purified by [chromatography](chromatography-split.md) and [size-exclusion chromatography](size-exclusion-chromatography.md). UV-transparent microplate wells contained [ADP](adenosine-diphosphate.md), [phosphoenolpyruvate](phosphoenolpyruvate.md), [NADH](nadh.md), [lactate dehydrogenase](lactate-dehydrogenase.md) and a [buffer solution](buffer-solution.md) with [magnesium](magnesium.md) [ions](ion.md). An Epoch plate reader used [spectrophotometry](spectrophotometry.md) to follow [absorbance](absorbance.md) at $340\,\mathrm{nm}$ every five to ten seconds for one minute at $25\,{}^\circ\mathrm C$. Its Figure 2 presents $A_0-A_t$, increasing as [NADH](nadh.md) is consumed. Heat-inactivated [pyruvate kinase](pyruvate-kinase.md) gave minimal background; a validated active preparation was the positive control. These comparisons support an [enzyme](enzyme-split.md)-dependent readout in the prepared system, rather than a whole-[biological cell](biological-cell-split.md) [glycolysis](glycolysis.md) measurement.[Procedure A.5–6 and B.2; Equipment item 1; Figure 2 and caption; Validation of protocol: preparation, optical readout and controls](an-optimized-enzyme-coupled-spectrophotometric-method-for-measuring-pyruvate-kinase-kinetics-by-saurabh-upadhyay.md)

The same report uses $0.5\,\mathrm{cm}$ for optical path length in Procedure B.2.i, but approximately $0.3\,\mathrm{cm}$ in Data analysis §3. An absolute conversion requires the actual path length and sufficient coupling [enzyme](enzyme-split.md) activity; no measured [ATP](adenosine-triphosphate.md) rate is inferred here.[Procedure B.2.i; Data analysis §3; General notes, items 4 and 6: path-length inconsistency and linear-range conditions](an-optimized-enzyme-coupled-spectrophotometric-method-for-measuring-pyruvate-kinase-kinetics-by-saurabh-upadhyay.md)

For an original dimensional example, stipulate a blank-corrected [absorbance](absorbance.md) decline $-dA_{340}/dt=0.024\,\mathrm{min^{-1}}$, a calibrated path length $\ell=0.40\,\mathrm{cm}$ and a chosen calibration coefficient $\varepsilon=6000\,\mathrm{L\,mol^{-1}\,cm^{-1}}$. These are invented teaching inputs, not the protocol's measurements or its quoted coefficient. The [Beer-Lambert law](beer-lambert-law.md) gives

$$
A_{340}=\varepsilon\ell c_{\mathrm{NADH}},\qquad
-\frac{dc_{\mathrm{NADH}}}{dt}
=\frac{0.024}{6000\times0.40}
=10^{-5}\,\mathrm{mol\,L^{-1}\,min^{-1}}.
$$

In a stipulated $0.20\,\mathrm{mL}$ reaction [volume](volume-thermodynamics.md), this is $2\,\mathrm{nmol\,min^{-1}}$ of [NADH](nadh.md) consumed and, conditionally, $2\,\mathrm{nmol\,min^{-1}}$ of [ATP](adenosine-triphosphate.md) formed. The conditional inference requires rapid [pyruvate](pyruvate.md) consumption by the coupling [enzyme](enzyme-split.md), no other [NADH](nadh.md)-consuming [chemical reactions](chemical-reaction-split.md), and a linear, correctly calibrated optical response. The readout measures this last [glycolysis](glycolysis.md) step; it cannot establish the full two-net-[ATP](adenosine-triphosphate.md)-per-[glucose](glucose.md) balance by itself.

## ↑ Ancestors (5)

1. [Glycolysis](glycolysis.md)
2. [Metabolic pathway](metabolic-pathway.md)
3. [Biochemistry](biochemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Substrate-level phosphorylation](substrate-level-phosphorylation.md)
