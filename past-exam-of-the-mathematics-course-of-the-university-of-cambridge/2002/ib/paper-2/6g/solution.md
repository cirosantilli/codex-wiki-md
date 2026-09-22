<h1 id="6g/solution">Solution</h1>

↑ **Parent:** [6G](../6g.md)

The [minimal polynomial](../../../../../minimal-polynomial.md) divides the annihilating polynomial $t^2(t-1)$, since $A^3-A^2=0$. Every nonconstant monic divisor can occur in dimension four: use [Jordan blocks](../../../../../jordan-block.md) of sizes at most two at [eigenvalue](../../../../../eigenvalue.md) $0$ and of size one at [eigenvalue](../../../../../eigenvalue.md) $1$, adding scalar blocks as needed. The complete list is

$$
\boxed{t,\quad t^2,\quad t-1,\quad t(t-1),\quad t^2(t-1)}.
$$

For example the first four occur for $0$, $J_2(0)\oplus0\oplus0$, $I$, and $\operatorname{diag}(0,0,1,1)$, respectively; the final one occurs for $J_2(0)\oplus0\oplus1$.

Failure to be [diagonalizable](../../../../../diagonalizable-matrix.md) requires a size-two [Jordan block](../../../../../jordan-block.md) at zero. The condition $A^2\ne0$ requires at least one block at one, since every allowed zero block squares to zero. A size-two zero block and one scalar block at one leave only one dimension. It can carry zero or one. Thus, up to permutation of blocks, **the only possible [Jordan normal forms](../../../../../jordan-normal-form.md) are**

$$
\boxed{J_2(0)\oplus[0]\oplus[1],\qquad J_2(0)\oplus[1]\oplus[1]},\qquad J_2(0)=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

## ↑ Ancestors (10)

1. [6G](../6g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
