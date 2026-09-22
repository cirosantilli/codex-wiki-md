<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume first that $A\subseteq\mathbb F_3^n$ is a [cap set](../../../../../cap-set.md). Over the [finite field](../../../../../finite-field.md) $\mathbb F_3$, define

$$
T(x,y,z)=\prod_{i=1}^n\left(1-(x_i+y_i+z_i)^2\right).
$$

Since $1-t^2$ is one at $t=0$ and zero at $t=\pm1$, $T$ is the [indicator function](../../../../../indicator-function.md) of $x+y+z=0$. If $x,y,z\in A$ satisfy this equation, then either they are all equal or they are three distinct points; the latter is excluded. Thus $T|_{A^3}$ is a [diagonal tensor](../../../../../diagonal-tensor.md) with every diagonal entry equal to one, and the [slice rank of a diagonal tensor](../../../../../slice-rank-of-a-diagonal-tensor.md) gives

$$
\operatorname{slice\ rank}(T|_{A^3})=|A|.
$$

Expand $T$ as a [polynomial](../../../../../polynomial-split.md). Every variable has exponent at most two, and every [monomial](../../../../../monomial.md) has total degree at most $2n$. Splitting a monomial's degree among its $x$-, $y$-, and $z$-blocks, at least one block has degree at most $2n/3$. Assign each monomial to one such block and group together terms with the same low-degree block monomial. Each group is one slice, so

$$
|A|\leq3m_n,
$$

where

$$
m_n=\left|\left\{\alpha\in\{0,1,2\}^n:\sum_i\alpha_i\leq\frac{2n}{3}\right\}\right|.
$$

If $X_i=1-\alpha_i$, then the $X_i$ are [independent random variables](../../../../../independent-random-variables.md) uniformly distributed on $\{-1,0,1\}$ and

$$
\frac{m_n}{3^n}
=\mathbb P\left(\sum_iX_i\geq\frac n3\right)
\leq e^{-n/12}
$$

by the given [tail probability](../../../../../tail-probability.md) bound. Consequently every cap set satisfies

$$
|A|\leq3^{n+1}e^{-n/12}.
$$

Put $C_0=3e^{-1/24}<3$. For $n\geq27$, the preceding bound is at most $C_0^n$. For each of the finitely many $1\leq n<27$, a cap set is a proper subset of $\mathbb F_3^n$, so its size is at most $3^n-1$. We may therefore choose

$$
\max\left\{C_0,\max_{1\leq n<27}(3^n-1)^{1/n}\right\}<C<3.
$$

Every cap set then has size strictly below $C^n$. Equivalently,

$$
\boxed{|A|\geq C^n\quad\Longrightarrow\quad
\text{$A$ contains distinct $x,y,z$ with $x+y+z=0$.}}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 147](../../paper-147-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
