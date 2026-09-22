<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand an initial bipartite [pure state](../../../../../../pure-state.md) in local [orthonormal bases](../../../../../../orthonormal-basis.md) as

$$
|\psi\rangle=\sum_{i,j}C_{ij}|i\rangle_A|j\rangle_B.
$$

By the [Schmidt decomposition](../../../../../../schmidt-decomposition.md), or equivalently the [singular value decomposition](../../../../../../singular-value-decomposition.md) of $C$, its [Schmidt rank](../../../../../../schmidt-rank.md) is $\operatorname{rank}C$. In a specified local measurement branch, the product [Kraus operator](../../../../../../kraus-operator.md) $A\otimes B$ changes the coefficient [matrix](../../../../../../matrix.md) to

$$
C'=ACB^{\mathsf T}.
$$

Indeed the coefficient of $|k\rangle|l\rangle$ is $\sum_{i,j}A_{ki}C_{ij}B_{lj}$. The elementary [matrix rank](../../../../../../matrix-rank.md) inequality gives

$$
\operatorname{rank}(ACB^{\mathsf T})\leq\operatorname{rank}C.
$$

Normalizing a nonzero branch multiplies $C'$ by a scalar and therefore leaves its [matrix rank](../../../../../../matrix-rank.md) unchanged.

Now refine a complete [LOCC](../../../../../../local-operations-and-classical-communication.md) transcript to record every individual [Kraus operator](../../../../../../kraus-operator.md). Although later choices depend on the earlier classical outcomes, fixing a transcript fixes all those choices. Composing the local operations therefore gives a single product [Kraus operator](../../../../../../kraus-operator.md) $A_\tau\otimes B_\tau$ in that branch. Each nonzero branch obeys the same [Schmidt-rank contraction under product operators](../../../../../../schmidt-rank-contraction-under-product-operators.md). Local auxiliary systems prepared independently are included by local isometries and do not add [entanglement](../../../../../../entangled-state.md). Discarding a local auxiliary system is included by resolving its [partial trace](../../../../../../partial-trace.md) in an [orthonormal basis](../../../../../../orthonormal-basis.md); this again yields refined product [Kraus operators](../../../../../../kraus-operator.md).

If the protocol produces a specified [pure state](../../../../../../pure-state.md) deterministically, its output [density operator](../../../../../../density-matrix.md) is a sum of positive rank-one branch [density operators](../../../../../../density-matrix.md). Every nonzero branch vector must be proportional to that output vector: its squared overlap with any vector orthogonal to the output sums to zero, so each such overlap is separately zero. Thus the output [Schmidt rank](../../../../../../schmidt-rank.md) equals that of each surviving branch, and

$$
\boxed{r_{\mathrm{out}}\leq r_{\mathrm{in}}.}
$$

This proves [monotonicity of Schmidt rank under LOCC](../../../../../../monotonicity-of-schmidt-rank-under-locc.md), even for a nonzero branch selected by [postselection](../../../../../../postselection.md). If the classical transcript is instead discarded and the result is mixed, the refined branch vectors supply an ensemble with [Schmidt ranks](../../../../../../schmidt-rank.md) at most $r_{\mathrm{in}}$; by definition its [Schmidt number](../../../../../../schmidt-number.md) is at most $r_{\mathrm{in}}$. This is the correct mixed-state extension, rather than a bound on the ranks of its [reduced density matrices](../../../../../../reduced-density-matrix.md). In finite dimensions, any limiting exact protocol obeys the same pure-state bound because the set of coefficient [matrices](../../../../../../matrix.md) of rank at most $r_{\mathrm{in}}$ is closed, being defined by vanishing minors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
