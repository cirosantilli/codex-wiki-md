<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The central principle is to **attach a recoverable spatial address to an RNA-derived molecule before the tissue's positional organization is destroyed**. After sequencing, each read identifies both a transcript and a capture location.

In the original array-based [spatial transcriptomics](../../../../../spatial-transcriptomics.md) method, a thin tissue section is placed on a slide carrying spatially indexed capture primers. The tissue is imaged for [histology](../../../../../histology.md), then permeabilized. Polyadenylated [messenger RNA](../../../../../messenger-rna.md) binds the oligo(dT) region of the primers and is copied by [reverse transcription](../../../../../reverse-transcription.md). The resulting [cDNA](../../../../../complementary-dna.md) carries the positional barcode. Sequencing identifies the expressed [gene](../../../../../gene.md), and a barcode lookup places its counts back on the tissue image. The first published array used approximately $100\,\mu\mathrm m$ capture features, so a feature could contain contributions from several cells; it was not a single-cell measurement by construction.[pp. 78–80, spatially localized cDNA synthesis, positional barcodes and array features](../../../../../visualization-and-analysis-of-gene-expression-in-tissue-sections-by-spatial-transcriptomics-by-patrik-l-stahl-and-others.md)

[Slide-seq](../../../../../slide-seq.md) applies the same addressing idea using a dense monolayer of roughly $10\,\mu\mathrm m$ barcoded beads. The bead barcode–position map is decoded in advance. A tissue section is transferred onto the beads, released [RNA](../../../../../ribonucleic-acid.md) is captured, and the sequenced molecular addresses recover the bead-level expression map. This gives much finer spatial sampling than the original coarse array, although RNA capture efficiency and assignment to individual cells remain limiting.[pp. 1463–1465, bead puck construction, positional decoding and RNA capture](../../../../../slide-seq-a-scalable-technology-for-measuring-genome-wide-expression-at-high-spatial-resolution-by-samuel-g-rodriques-and-others.md)

Some assays also incorporate a [unique molecular identifier](../../../../../unique-molecular-identifier.md) so that amplified reads from one captured molecule can be collapsed, reducing [polymerase chain reaction](../../../../../polymerase-chain-reaction.md) duplication bias. Spatial barcodes identify capture locations; [unique molecular identifiers](../../../../../unique-molecular-identifier.md) identify molecules within those locations. Neither alone supplies cell boundaries.

For either method, align the coordinate map with [histology](../../../../../histology.md), account for capture efficiency and background, and use independent tissue specimens as [biological replicates](../../../../../biological-replicate.md). A smaller capture feature improves sampling granularity but does not guarantee equal effective [spatial resolution](../../../../../spatial-resolution.md) or a pure single-cell transcriptome: tissue thickness, diffusion and mixed cell boundaries still matter.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
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
