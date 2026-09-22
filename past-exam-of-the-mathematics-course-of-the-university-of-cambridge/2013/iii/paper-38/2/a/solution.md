<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the primal in the form $\min c^Tx$ with $Ax\geq b$ and $x\geq0$. Its [dual linear program](../../../../../../dual-linear-program.md) is $\max b^T\lambda$ with $A^T\lambda\leq c$ and $\lambda\geq0$. Indeed, nonnegative combinations of the primal inequalities give $c^Tx\geq\lambda^TAx\geq\lambda^Tb$, which is [weak duality](../../../../../../weak-duality.md). The specific dual is

$$
\boxed{\begin{aligned}
\text{maximize }&3\lambda_1+4\lambda_2+\lambda_3,\\
\text{subject to }&\lambda_1-2\lambda_3\leq2,\\
&2\lambda_1+2\lambda_2\leq4,\\
&-\lambda_1+\lambda_2+3\lambda_3\leq3,\\
&-3\lambda_2+\lambda_3\leq1,\\
&\lambda_1,\lambda_2,\lambda_3\geq0.
\end{aligned}}
$$

The four dual inequalities correspond, in order, to the four primal variables.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
