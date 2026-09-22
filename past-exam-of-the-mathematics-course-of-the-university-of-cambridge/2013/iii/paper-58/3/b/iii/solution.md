<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Maintain a known list of the still-active indices, initially all $N=2K$ positions. On a list of even size $M$, perform the three-step construction with $M$ replacing $N$. A known reversible relabeling prepares and queries the corresponding original indices, so [quantum phase kickback](../../../../../../../phase-kickback.md) still needs only one call to $O_{\mathbf x}$. The full [unitary extension](../../../../../../../unitary-extension-of-a-finite-dimensional-isometry.md) for that current size is independent of the remaining unknown values. It is allowed even when $M$ is not a power of two.

If the measurement gives $(0,0)$, its amplitude is the imbalance divided by $M$. A balanced active string has zero such amplitude, so an observed zero pair certifies that the active string is unbalanced. Return unbalanced immediately. No probability-of-error estimate is needed: an impossible outcome never occurs in the balanced case.

Otherwise the measured pair corresponds to two opposite bits. Delete those two indices and repeat. Each deletion removes exactly one zero and one one, preserving the difference between their counts. Thus the active string is balanced if and only if the original one is balanced. If all indices are removed, return balanced. This is [opposite-pair elimination for exact quantum balance testing](../../../../../../../opposite-pair-elimination-for-exact-quantum-balance-testing.md); it never requires determining which member of a deleted pair is zero.

Each query either terminates with a valid imbalance certificate or reduces the active length by two. After at most $K$ opposite-pair outcomes the active list is empty. **The result is certain on every input, with worst-case query count**

$$
\boxed{Q(N)\le N/2=K.}
$$

The same argument includes the $M=2$ last step: equal bits give $(0,0)$ with certainty, while opposite bits give the sole nonzero pair with certainty. There is no additional final query. The measurement probabilities are normalized because $(M-2w)^2+4w(M-w)=M^2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
