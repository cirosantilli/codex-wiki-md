<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For any normalized [pure state](../../../../../../pure-state.md) on finite-dimensional [Hilbert spaces](../../../../../../hilbert-space-split.md) $\mathcal H_A\otimes\mathcal H_B$, the [Schmidt decomposition](../../../../../../schmidt-decomposition.md) gives

$$
\boxed{|\psi\rangle_{AB}=\sum_{j=1}^r\sqrt{p_j}\,|u_j\rangle_A|v_j\rangle_B,\qquad
p_j>0,\quad\sum_jp_j=1,\quad r\leq\min(d_A,d_B).}
$$

The $u_j$ and $v_j$ form [orthonormal sets](../../../../../../orthonormal-set.md) in their respective spaces. The positive numbers $\sqrt{p_j}$ are the [Schmidt coefficients](../../../../../../schmidt-coefficient.md), and $r$ is the [Schmidt rank](../../../../../../schmidt-rank.md). Taking a [partial trace](../../../../../../partial-trace.md) gives the [reduced density matrices](../../../../../../reduced-density-matrix.md)

$$
\rho_A=\sum_jp_j|u_j\rangle\langle u_j|,\qquad
\rho_B=\sum_jp_j|v_j\rangle\langle v_j|.
$$

Thus the nonzero [eigenvalues](../../../../../../eigenvalue.md) of the two [reduced density matrices](../../../../../../reduced-density-matrix.md) agree.

One construction is a [singular value decomposition](../../../../../../singular-value-decomposition.md) of the coefficient [matrix](../../../../../../matrix.md) $M$ in $|\psi\rangle=\sum_{a,b}M_{ab}|a\rangle|b\rangle$. If $M=U\Sigma V^\dagger$, the columns of $U$ give $u_j$, the complex conjugates of the columns of $V$ give $v_j$, and the [singular values](../../../../../../singular-value.md) give $\sqrt{p_j}$. This also explains why the [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are real and nonnegative.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
