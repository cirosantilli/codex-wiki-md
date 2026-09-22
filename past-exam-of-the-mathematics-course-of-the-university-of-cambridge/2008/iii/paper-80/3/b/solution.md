<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated hypotheses are precisely the algebraic criterion in part (a). To prove its stability content, compare two [Runge-Kutta method](../../../../../../runge-kutta-method.md) steps for the same [dissipative vector field](../../../../../../dissipative-vector-field.md). Let $d=y_n-z_n$ be the input difference, $D_i=Y_i-Z_i$ the stage differences, and $F_i=f(t_n+c_i h,Y_i)-f(t_n+c_i h,Z_i)$. Then

$$
D_i=d+h\sum_j a_{ij}F_j,\qquad
 d_+=d+h\sum_i b_iF_i.
$$

Expanding the squared [norm](../../../../../../norm.md) of $d_+$ gives

$$
\|d_+\|^2=\|d\|^2+2h\sum_i b_i\langle d,F_i\rangle
+h^2\sum_{i,j}b_i b_j\langle F_i,F_j\rangle.
$$

In each term of the linear sum, replace $d$ by $D_i-h\sum_ja_{ij}F_j$. Symmetrizing the resulting double sum proves the [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md):

$$
\boxed{\|d_+\|^2-\|d\|^2
=2h\sum_i b_i\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\langle F_i,F_j\rangle.}
$$

Dissipativity makes $\langle D_i,F_i\rangle\leq0$, and the weights are nonnegative. For the second term, positive semidefiniteness permits a factorization $M=C^TC$, giving

$$
\sum_{i,j}m_{ij}\langle F_i,F_j\rangle
=\sum_k\left\|\sum_i C_{ki}F_i\right\|^2\geq0.
$$

For $h\geq0$ both contributions in the distance-change identity are nonpositive. Therefore **$\|y_{n+1}-z_{n+1}\|\leq\|y_n-z_n\|$**. This proves the contractivity assertion behind [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md), usually called the [Butcher contractivity theorem](../../../../../../butcher-contractivity-theorem.md). It assumes the compared implicit stage equations have solutions; the matrix condition by itself should not be substituted for a separate stage-solvability argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
