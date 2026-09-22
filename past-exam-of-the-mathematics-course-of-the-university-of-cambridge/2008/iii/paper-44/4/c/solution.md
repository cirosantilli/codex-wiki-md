<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The priors are proper but difficult to justify as practically weak information. Uniform bounds $[-100,100]$ on log asymptotes cover fantastically small and large circumferences. The independent prior on the transformed location makes the centered fraction spend much of its mass near zero or one, while the slope prior permits decreasing growth. Independence also ignores likely relationships among curve parameters.

The $\operatorname{Gamma}(0.001,0.001)$ prior on error precision is proper, but its near-zero shape creates a highly skewed prior with consequential mass near very small precision. It is not automatically harmless. Use biologically scaled priors for asymptotes and timing, a positive growth-rate prior, and a defensible prior on the error standard deviation such as a suitably scaled [half-normal distribution](../../../../../../half-normal-distribution.md). Check simulated trajectories with [prior predictive checks](../../../../../../prior-predictive-check.md) and assess prior sensitivity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
