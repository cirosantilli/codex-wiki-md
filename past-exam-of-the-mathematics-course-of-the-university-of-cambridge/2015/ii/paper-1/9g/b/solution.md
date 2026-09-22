<h1 id="9g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Hamming code](../../../../../../hamming-code.md) decoder succeeds on a seven-bit block exactly when there are zero or one errors. Its radius-one decoding regions are disjoint, so an error of weight at least two cannot decode back to the original codeword. Thus

$$
q=(1-p)^7+7p(1-p)^6=1-21p^2+O(p^3),\qquad
\boxed{Q=q^N\simeq(1-21p^2)^N\simeq e^{-21Np^2}}.
$$

Numerically $Q\approx0.97929$, so only about $1.0212$ transmissions are expected. Even accounting for seven rather than four bits per letter, expected bits sent are $7N/Q\approx7148$, compared with $4N/P\approx218830$. **The Hamming method is substantially better** under the stated error detection and independent retransmission assumptions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9G](../../9g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
