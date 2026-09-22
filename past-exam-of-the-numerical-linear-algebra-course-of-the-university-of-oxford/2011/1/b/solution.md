<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [singular value decomposition](../../../../singular-value-decomposition.md) and the [orthogonal invariance of the Euclidean norm](../../../../orthogonal-invariance-of-the-euclidean-norm.md). Put $z=V^Tx$ and $c=U^Tb$. Since precisely $\sigma_1,\ldots,\sigma_r$ are positive,

$$
\|Ax-b\|_2^2=\sum_{j=1}^r(\sigma_jz_j-c_j)^2+\sum_{j=r+1}^m c_j^2.
$$

The second sum is independent of $x$ and cannot be removed. The first sum vanishes exactly when $z_j=c_j/\sigma_j$ for $1\leq j\leq r$, while $z_{r+1},\ldots,z_n$ are arbitrary. Thus every [least-squares solution](../../../../least-squares-solution-of-a-linear-inverse-problem.md) is

$$
\boxed{x=\sum_{j=1}^r\frac{u_j^Tb}{\sigma_j}v_j+\sum_{j=r+1}^n\alpha_jv_j,\qquad\alpha_j\in\mathbb R.}
$$

The unavoidable [linear-system residual](../../../../linear-system-residual.md) is the component of $b$ [orthogonal](../../../../orthogonal-vectors.md) to the [column space](../../../../column-space.md) of $A$:

$$
\boxed{\min_x\|Ax-b\|_2=\left(\sum_{j=r+1}^m|u_j^Tb|^2\right)^{1/2}.}
$$

The [minimum-norm least-squares solution](../../../../minimum-norm-least-squares-solution.md) sets all $\alpha_j=0$ and equals $A^+b$, where $A^+$ is the [Moore-Penrose inverse](../../../../moore-penrose-inverse.md). The squared minimum, rather than the minimum itself, is the second sum in the first display.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
