<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

[Convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md) on $[0,T]$ means that its grid error obeys $\max_{0\leq nh\leq T}|y_n-y(nh)|\to0$ as $h\to0$, with consistent initial values.

First, the implicit step of [Backward Euler method](../../../../../backward-euler-method.md) is well-defined for $hL<1$: the map $z\mapsto y_n+hf(t_{n+1},z)$ is a [contraction mapping](../../../../../contraction-mapping.md) on $\mathbb R$, so the [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) gives a unique solution. Let $M=\max_{[0,T]}|y''|$, finite under the stated smoothness. The exact solution's step defect is

$$
d_n=y(t_{n+1})-y(t_n)-hy'(t_{n+1})=\int_{t_n}^{t_{n+1}}[y'(s)-y'(t_{n+1})]ds,
$$

so $|d_n|\leq Mh^2/2$. Subtract the exact and numerical step equations. The [Lipschitz condition](../../../../../lipschitz-continuity.md) gives

$$
|e_{n+1}|\leq\frac{|e_n|+Mh^2/2}{1-hL},\qquad e_n=y_n-y(t_n).
$$

With exact initial data, sum this [geometric progression](../../../../../geometric-progression.md) to obtain

$$
|e_n|\leq\frac{Mh}{2L}\big[(1-hL)^{-n}-1\big].
$$

For $hL\leq1/2$ and $nh\leq T$, $-\log(1-hL)\leq2hL$, so the bracket is at most $e^{2LT}-1$. Thus **the global error is $O(h)$, uniformly on $[0,T]$, and [Backward Euler method](../../../../../backward-euler-method.md) converges with order one**. A vanishing initial error adds only $(1-hL)^{-n}|e_0|$.

Order one is sharp: for $y'=y$, $y(0)=1$ and $nh=T$, $y_n=(1-h)^{-n}=e^T(1+Th/2+O(h^2))$.

For the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$, the [stability function](../../../../../stability-function.md) is $R(z)=1/(1-z)$, $z=h\lambda$. Therefore its [linear stability domain](../../../../../linear-stability-domain.md) is

$$
\boxed{\{z\in\mathbb C:|1-z|\geq1\}.}
$$

The strict inequality gives decay; equality gives bounded amplification. The whole closed left half-plane lies in this region, so [Backward Euler method](../../../../../backward-euler-method.md) is [A-stable](../../../../../a-stability.md).

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
