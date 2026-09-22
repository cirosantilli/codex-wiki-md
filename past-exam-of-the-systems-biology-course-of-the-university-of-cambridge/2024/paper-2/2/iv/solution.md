<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The distinction is principally **molecular readout by sequencing versus molecular readout by imaging**; it does not impose one universal ranking of sensitivity or spatial resolution.

| Issue | Sequencing-based [spatial transcriptomics](../../../../../spatial-transcriptomics.md) | Imaging-based [spatial transcriptomics](../../../../../spatial-transcriptomics.md) |
| --- | --- | --- |
| Target breadth | Many capture assays survey broad polyadenylated [RNA](../../../../../ribonucleic-acid.md) without a fixed gene panel. | Probe-based assays usually require a designed target set, though [seqFISH+](../../../../../seqfish-plus.md) and [MERFISH](../../../../../multiplexed-error-robust-fluorescence-in-situ-hybridization.md) can be highly multiplexed. |
| Spatial information | Positions are capture features or beads; some collect mixtures of cells. | Individual molecular coordinates and subcellular distributions can be retained. |
| Sensitivity and bias | Capture, [reverse transcription](../../../../../reverse-transcription.md) and library sampling lose molecules; amplification and diffusion add bias. | Probe accessibility, optical crowding, [autofluorescence](../../../../../autofluorescence.md) and decoding errors determine detection. |
| Resources | Requires sequencing capacity and barcode-aware analysis. | Requires extensive imaging, repeated fluidics, registration and image storage. |
| Cell assignment | Mixed features may need statistical estimation using reference cell profiles. | Usually needs explicit [cell segmentation](../../../../../cell-segmentation.md), which can misassign otherwise well-localized molecules. |

For discovery of unexpected [gene expression](../../../../../gene-expression.md) programmes across a large section, broad sequencing-based capture is attractive. To test where selected transcripts lie within cells or precisely map a known anatomical niche, molecular imaging is attractive. Neither implies that every transcript is measured, and a nominal spot size should not be confused with biological assignment accuracy.

A productive study can combine broad discovery with targeted spatial validation on independent sections. Compare effective detection, tissue area, resolution, cost and replicate count for the specific implementations available, rather than treating all sequencing assays as coarse and all imaging assays as low-plex. Cells or capture spots from one donor are not substitutes for independent [biological replicates](../../../../../biological-replicate.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
