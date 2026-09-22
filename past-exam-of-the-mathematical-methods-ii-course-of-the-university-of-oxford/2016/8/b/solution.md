<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Stokes theorem](../../../../stokes-theorem.md) to $\mathbf F=\psi\mathbf B$, with $\mathbf B$ an arbitrary constant vector. The [curl product rule for a scalar field](../../../../curl-product-rule-for-a-scalar-field.md) reduces to $\nabla\times(\psi\mathbf B)=\nabla\psi\times\mathbf B$. Using the [scalar triple product](../../../../scalar-triple-product.md),

$$
\mathbf B\cdot\oint_C\psi\,d\mathbf r=\iint_S\hat{\mathbf n}\cdot(\nabla\psi\times\mathbf B)\,dS=\mathbf B\cdot\iint_S(\hat{\mathbf n}\times\nabla\psi)\,dS.
$$

Since these scalar products agree for every $\mathbf B$, the vectors agree. This proves the [vector-valued Stokes identity](../../../../vector-valued-stokes-identity.md)

$$
\boxed{\oint_C\psi\,d\mathbf r=\iint_S(\hat{\mathbf n}\times\nabla\psi)\,dS.}
$$

In particular, the ordering of the [cross product](../../../../cross-product.md) is normal crossed with gradient; reversing it would change the sign.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
