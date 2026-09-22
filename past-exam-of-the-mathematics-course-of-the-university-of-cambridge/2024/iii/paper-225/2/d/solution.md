<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The squared-norm test is omnibus: every fixed nonzero mean eventually changes $\lVert\overline X_n\rVert$. Its null law, however, is an infinite weighted chi-squared distribution and requires accurate estimation of enough covariance eigenvalues; noisy low-variance directions can also make calibration inefficient.

The [FPCA mean test](../../../../../../fpca-mean-test.md) has the simple $\chi_K^2$ limit and standardizes retained directions by their variances. It is effective when the signal lies in the leading principal component subspace, but choosing $K$ introduces a tuning decision and truncation makes the test blind to alternatives orthogonal to that subspace. Close or repeated eigenvalues also make individual empirical eigenfunctions unstable.

The [sign-flip randomization test](../../../../../../sign-flip-randomization-test.md) can provide finite-sample calibration and avoids estimating a limiting covariance spectrum. Its exactness requires central symmetry, which is stronger than merely having zero mean, and exhaustive enumeration costs $2^n$ evaluations; Monte Carlo sign flips introduce simulation error. Its power still depends on the statistic used inside the randomization scheme.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
