# Vector projection

↑ **Parent:** [Dot product](dot-product.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_projection)

The [vector projection](vector-projection.md) multiplies the [scalar projection](scalar-projection.md) by the chosen [unit vector](unit-vector.md), giving the [orthogonal projection](orthogonal-projection.md) onto the [linear span](linear-span.md) of a nonzero real [Euclidean vector](euclidean-vector.md) $\mathbf c$:

$$
\mathbf p=\operatorname{proj}_{\mathbf c}\mathbf a
=\frac{\mathbf a\cdot\mathbf c}{\mathbf c\cdot\mathbf c}\mathbf c,\qquad
\mathbf r=\mathbf a-\mathbf p,\qquad \mathbf r\cdot\mathbf c=0.
$$

For $\mathbf a=(3,4)$ and $\mathbf c=(2,0)$, this gives $\mathbf p=(6/4)(2,0)=(3,0)$ and $\mathbf r=(0,4)$; the [dot product](dot-product.md) $\mathbf r\cdot\mathbf c=0$ checks the [orthogonal projection residual](orthogonal-projection-residual.md). Replacing $\mathbf c$ by $(-2,0)$ gives the same $\mathbf p=(-6/4)(-2,0)=(3,0)$: reversing direction changes the [scalar projection](scalar-projection.md), but preserves the [vector projection](vector-projection.md) onto the line.

For a short proof of the nearest-point property, any [vector](vector.md) $\mathbf z$ on this line satisfies $\|\mathbf a-\mathbf z\|^2=\|\mathbf r\|^2+\|\mathbf p-\mathbf z\|^2$ by the [Pythagorean identity](pythagorean-theorem-in-an-inner-product-space.md). The second term is uniquely minimized at $\mathbf z=\mathbf p$. This connects a directional measurement to the [orthogonal projection](orthogonal-projection.md) used in approximation.[Strang, MIT 18.06, Lecture 15: projections onto subspaces](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-15-projections-onto-subspaces/)

## ↑ Ancestors (7)

1. [Dot product](dot-product.md)
2. [Inner product](inner-product-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dot product](dot-product.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/10/b/solution.md)
- [Vector projection](vector-projection.md)
