<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [nonlinear compact operator](../../../../nonlinear-compact-operator.md) is a continuous map that sends [bounded sets](../../../../bounded-set.md) of its domain to [relatively compact subsets](../../../../relatively-compact-subset.md) of the target space; linearity is not part of this general definition.

For the specified [diagonal operator on sequence space](../../../../diagonal-operator-on-sequence-space.md) on [l2 sequence space](../../../../l2-sequence-space.md),

$$
\|Tx\|_2^2=\sum_{i\geq1}\frac{|x_i|^2}{i^2}\leq\sum_{i\geq1}|x_i|^2,
$$

so it is well-defined, [linear](../../../../linearity.md) and [bounded](../../../../boundedness.md). Let $T_N$ retain only its first $N$ output coordinates. This is a [finite-rank operator](../../../../finite-rank-operator.md), and

$$
\boxed{\|T-T_N\|=\frac1{N+1}\longrightarrow0.}
$$

The upper bound follows by estimating each tail multiplier by $1/(N+1)$; equality follows on the unit coordinate vector $e_{N+1}$. Finite-rank operators between [Banach spaces](../../../../banach-space-split.md) are compact, and a limit of compact linear operators in [operator norm](../../../../operator-norm.md) is compact, the [norm-closedness of compact operators](../../../../norm-closedness-of-compact-operators.md). Therefore $\boxed{T\text{ is compact}}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
