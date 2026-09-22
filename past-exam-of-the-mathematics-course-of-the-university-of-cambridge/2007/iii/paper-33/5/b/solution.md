<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Path continuity makes each time-segment range compact and therefore Borel measurable. The membership event is jointly measurable in the sample and spatial variable: distance to the range equals the infimum of $|B_t-y|$ over a countable dense set of times. We may consequently apply the [Tonelli theorem](../../../../../../tonelli-theorem.md) to its indicator.

Put $m=\mathbb E\lambda(R)<\infty$, using the allowed integrability hypothesis. Since $R=A_1\cup A_2$, finite-measure inclusion-exclusion and the preceding [expectation](../../../../../../expected-value.md) identities give

$$
\mathbb E\lambda(A_1\cap A_2)=\mathbb E\lambda(A_1)+\mathbb E\lambda(A_2)-\mathbb E\lambda(R)=m/2+m/2-m=0.
$$

Finally [Tonelli theorem](../../../../../../tonelli-theorem.md) gives

$$
\boxed{\int_{\mathbb R^2}\mathbb P(y\in A_1\cap A_2)\,dy=\mathbb E\lambda(A_1\cap A_2)=0.}
$$

Finiteness of $m$ is what justifies the subtraction of [expectations](../../../../../../expected-value.md); an infinite-minus-infinite calculation would not establish this conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
