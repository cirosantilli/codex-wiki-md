<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

A [norm](../../../../../norm.md) is a function $N:\mathbb R^n\to[0,\infty)$ such that $N(x)=0$ exactly when $x=0$, $N(tx)=|t|N(x)$, and $N(x+y)\leq N(x)+N(y)$. Both specified [Lp norms](../../../../../lp-norm.md) are nonnegative, vanish only at zero and satisfy absolute homogeneity immediately from their formulas.

For the $1$-norm, the scalar [triangle inequality](../../../../../triangle-inequality.md) gives $\sum_i|x_i+y_i|\leq\sum_i|x_i|+\sum_i|y_i|$. For the $2$-norm, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\|x+y\|_2^2=\|x\|_2^2+2x\cdot y+\|y\|_2^2
\leq(\|x\|_2+\|y\|_2)^2.
$$

Taking nonnegative square roots proves its [triangle inequality](../../../../../triangle-inequality.md). Hence both are [norms](../../../../../norm.md).

For the [sharp comparison of l1 and l2 norms](../../../../../sharp-comparison-of-l1-and-l2-norms.md), Cauchy-Schwarz yields

$$
\|x\|_1=\sum_i|x_i|\leq\sqrt n\left(\sum_i|x_i|^2\right)^{1/2}.
$$

The vector $(1,\ldots,1)$ attains equality, so no smaller constant works. Conversely, $(\sum_i|x_i|)^2\geq\sum_i|x_i|^2$, giving $\|x\|_2\leq\|x\|_1$. A standard basis vector attains equality. Thus, for $n\geq1$,

$$
\boxed{C_n=\sqrt n,\qquad C'_n=1.}
$$

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
