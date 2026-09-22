<h1 id="11d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives a root $r\in(a,b)$, unique because $f'>0$ makes $f$ [strictly increasing](../../../../../../strictly-increasing-function.md). We show that [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md), started at $b$, always stays to the right of $r$. If $x>r$, the [mean value theorem](../../../../../../mean-value-theorem.md) gives $f(x)=f'(\xi)(x-r)$ for some $\xi\in(r,x)$. Since $f''>0$, $f'$ is [strictly increasing](../../../../../../strictly-increasing-function.md), so $0<f'(\xi)<f'(x)$. It follows that

$$
0<\frac{f(x)}{f'(x)}<x-r,\qquad \boxed{r<F(x)<x.}
$$

Induction gives $r<x_{n+1}<x_n\le b$, so the [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md) supplies a limit $\alpha\ge r$. The continuous positive $f'$ is bounded away from zero on $[a,b]$, making $F$ continuous. Passing to the limit in $x_{n+1}=F(x_n)$ gives $\alpha=F(\alpha)$ and hence $f(\alpha)=0$. Uniqueness implies **$\boxed{\alpha=r}$**.

For the rate, apply the [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) to $f$ between $r$ and $x_n$:

$$
0=f(r)=f(x_n)-f'(x_n)(x_n-r)+\frac12f''(\xi_n)(x_n-r)^2,\qquad \xi_n\in(r,x_n).
$$

With $e_n=x_n-r>0$, rearrangement gives

$$
\boxed{e_{n+1}=\frac{f''(\xi_n)}{2f'(x_n)}e_n^2,\qquad
\frac{e_{n+1}}{e_n^2}\longrightarrow\frac{f''(r)}{2f'(r)}>0.}
$$

Thus the [monotone Newton convergence for a strictly convex function](../../../../../../monotone-newton-convergence-for-a-strictly-convex-function.md) has **quadratic convergence**. More concretely, if $K=\max_{[a,b]}f''/[2\min_{[a,b]}f']$, then $e_{n+1}\le Ke_n^2$. Once $Ke_N<1$, induction gives $e_{N+j}\le K^{-1}(Ke_N)^{2^j}$, exhibiting the repeated squaring of small errors.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
