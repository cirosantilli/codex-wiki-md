<h1 id="1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Prepare the auxiliary system in the [maximally mixed state](../../../../../../maximally-mixed-state.md) $\rho=I/N$. Then $\operatorname{Tr}(\rho U)=\operatorname{Tr}U/N$, so the two measurement bases give

$$
\boxed{\widehat{\operatorname{Tr}U}=N\bigl[(\widehat P_0-\widehat P_1)+i(\widehat P_--\widehat P_+)\bigr].}
$$

There is no need to know the [eigenvectors](../../../../../../eigenvector.md) of $U$. Choose a uniformly random member of any known orthonormal basis on each run; discarding the classical preparation label produces $I/N$. Alternatively, discard one half of a maximally entangled pair of $N$-level systems. This is [trace estimation by a maximally mixed Hadamard test](../../../../../../trace-estimation-by-a-maximally-mixed-hadamard-test.md).

The circuit directly estimates the normalized [trace](../../../../../../matrix-trace.md). To demand fixed absolute accuracy $\varepsilon$ in the unnormalized [trace](../../../../../../matrix-trace.md) requires normalized accuracy $\varepsilon/N$; straightforward independent frequency sampling consequently uses order $N^2/\varepsilon^2$ runs at fixed confidence. Thus the construction should not be confused with a dimension-independent guarantee for arbitrary absolute trace precision.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
