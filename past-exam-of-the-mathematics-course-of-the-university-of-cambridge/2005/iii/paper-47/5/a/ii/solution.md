<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Single-component updates propose one coordinate while holding the others fixed, with acceptance based on the resulting target ratio. They are cheap and permit individual scale tuning, but can crawl along a narrow correlated ridge. Block updates propose several coordinates jointly and can follow [posterior](../../../../../../../bayesian-posterior.md) [covariance](../../../../../../../covariance.md) directions, potentially improving mixing substantially.

A practical compromise uses small correlated blocks, or a full [Gaussian](../../../../../../../normal-distribution.md) block with [covariance](../../../../../../../covariance.md) estimated in a pilot run and rescaled for acceptance. Blocking [independent](../../../../../../../independent-random-variables.md) coordinates need not help, and a badly scaled high-dimensional block may be rejected frequently. Compare computing cost per effective draw, rather than acceptance rate alone. A [Metropolis-within-Gibbs](../../../../../../../metropolis-within-gibbs-algorithm.md) sweep of coordinate updates and a properly accepted block update both preserve the target.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
