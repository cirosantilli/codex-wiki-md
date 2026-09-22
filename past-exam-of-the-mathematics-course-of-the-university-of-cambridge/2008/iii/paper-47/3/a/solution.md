<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A good [pseudorandom number generator](../../../../../../pseudorandom-number-generator.md) for [Monte Carlo integration](../../../../../../monte-carlo-integration.md) should have approximately uniform outputs, a period much longer than the intended run, and negligible detectable dependence both serially and in higher-dimensional tuples. It should be fast, reproducible from a seed, portable enough to reproduce a calculation, and numerically precise enough for the required tail probabilities. Values strictly inside $(0,1)$ avoid singularities in logarithmic [inverse transform sampling](../../../../../../inverse-transform-sampling.md). Separate simulations also need well-separated streams or seeds, rather than accidentally identical streams. A [pseudorandom number generator](../../../../../../pseudorandom-number-generator.md) is deterministic; these properties mean that it imitates independent [uniform distributions](../../../../../../continuous-uniform-distribution.md) sufficiently well for the application, not that its outputs are literally independent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
