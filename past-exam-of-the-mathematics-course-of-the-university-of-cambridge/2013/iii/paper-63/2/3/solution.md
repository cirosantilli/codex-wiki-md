<h1 id="2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an [implicit Runge-Kutta method](../../../../../../implicit-runge-kutta-method.md), [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) means that $b_i\geq0$ and the symmetric matrix

$$
\mathcal M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j
$$

is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md). Here $b_1=b_2=1/2$ and $A+A^T=ee^T/2$, so

$$
\mathcal M=\frac12(A+A^T)-\frac14ee^T=0.
$$

**The method is algebraically stable.** This also explains why the property matters for nonlinear problems. If a vector field satisfies $\langle f(v)-f(w),v-w\rangle\leq0$, the [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md) for two solutions, with stage differences $D_i$ and vector-field differences $F_i$, is

$$
\|d_{n+1}\|^2-\|d_n\|^2
=2h\sum_i b_i\langle D_i,F_i\rangle
-h^2\sum_{i,j}\mathcal M_{ij}\langle F_i,F_j\rangle\leq0.
$$

The first sum is nonpositive and the second vanishes. Thus, whenever the implicit stage equations have the relevant solutions, their updates are contractive in the [Hilbert space](../../../../../../hilbert-space-split.md) norm.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
