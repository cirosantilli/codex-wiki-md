<h1 id="25j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in the real $L^1$ space, consistent with the specified real step coefficients. First approximate an integrable function by a finite-valued measurable function with bounded support. Truncate its domain to $[-M,M]$ and its values to $[-M,M]$; the $L^1$ error tends to zero by integrability. Quantize those remaining values in intervals of mesh $\delta$, producing a simple function $u=\sum_{j=1}^mc_j\mathbf1_{B_j}$ with finite-measure Borel sets $B_j$ and error at most $2M\delta$ on the truncated domain. Thus $\|f-u\|_1$ can be made arbitrarily small.

For each $B_j$, use the allowed approximation by a finite union of intervals $A_j$, choosing the symmetric-difference errors so

$$
\sum_j|c_j|\mu(A_j\mathbin\triangle B_j)<\varepsilon.
$$

These unions can be written as finite disjoint bounded intervals, and changing endpoints to the required half-open convention changes only a null set. The function $s=\sum_jc_j\mathbf1_{A_j}$ is therefore a [step function](../../../../../../step-function.md) of the specified form, and

$$
\|u-s\|_1\leq\sum_j|c_j|\mu(A_j\mathbin\triangle B_j)<\varepsilon.
$$

Combining the two approximations proves **the step functions are dense in $L^1(\mathbb R)$**. In the complex version of $L^1$, the same argument applies to real and imaginary parts when complex step coefficients are allowed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [25J](../../25j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
