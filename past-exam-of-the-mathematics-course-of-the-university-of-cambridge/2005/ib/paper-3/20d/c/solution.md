<h1 id="20d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The dual constraints and objective coefficients on $x$ are unchanged, so $y^*$ remains dual feasible. Since every component of $y^*$ is positive, complementary slackness forces every constraint of any primal optimum paired with it to bind. Let $A$ be the original three-by-three constraint matrix and $b'=b+\epsilon$. It is invertible, and the only possible paired primal point is

$$
x'=A^{-1}b'=\begin{pmatrix}7+(2\epsilon_1+4\epsilon_2+5\epsilon_3)/33\\22-\epsilon_1/3+\epsilon_2+\epsilon_3/3\\1+(-4\epsilon_1+3\epsilon_2+\epsilon_3)/33\end{pmatrix}.
$$

If this point is nonnegative, it is primal feasible with zero slacks and $c^Tx'=y^{*T}b'$, proving $y^*$ optimal. Conversely, if $y^*$ is optimal, [linear programming duality](../../../../../../linear-programming-duality.md) supplies a paired primal optimum, and complementary slackness forces it to be exactly this point. This proves the [strictly positive dual certificate and right-hand-side sensitivity](../../../../../../strictly-positive-dual-certificate-and-right-hand-side-sensitivity.md) criterion:

$$
\boxed{\begin{aligned}2\epsilon_1+4\epsilon_2+5\epsilon_3&\geq-231,\\-\epsilon_1+3\epsilon_2+\epsilon_3&\geq-66,\\-4\epsilon_1+3\epsilon_2+\epsilon_3&\geq-33.\end{aligned}}
$$

Non-strict inequalities are essential: boundary cases can be degenerate but retain the same optimal dual vector. This is the complete range, not just a small-perturbation sufficient condition for [linear programming sensitivity within a fixed optimal basis](../../../../../../linear-programming-sensitivity-within-a-fixed-optimal-basis.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20D](../../20d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
