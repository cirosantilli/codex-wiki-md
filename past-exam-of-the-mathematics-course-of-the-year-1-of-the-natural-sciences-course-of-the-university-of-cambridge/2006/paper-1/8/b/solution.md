<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Minimize $\frac12\|\mathbf r\|^2$ subject to $\mathbf n_1\cdot\mathbf r=1$, $\mathbf n_2\cdot\mathbf r=2$, where $\mathbf n_1=(2,1,-1)$ and $\mathbf n_2=(1,-1,1)$. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equation gives $\mathbf r=\lambda\mathbf n_1+\mu\mathbf n_2$. Since $\mathbf n_1\cdot\mathbf n_2=0$, $\|\mathbf n_1\|^2=6$, and $\|\mathbf n_2\|^2=3$, the constraints imply $\lambda=1/6$, $\mu=2/3$. Hence

$$
\boxed{\mathbf r_*=(1,-1/2,1/2).}
$$

No explicit parametrization of the line was needed. For any other feasible point, $\mathbf h=\mathbf r-\mathbf r_*$ is [orthogonal](../../../../../orthogonal-vectors.md) to both normals and therefore to $\mathbf r_*$. The [Pythagorean theorem](../../../../../pythagorean-theorem.md) gives $\|\mathbf r\|^2=\|\mathbf r_*\|^2+\|\mathbf h\|^2$, proving the unique global minimum. This is the geometric principle behind the [minimum-norm least-squares solution](../../../../../minimum-norm-least-squares-solution.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
