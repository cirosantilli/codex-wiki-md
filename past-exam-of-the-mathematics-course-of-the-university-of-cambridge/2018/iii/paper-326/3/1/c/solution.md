<h1 id="3/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $0<\alpha<\beta$, abbreviate $D_\alpha=D(u_\alpha)$ and $J_\alpha=J(u_\alpha)$. Optimality of the two [variational regularization](../../../../../../../variational-regularization.md) solutions gives

$$
D_\alpha+\alpha J_\alpha\leq D_\beta+\alpha J_\beta,\qquad
D_\beta+\beta J_\beta\leq D_\alpha+\beta J_\alpha.
$$

Adding shows $(\beta-\alpha)(J_\beta-J_\alpha)\leq0$, so $J_\beta\leq J_\alpha$. Rearranging each comparison then gives the [monotonicity of data fidelity and regularization penalty](../../../../../../../monotonicity-of-data-fidelity-and-regularization-penalty.md)

$$
\boxed{0\leq\alpha(J_\alpha-J_\beta)
\leq D_\beta-D_\alpha
\leq\beta(J_\alpha-J_\beta).}
$$

Hence **the regulariser value is non-increasing and the data misfit is non-decreasing with the parameter**. These inequalities hold for any choices of minimizers at the two distinct parameters, including when uniqueness fails.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
