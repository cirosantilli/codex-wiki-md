<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work with the [L1 norm](../../../../../l1-norm.md) on $\mathbb R^2$. The scalar Lipschitz hypothesis implies

$$
\begin{aligned}
\|\mathbf f(x,\mathbf y)-\mathbf f(x,\mathbf z)\|_1
&=|y_2-z_2|+|F(x,\mathbf y)-F(x,\mathbf z)|\\
&\leq(1+L)\|\mathbf y-\mathbf z\|_1.
\end{aligned}
$$

We may take $L\geq0$. The [compact set](../../../../../compact-space.md) $S$ and continuity give a finite bound $M=\max_S\|\mathbf f\|_1$. Choose

$$
\boxed{0<\eta\leq\min\left\{h,\frac{k}{M+1},\frac1{2(1+L)}\right\}.}
$$

Let $I=[a-\eta,a+\eta]$. The space $C_\eta$ of continuous maps $I\to B_k(\mathbf b)$ is complete in the [supremum norm](../../../../../supremum-norm.md): it is a closed subset of the [Banach space](../../../../../banach-space-split.md) $C(I,\mathbb R^2)$. Define the [Picard operator on a closed ball](../../../../../picard-operator-on-a-closed-ball.md) by

$$
(\mathcal P\mathbf g)(x)=\mathbf b+\int_a^x\mathbf f(t,\mathbf g(t))\,dt.
$$

For any $\mathbf g\in C_\eta$, the [integral triangle inequality](../../../../../integral-triangle-inequality.md) gives

$$
\|\mathcal P\mathbf g(x)-\mathbf b\|_1\leq |x-a|M\leq\eta M<k.
$$

The integrand is continuous, so the result is continuous and remains in the prescribed [closed ball](../../../../../closed-ball.md). Thus $\mathcal P$ is a self-map of the complete space. Moreover,

$$
\|\mathcal P\mathbf g-\mathcal P\mathbf h\|_\infty
\leq\eta(1+L)\|\mathbf g-\mathbf h\|_\infty
\leq\frac12\|\mathbf g-\mathbf h\|_\infty.
$$

It is a [contraction mapping](../../../../../contraction-mapping.md). The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) gives a unique [fixed point](../../../../../fixed-point.md) $\mathbf y$. By the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), the fixed-point identity makes $\mathbf y$ continuously differentiable and gives $\mathbf y'=\mathbf f(x,\mathbf y)$ and $\mathbf y(a)=\mathbf b$. Its first component is twice continuously differentiable, because its derivative is the second component.

Conversely, integrating any solution that remains in the ball makes it a [fixed point](../../../../../fixed-point.md), so it equals $\mathbf y$. A solution starting at $\mathbf b$ cannot first reach the boundary of this ball during $I$: before such an exit the same estimate gives distance at most $\eta M<k$, contradicting distance $k$ at the first exit. This proves **existence and uniqueness on $|x-a|\leq\eta$**, not merely formal convergence of an iteration. It is the local [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) construction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
