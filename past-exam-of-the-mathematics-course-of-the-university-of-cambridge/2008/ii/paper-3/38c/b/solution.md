<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $h\lambda/2<1$, the implicit step map $z\mapsto y_n+(h/2)[f(t_n,y_n)+f(t_{n+1},z)]$ is a [contraction](../../../../../../contraction-mapping.md), so the [Banach fixed-point theorem](../../../../../../contraction-mapping-theorem.md) supplies a unique next value. Smoothness of the exact solution gives the one-step defect

$$
d_n=y(t_{n+1})-y(t_n)-\frac h2\bigl[y'(t_n)+y'(t_{n+1})\bigr],\qquad |d_n|\leq Ch^3,
$$

uniformly on $[0,T]$, by the [trapezoidal rule](../../../../../../trapezoidal-rule.md) error estimate or a direct Taylor expansion. Let $e_n=y_n-y(t_n)$. Subtracting exact and numerical steps and applying the [Lipschitz condition](../../../../../../lipschitz-continuity.md) gives

$$
(1-h\lambda/2)|e_{n+1}|\leq(1+h\lambda/2)|e_n|+Ch^3.
$$

Put $r_h=(1+h\lambda/2)/(1-h\lambda/2)$. With $e_0=0$, iteration yields $|e_n|\leq[Ch^3/(1-h\lambda/2)](r_h^n-1)/(r_h-1)$. Since $r_h-1=h\lambda/(1-h\lambda/2)$, this is $Ch^2(r_h^n-1)/\lambda$. For sufficiently small $h$, $\log r_h\leq2\lambda h$, so $r_h^n\leq e^{2\lambda T}$ whenever $nh\leq T$. Therefore

$$
\boxed{\max_{nh\leq T}|e_n|\leq\frac C\lambda(e^{2\lambda T}-1)h^2\longrightarrow0.}
$$

This proves convergence with global order two directly from the defect bound and stability recurrence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
