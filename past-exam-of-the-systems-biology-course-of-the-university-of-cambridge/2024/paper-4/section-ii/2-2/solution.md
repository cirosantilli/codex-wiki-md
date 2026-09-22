<h1 id="section-ii/2-2/solution">Solution</h1>

↑ **Parent:** [2.2](../2-2.md)

**Objective and rationale.** Build an evidence-traceable [genome](../../../../../genome.md) resource for the organism described in the question, then improve its [gene](../../../../../gene.md) structures using one genome-wide experiment: replicated, strand-aware [RNA sequencing](../../../../../rna-sequencing.md) across a deliberately chosen range of growth conditions. The species name is treated as part of the hypothetical study; no established [gene](../../../../../gene.md) catalogue is assumed.

Poor annotation limits both discovery and interpretation. Missing exons distort [protein sequences](../../../../../protein-sequence.md), merged or split [gene models](../../../../../gene-model.md) create false absences and duplications, and unrecognized transcripts bias expression analyses. Functional claims transferred to an incorrectly predicted [protein](../../../../../protein-split.md) can then compound the original error. Reliable coordinates, [gene](../../../../../gene.md) identifiers and evidence provenance are therefore prerequisites for a comparative model system.

**Resource construction.** Assemble a versioned reference containing the [genome assembly](../../../../../genome-assembly.md), existing [gene models](../../../../../gene-model.md), published sequence evidence and curated cross-references. Reconcile naming and coordinates, flag conflicting [gene](../../../../../gene.md) structures, and document assembly gaps and repetitive regions. Compare predicted [proteins](../../../../../protein-split.md) with well-annotated yeast homologues using [orthology](../../../../../orthology.md), conserved domain architecture and, where informative, conserved [gene](../../../../../gene.md) neighbourhoods. Sequence similarity is evidence for a relationship; it is not sufficient to give every paralogue its best hit's exact function.

**Genome-wide experiment.** Use [RNA sequencing](../../../../../rna-sequencing.md) to supply transcript evidence from independent biological samples covering contrasting physiological states. Multiple conditions broaden the chance of observing condition-specific [genes](../../../../../gene.md), but read counts within a library remain technical observations, not extra [biological replicates](../../../../../biological-replicate.md). Quality-control and strand-aware alignment would assess mapping uniqueness, exon coverage and [splice junction](../../../../../splice-junction.md) support. Reference-guided and appropriately checked [transcript assembly](../../../../../transcript-assembly.md) can identify expressed loci absent from the current annotation and suggest corrected exon boundaries, alternative transcripts and untranslated regions.

Integrate these data with [protein](../../../../../protein-split.md) homology and gene-prediction evidence. A proposed exon should have coherent splice support and coding plausibility; an isolated ambiguous read is insufficient. Keep alternative models and confidence levels when repeat structure or incomplete coverage prevents a unique assignment. No expression in the sampled conditions should be recorded as lack of evidence, not proof that a [gene](../../../../../gene.md) is absent.

**Validation and functional annotation.** Validate a representative set of corrected and new models by targeted transcript and junction checks, prioritizing models whose revision changes a predicted [protein domain](../../../../../protein-domain.md) or conserved function. Retain known positive controls and distinguish biological alternatives from assembly or mapping errors. Transfer broad functional terms conservatively using [orthology](../../../../../orthology.md) and domain evidence, with explicit evidence codes and source organisms; a computationally inferred function remains distinct from an experimental demonstration.

[RNA sequencing](../../../../../rna-sequencing.md) improves expressed [gene](../../../../../gene.md) structures and condition-specific expression annotation, but it does not repair every assembly gap, establish translation of every transcript, or identify every [gene](../../../../../gene.md)'s biochemical activity. Those limitations should remain visible in the resource. The deliverables are a searchable [genome browser](../../../../../genome-browser.md), stable identifiers, versioned [gene models](../../../../../gene-model.md) and downloadable evidence tracks, together with a reproducible update process that preserves previous releases and community corrections.

## ↑ Ancestors (13)

1. [2.2](../2-2.md)
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
