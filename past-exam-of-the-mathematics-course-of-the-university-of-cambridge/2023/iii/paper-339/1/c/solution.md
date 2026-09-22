<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $z_i(x)=\langle a_i,x\rangle+b_i$. The [log-sum-exp function](../../../../../../log-sum-exp-function.md) is convex and composition with the [affine functions](../../../../../../affine-function.md) $z_i$ preserves convexity, so $f_\beta$ is [convex](../../../../../../convex-function.md). Directly, its [Hessian matrix](../../../../../../hessian-matrix.md) will also be shown [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) in part d.

Let $M=f(x)=\max_i z_i(x)$. Factoring $e^{\beta M}$ out of the sum gives

$$
f_\beta(x)
=M+\frac1\beta\log\sum_i e^{\beta(z_i(x)-M)}.
$$

At least one term in the sum is $1$, while every term is at most $1$. Therefore

$$
1\leq\sum_i e^{\beta(z_i-M)}\leq m,
$$

and hence

$$
\boxed{f(x)\leq f_\beta(x)\leq f(x)+\frac{\log m}{\beta}.}
$$

**Thus $f_\beta$ is a uniform [smooth maximum](../../../../../../smooth-maximum.md) of the affine pieces of $f$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
