<h1 id="section-ii/2-3/solution">Solution</h1>

↑ **Parent:** [2.3](../2-3.md)

**Model and central question.** Use [Saccharomyces cerevisiae](../../../../../saccharomyces-cerevisiae.md) as a tractable eukaryotic system with a well-annotated [genome](../../../../../genome.md) and established [DNA repair](../../../../../dna-repair.md) and checkpoint biology. The aim is to identify the UV-responsive transcriptional programme and separate direct regulation from secondary changes caused by cell-cycle arrest, altered growth or loss of viability. The resulting network is a yeast model; conservation in other eukaryotes remains a hypothesis to test.

**Discovery design.** Compare UV-exposed and mock-handled cultures at baseline and several recovery stages, using independent [biological replicates](../../../../../biological-replicate.md) and balanced processing. Include matched handling controls and record growth, viability and [cell cycle](../../../../../cell-cycle-split.md) state. Choose conditions yielding an interpretable damage response rather than treating terminally damaged cells as a normal regulatory trajectory. Biological replication and [randomization](../../../../../randomization.md) must occur at the culture level, not merely by sequencing the same material repeatedly.

Measure transcript abundance using [RNA sequencing](../../../../../rna-sequencing.md) and assess sample quality before testing differences. Model condition, time, their interaction and recorded batch factors, using an appropriate count-based expression model. Report [effect sizes](../../../../../effect-size.md), uncertainty and [false discovery rate](../../../../../false-discovery-rate.md), not only a list passing a significance cutoff. Where changes in total [RNA](../../../../../ribonucleic-acid.md) per cell could invalidate relative normalization, include a suitable external reference strategy and distinguish relative composition from absolute expression.

**Candidate regulators and direct targets.** Cluster well-supported expression trajectories to nominate coordinated modules, then ask whether their promoters are enriched for known transcription-factor motifs. Combine motif evidence with regulator expression, localization or activity measurements and prior knowledge. Motif occurrence and coexpression alone are insufficient to establish a direct regulatory edge: a factor can be activated without changing its own transcript abundance, and many coexpressed [genes](../../../../../gene.md) share an upstream cause.

For prioritized factors, compare chromatin association before and after damage using [chromatin immunoprecipitation](../../../../../chromatin-immunoprecipitation.md) with genome-wide readout and appropriate input and specificity controls. Binding near a [gene](../../../../../gene.md) is additional evidence, not proof that the binding event regulates it. A targeted regulator perturbation and rescue comparison should test the predicted expression response while monitoring viability and checkpoint effects. Reporter or promoter-element comparisons can further test a specific cis-regulatory mechanism without assuming that every enriched motif is functional.

**Temporal and causal integration.** Use timing, perturbation effects and occupancy jointly. A plausible direct target changes after regulator activation, shows relevant occupancy evidence and responds to a selective perturbation. Secondary effects may appear later or depend on cell-cycle redistribution. Where transcript abundance cannot separate synthesis from [RNA](../../../../../ribonucleic-acid.md) stability, a focused measurement of newly synthesized [RNA](../../../../../ribonucleic-acid.md) can test the proposed transcriptional component.

Build a [gene regulatory network](../../../../../gene-regulatory-network.md) whose edges retain sign, condition, confidence and evidence type. Predict responses to a held-out perturbation or recovery condition, and assess those predictions using new biological samples. Release the design, metadata, code and qualified edge list. Success is a validated account of important regulatory modules and their limits, rather than an unsupported claim to have measured every possible interaction in the eukaryotic damage response.

## ↑ Ancestors (13)

1. [2.3](../2-3.md)
2. [Section II](../../section-ii.md)
3. [Paper 4](../../../paper-4-split.md)
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
