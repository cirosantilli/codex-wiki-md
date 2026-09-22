<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For

$$
Lu=a^{ij}D_{ij}u+b^iD_iu+cu,
\qquad c\leq0,
$$

the [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) states that $Lu\geq0$ implies

$$
\max_{\overline\Omega}u\leq\max\{0,\max_{\partial\Omega}u\}.
$$

In particular, a solution of $Lu=0$ cannot have a positive interior maximum exceeding its boundary maximum.

Because the coefficient matrix is positive definite and the closure of the smooth bounded domain is compact, strict ellipticity supplies a uniform lower bound after restricting to $\overline\Omega$. Rotate and translate coordinates so that $\Omega$ is bounded in the $x_1$ direction, and set $h=e^{\gamma x_1}$. For sufficiently large $\gamma$,

$$
Lh=e^{\gamma x_1}(\gamma^2a^{11}+\gamma b^1+c)>0.
$$

If $u+\varepsilon h$ had a positive interior maximum, its gradient would vanish and its [Hessian matrix](../../../../../../hessian-matrix.md) would be negative semidefinite there, giving $L(u+\varepsilon h)\leq0$. This contradicts $L(u+\varepsilon h)=\varepsilon Lh>0$. Comparing on the boundary and sending $\varepsilon\downarrow0$ proves the assertion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
