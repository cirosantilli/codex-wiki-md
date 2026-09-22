<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the first [Butcher tableau](../../../../../../butcher-tableau.md), $b=(1/2,1/2)^T$ and the off-diagonal entries sum to $1/2$, while each diagonal entry is $1/4$. Thus

$$
BA+A^TB-bb^T=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
$$

The positive weights and zero [matrix](../../../../../../matrix.md) prove that **method 1 is [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**. It is the two-stage [Gauss collocation method](../../../../../../gauss-legendre-method.md).

The second method is explicit and has $b=(1/4,3/8,3/8)^T$. Its first diagonal algebraic-stability entry is

$$
m_{11}=2b_1a_{11}-b_1^2=-\frac1{16}<0.
$$

A [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) [matrix](../../../../../../matrix.md) cannot have a negative diagonal [quadratic form](../../../../../../quadratic-form.md), so **method 2 is not [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**. The negative value supplies a direct test; its order is irrelevant to this conclusion.

For the third method, $A=\begin{pmatrix}1/4&-1/4\\1/4&5/12\end{pmatrix}$ and $b=(1/4,3/4)^T$. Direct computation gives

$$
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\qquad
v^TMv=\frac1{16}(v_1-v_2)^2\geq0.
$$

Both weights are positive, so **method 3 is [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md)**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
