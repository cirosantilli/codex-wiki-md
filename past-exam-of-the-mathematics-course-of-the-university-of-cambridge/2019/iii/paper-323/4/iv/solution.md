<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose the [trace-distance-preserving binary measurement](../../../../../../trace-distance-preserving-binary-measurement.md) from the previous part. Let $p,q$ be its output probability distributions, so $\lVert p-q\rVert_1=2D(\rho,\sigma)$. The [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) gives

$$
D(\rho\|\sigma)\geq D(\Phi(\rho)\|\Phi(\sigma))=D(p\|q).
$$

For diagonal [density operators](../../../../../../density-matrix.md), the quantum expression is the classical [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md). Applying the supplied [Pinsker's inequality](../../../../../../pinsker-s-inequality.md) gives

$$
D(p\|q)\geq\frac1{2\ln2}\lVert p-q\rVert_1^2
=\frac2{\ln2}D(\rho,\sigma)^2.
$$

Consequently the [quantum Pinsker inequality](../../../../../../quantum-pinsker-inequality.md) is

$$
\boxed{D(\rho\|\sigma)\geq\frac2{\ln2}D(\rho,\sigma)^2}.
$$

The $\ln2$ factor converts natural-logarithm relative entropy to bits. If the relative entropy is infinite because its support condition fails, the inequality holds automatically.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
