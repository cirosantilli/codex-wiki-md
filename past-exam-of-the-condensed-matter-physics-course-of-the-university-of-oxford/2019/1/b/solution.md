<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $v=\mathbf a_1\cdot(\mathbf a_2\times\mathbf a_3)\ne0$. Define

$$
\boxed{\mathbf b_1=\frac{2\pi}{v}\mathbf a_2\times\mathbf a_3,\quad\mathbf b_2=\frac{2\pi}{v}\mathbf a_3\times\mathbf a_1,\quad\mathbf b_3=\frac{2\pi}{v}\mathbf a_1\times\mathbf a_2.}
$$

The [scalar triple product](../../../../scalar-triple-product.md) gives $\mathbf a_i\cdot\mathbf b_j=2\pi\delta_{ij}$. Consequently every integer combination $\mathbf G=\sum_jm_j\mathbf b_j$ satisfies

$$
\mathbf G\cdot\mathbf R=2\pi\sum_jm_jn_j\in2\pi\mathbb Z,\qquad e^{i\mathbf G\cdot\mathbf R}=1.
$$

This proves that the proposed vectors generate points in the [reciprocal lattice](../../../../reciprocal-lattice.md), but primitiveness also requires the converse. Let $\mathbf G$ satisfy the exponential condition for every [lattice vector](../../../../lattice-vector.md), and in particular for $\mathbf R=\mathbf a_i$. Then

$$
m_i=\frac{\mathbf G\cdot\mathbf a_i}{2\pi}\in\mathbb Z.
$$

Since the $\mathbf b_i$ form a [basis](../../../../basis.md) of three-dimensional space, the vector $\sum_i m_i\mathbf b_i$ has the same dot products with each $\mathbf a_j$ as $\mathbf G$. Their difference is orthogonal to three independent vectors and is zero. Hence

$$
\boxed{\Lambda^*=\left\{\sum_i m_i\mathbf b_i:m_i\in\mathbb Z\right\},}
$$

and no additional [reciprocal lattice vectors](../../../../reciprocal-lattice-vector.md) lie outside that integer span. Thus the $\mathbf b_i$ are primitive, not merely three possible reciprocal translations.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
