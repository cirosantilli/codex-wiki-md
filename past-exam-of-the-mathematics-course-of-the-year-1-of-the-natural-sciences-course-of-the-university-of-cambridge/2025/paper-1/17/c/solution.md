<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply [matrix multiplication](../../../../../matrix-multiplication.md) to obtain

$$
M\mathbf x=\mathbf x-\hat{\mathbf n}(\hat{\mathbf n}^T\mathbf x)=\mathbf x-(\hat{\mathbf n}\cdot\mathbf x)\hat{\mathbf n}.
$$

Since $\hat{\mathbf n}$ is a [unit vector](../../../../../unit-vector.md), the subtracted term is the [orthogonal projection](../../../../../orthogonal-projection.md) of $\mathbf x$ along $\hat{\mathbf n}$. Hence **$M$ is the [orthogonal projection onto a plane](../../../../../closest-point-on-a-plane.md) through the origin with [normal vector](../../../../../normal-vector.md) $\hat{\mathbf n}$**. It fixes every [vector](../../../../../vector.md) perpendicular to $\hat{\mathbf n}$ and sends every [scalar multiple](../../../../../scalar-multiple.md) of $\hat{\mathbf n}$ to zero. In particular $\hat{\mathbf n}\cdot M\mathbf x=0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
