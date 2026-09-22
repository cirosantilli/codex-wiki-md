<h1 id="21h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $x_0=1$. The constraints are equivalent to $y_i=x_i-x_{i-1}$, so the objective becomes the strictly convex quadratic

$$
J(x_1,\ldots,x_n)=\sum_{i=1}^n\bigl[2(x_i-x_{i-1})^2+x_i^2\bigr].
$$

Its derivative at an interior index gives $5x_i-2x_{i-1}-2x_{i+1}=0$, $1\leq i<n$. The terminal derivative gives $3x_n-2x_{n-1}=0$. The characteristic equation $2r^2-5r+2=0$ has roots $2$ and $1/2$, so

$$
x_i=a2^i+b2^{-i},\qquad
y_i=\frac a2\,2^i-b2^{-i}.
$$

The conditions $x_0=1$ and $3x_n=2x_{n-1}$ give $a+b=1$ and $b=2\cdot4^n a$. Thus

$$
\boxed{a=\frac1{1+2\cdot4^n},\qquad
b=\frac{2\cdot4^n}{1+2\cdot4^n},\qquad
A=\frac1{2(1+2\cdot4^n)},\qquad
B=-\frac{2\cdot4^n}{1+2\cdot4^n}.}
$$

These formulas also cover $n=1$, giving $x_1=2/3$, $y_1=-1/3$.

For a direct application of [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md), use equality constraints $h_i=x_i-1-\sum_{k=1}^iy_k$ and multipliers $\mu_i=-2x_i^*$. The Lagrangian derivatives in $x_i$ vanish. Its derivative in $y_j$ is $4y_j^*+2\sum_{i=j}^nx_i^*$, which also vanishes: putting $S_j=2y_j^*+\sum_{i=j}^nx_i^*$, the interior recurrence gives $S_j-S_{j+1}=0$, and the terminal condition gives $S_n=0$. The Lagrangian has positive-definite quadratic part $\sum_i(x_i^2+2y_i^2)$, so this stationary point is its unique global minimum. The candidate is feasible, and the theorem proves **it is the unique constrained optimal solution**. Equivalently, strict convexity of the eliminated objective proves the same global conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
