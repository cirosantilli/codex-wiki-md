# Second-order-cone optimality certificate

↑ **Parent:** [Conic dual problem](conic-dual-problem.md)

A curved [feasible set](feasible-region.md) can have the same certificate structure. Consider

$$
\min_{t,z}t\qquad\text{subject to}\qquad \sqrt{1+z^2}\leq t.
$$

Write $x=(t,z)^T$ and use the [second-order cone](second-order-cone.md) $K=\{(s_0,s_1,s_2):s_0\geq\sqrt{s_1^2+s_2^2}\}$. In this coordinate ordering,

$$
A=\begin{pmatrix}1&0\\0&0\\0&1\end{pmatrix},\quad
b=\begin{pmatrix}0\\-1\\0\end{pmatrix},\quad
c=\begin{pmatrix}1\\0\end{pmatrix},\quad
Ax-b=(t,1,z)^T.
$$

[Self-duality of a second-order cone](self-duality-of-a-second-order-cone.md) makes $K^*=K$. The equality $A^Ty=c$ forces $y_0=1$ and $y_2=0$, leaving $-1\leq y_1\leq1$. Its dual [objective function](objective-function.md) is $b^Ty=-y_1$, maximized at $y=(1,-1,0)^T$. Thus every [feasible point](feasible-point.md) satisfies $t\geq1$, and $(t,z)=(1,0)$ attains that bound: $\boxed{p_*=d_*=1}$.

<a id="image-a-curved-primal-constraint-and-an-interval-of-dual-certificates"></a>
![](conic-second-order-primal-and-dual-slices.png)

**[Figure 6](#image-a-curved-primal-constraint-and-an-interval-of-dual-certificates). A curved primal constraint and an interval of dual certificates**. The left panel is the slice $s_1=1$ of the [second-order cone](second-order-cone.md), so its boundary is $t=\sqrt{1+z^2}$. The right panel is the dual slice $y_0=1$, $y_2=0$: admissible $y_1$ form $[-1,1]$, and $-y_1$ reaches $1$ at $y_1=-1$. The optimal [slack variable](slack-variable.md) and [dual variable](dual-variable.md) lie on different cone boundary rays with zero [dot product](dot-product.md).

The zero [dot product](dot-product.md) is $(1,1,0)\cdot(1,-1,0)=0$. Individual coordinate products need not be nonnegative here: the cancellation $1-1=0$ occurs across coordinates. The valid [complementary slackness](complementary-slackness.md) condition is cone-level [orthogonality](orthogonal-vectors.md), rather than the coordinatewise interpretation of the [nonnegative orthant](nonnegative-orthant.md).

## ↑ Ancestors (7)

1. [Conic dual problem](conic-dual-problem.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
