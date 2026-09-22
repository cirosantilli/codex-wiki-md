<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Imaging methods **identify RNA molecules where they remain in the fixed specimen**, rather than recovering their position through a sequencing-library address. Their common foundation is sequence-specific [oligonucleotide probe](../../../../../oligonucleotide-probe.md) binding and repeated [fluorescence microscopy](../../../../../fluorescence-microscopy.md).

In [single-molecule fluorescence in situ hybridization](../../../../../single-molecule-fluorescence-in-situ-hybridization.md), many short complementary probes bind one transcript. Their combined [fluorescence](../../../../../fluorescence-split.md) produces a detectable spot that can be localized and counted. Multiple probes make an individual bound molecule distinguishable from isolated-probe background. Conventional colour channels limit how many transcript species can be distinguished in one image, and overlapping spots make abundant targets difficult to count.

**[MERFISH](../../../../../multiplexed-error-robust-fluorescence-in-situ-hybridization.md).** Encoding probes bind each target [RNA](../../../../../ribonucleic-acid.md) and expose selected readout sequences. Across successive hybridization and imaging rounds, fluorescent readout probes interrogate those sequences, producing an on/off code at each molecular position. The code identifies the transcript. The codebook is designed with separation between valid words so that some missing or spurious signals can be detected and, for suitable codes, corrected. Fiducials and image registration keep the same molecule aligned across rounds. This multiplexes many targets without needing one physically separate fluorescence colour for each [gene](../../../../../gene.md).[Results, encoding scheme and error-robust barcodes; Figs. 1–3](../../../../../spatially-resolved-highly-multiplexed-rna-profiling-in-single-cells-by-kok-hao-chen-and-others.md)

**[seqFISH](../../../../../sequential-fluorescence-in-situ-hybridization.md) and [seqFISH+](../../../../../seqfish-plus.md).** Successive probe hybridization rounds encode a transcript through a sequence of detected colours. The expanded [seqFISH+](../../../../../seqfish-plus.md) strategy distributes targets among many pseudocolour states, so each round contains only a sparse subset of the total signals. This reduces optical crowding and makes a much larger target set readable on an ordinary [confocal microscope](../../../../../confocal-microscope.md). The original [seqFISH+](../../../../../seqfish-plus.md) study profiled about 10,000 genes in mouse brain tissue and examined both cellular organization and subcellular expression patterns.[Abstract; Figs. 1–4, pseudocolours, optical crowding and tissue organization](../../../../../transcriptome-scale-super-resolved-imaging-in-tissues-by-rna-seqfish-plus-by-chee-huat-linus-eng-and-others.md)

These are two distinct multiplexing implementations, although both build on repeated in situ probe readout. Their performance depends on probe specificity, the codebook, stripping or inactivation of previous signals, retention of [RNA](../../../../../ribonucleic-acid.md), registration across rounds and the density of simultaneously visible spots. Imaging many rounds can be slow, and tissue [autofluorescence](../../../../../autofluorescence.md) or poor probe penetration can obscure molecules.

Finally, use nuclear and membrane information for [cell segmentation](../../../../../cell-segmentation.md), with checks for errors at touching cells and tissue boundaries. A precise molecular coordinate does not guarantee correct cell assignment. Negative or unused codes and independent probes help estimate false calls; [biological replicates](../../../../../biological-replicate.md) establish whether a spatial pattern is reproducible.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
