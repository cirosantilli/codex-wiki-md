<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $e_1,\ldots,e_n$ denote the standard [basis of a module](../../../../basis-of-a-module.md) of the [free module](../../../../free-module.md) $R^n$. Since the [module homomorphism](../../../../module-homomorphism.md) $\phi:R^m\to M$ is [surjective](../../../../surjective-function.md), choose $v_j\in R^m$ such that $\phi(v_j)=\psi(e_j)$ for each $j$. Define

$$
\boxed{q:R^n\longrightarrow R^m,\qquad q\left(\sum_{j=1}^n r_je_j\right)=\sum_{j=1}^n r_jv_j}.
$$

Uniqueness of coordinates in a [basis of a module](../../../../basis-of-a-module.md) makes this well-defined, and the formula preserves [addition](../../../../addition.md) and [scalar multiplication](../../../../scalar-multiplication.md), so $q$ is a [module homomorphism](../../../../module-homomorphism.md). For every $x=\sum_jr_je_j$,

$$
\phi(q(x))=\sum_jr_j\phi(v_j)=\sum_jr_j\psi(e_j)=\psi(x).
$$

Thus $\boxed{\phi\circ q=\psi}$. This is the [lifting property of a free module](../../../../lifting-property-of-a-free-module.md); only the [surjectivity](../../../../surjective-function.md) of $\phi$ is needed for this part.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
