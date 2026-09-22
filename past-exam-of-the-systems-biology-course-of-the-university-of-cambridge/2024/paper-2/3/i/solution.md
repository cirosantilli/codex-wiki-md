<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Affinity purification and proximity labeling answer related but different questions.** The former enriches material that remains associated during extraction; the latter marks a neighbourhood before extraction. Neither alone proves a direct [protein-protein interaction](../../../../../protein-protein-interaction.md).

In [affinity purification-mass spectrometry](../../../../../affinity-purification-mass-spectrometry.md), isolate a bait [protein](../../../../../protein-split.md) with an [antibody](../../../../../antibody.md) or an endogenous [epitope tag](../../../../../epitope-tag.md). Lyse under conditions chosen to preserve the relevant [protein complex](../../../../../protein-complex.md), capture the bait on an affinity matrix, wash away background and identify co-purifying [proteins](../../../../../protein-split.md) by [liquid chromatography-mass spectrometry](../../../../../liquid-chromatography-mass-spectrometry.md) after digestion into [peptides](../../../../../peptide.md). [Co-immunoprecipitation](../../../../../co-immunoprecipitation.md) is the antibody-based version of this association test. Gentle conditions preserve more weak interactions but also increase background; stringent washing improves specificity at the cost of labile partners. Extraction can disrupt membrane assemblies or create associations that were not present in intact cells.

Controls should include matched tag-only or untagged cells, an appropriate antibody control, input abundance and, where feasible, a binding-defective bait that retains its normal localization. Check that tagging has not changed the bait's abundance, localization or function. Reciprocal capture of a candidate partner is useful validation. If an association might be bridged by [RNA](../../../../../ribonucleic-acid.md) or [DNA](../../../../../deoxyribonucleic-acid.md), compare nuclease-treated and untreated samples while recognizing that nuclease treatment may dismantle a biologically genuine assembly.

For [proximity labeling](../../../../../proximity-labeling.md), fuse the bait to [TurboID](../../../../../turboid.md), which activates [biotin](../../../../../biotin.md) and covalently labels accessible nearby [proteins](../../../../../protein-split.md) in living cells. After a timed labeling pulse, harsh lysis can be used because recovery no longer requires the original assembly to survive. Capture biotinylated material using [streptavidin](../../../../../streptavidin.md) and identify enriched [proteins](../../../../../protein-split.md) by [mass spectrometry](../../../../../mass-spectrometry.md). This can recover transient or insoluble neighbourhoods missed by ordinary extraction. A localization-matched control enzyme, no-added-biotin condition and matched expression help separate the bait's neighbourhood from diffuse labeling and endogenous biotinylated proteins.[Figs. 1–3, enzyme activity, labeling time and compartment-specific comparisons](../../../../../efficient-proximity-labeling-in-living-cells-and-organisms-with-turboid-by-tess-c-branon-and-others.md)

The label records proximity, accessibility and time spent nearby. A neighbour need not bind the bait; a real binder might label poorly if reactive groups are inaccessible. Pulse duration therefore trades temporal selectivity against labeling yield, rather than defining an exact universal distance cutoff.

**Quantification distinguishes enrichment from a list of contaminants.** Use [label-free quantification](../../../../../label-free-quantification.md) of [peptide](../../../../../peptide.md) signals across independent bait and control purifications, or [SILAC](../../../../../stable-isotope-labeling-by-amino-acids-in-cell-culture.md) in compatible cell cultures to compare light and heavy samples. In [SILAC](../../../../../stable-isotope-labeling-by-amino-acids-in-cell-culture.md), isotope-containing amino acids enter newly synthesized [proteins](../../../../../protein-split.md); matched peptides form distinguishable mass pairs. A label swap helps identify isotope-condition confounding. [Tandem mass tags](../../../../../tandem-mass-tag.md) offer multiplexed comparison using reporter signals, but interfering co-isolated peptides can compress ratios.

Estimate enrichment and its reproducibility relative to matched controls, accounting for bait recovery and input abundance. Common abundant contaminants should not be promoted solely because many spectra identify them. Statistical scoring such as SAINT models the contrast between specific and background recovery across controls and replicates, allowing candidate associations to be ranked with estimated error rates.[Statistical model, control purifications and interaction-probability estimation](../../../../../saint-probabilistic-scoring-of-affinity-purification-mass-spectrometry-data-by-hyungwon-choi-and-others.md) **A reproducibly enriched candidate is evidence for the assay-defined association or neighbourhood, not automatically a direct binding partner or fixed stoichiometric subunit.**

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
