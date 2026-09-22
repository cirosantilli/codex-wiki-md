<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [Runge-Kutta method](../../../../../../runge-kutta-method.md) with real stage matrix $A=(a_{ij})$ and weights $b_i$, define

$$
M=\operatorname{diag}(b)A+A^T\operatorname{diag}(b)-bb^T,
\qquad m_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

The method has [algebraic stability of a Runge-Kutta method](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) if

$$
\boxed{b_i\geq0\text{ for every }i,\qquad M\text{ is positive semidefinite}.}
$$

The matrix condition means $z^TMz\geq0$ for every real vector $z$. Its significance is nonlinear contractivity: an algebraically stable method, on well-defined stage solutions, is [B-stable](../../../../../../b-stability.md) for a [dissipative vector field](../../../../../../dissipative-vector-field.md) satisfying $\langle f(t,y)-f(t,z),y-z\rangle\leq0$. This is distinct from scalar [A-stability](../../../../../../a-stability.md), which concerns the linear test equation. The contractivity proof in part (b) explains the matrix criterion directly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
