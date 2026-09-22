<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Browder convergence theorem for averaged operators](../../../../../../browder-convergence-theorem-for-averaged-operators.md) states: if $T:\mathbb R^d\to\mathbb R^d$ is an [averaged operator](../../../../../../averaged-operator.md) and its fixed-point set $\operatorname{Fix}T=\{z:Tz=z\}$ is nonempty, then **for every starting point, $z^{k+1}=Tz^k$ converges in norm to a [fixed point](../../../../../../fixed-point.md) of $T$**. The theorem assumes a [fixed point](../../../../../../fixed-point.md) exists; averaging by itself does not create one.

The finite-dimensional mechanism is worth making explicit. For any [fixed point](../../../../../../fixed-point.md) $p$, the [averaged-operator inequality](../../../../../../averaged-operator-inequality.md) gives

$$
\|z^{k+1}-p\|_2^2\leq\|z^k-p\|_2^2-\frac{1-\alpha}{\alpha}\|z^{k+1}-z^k\|_2^2.
$$

This is [Fejér monotonicity](../../../../../../fejer-monotonicity.md) with respect to the fixed-point set. It makes the sequence bounded and, by summation, makes $\sum_k\|z^{k+1}-z^k\|_2^2$ finite. Hence its residual tends to zero. Choose a convergent subsequence $z^{k_j}\to\bar z$; continuity of the [nonexpansive mapping](../../../../../../nonexpansive-mapping.md) $T$ implies $T\bar z=\bar z$. Apply [Fejér monotonicity](../../../../../../fejer-monotonicity.md) with $p=\bar z$. The nonincreasing distances $\|z^k-\bar z\|_2$ have a subsequence tending to zero, so the whole sequence converges to $\bar z$. This last compactness step uses finite dimension; a corresponding general [Hilbert space](../../../../../../hilbert-space-split.md) statement usually gives weak convergence.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
