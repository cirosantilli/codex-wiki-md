<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the [polygon vertices](../../../../vertex-of-a-polygon.md) of the nondegenerate [triangle](../../../../triangle.md) $K$ as $a_1,a_2,a_3$, and put $m_{ij}=(a_i+a_j)/2$ for its three edge [midpoints](../../../../midpoint.md). The six [monomials](../../../../monomial.md) $1,x_1,x_2,x_1^2,x_1x_2,x_2^2$ form a [basis](../../../../basis.md) of $\mathcal P_2(K)$, so its [dimension](../../../../dimension-vector-space.md) is six. Nondegeneracy matters: $K$ has nonempty interior, and a [polynomial](../../../../polynomial-split.md) vanishing on that interior is the zero [polynomial](../../../../polynomial-split.md).

Let $\lambda_1,\lambda_2,\lambda_3$ be the [affine functions](../../../../affine-function.md) of the [barycentric coordinate system](../../../../barycentric-coordinate-system.md), characterized by $\lambda_i(a_j)=\delta_{ij}$ and $\sum_i\lambda_i=1$. Define six [quadratic polynomials](../../../../quadratic-polynomial.md)

$$
N_i=\lambda_i(2\lambda_i-1)\quad(i=1,2,3),\qquad
N_{ij}=4\lambda_i\lambda_j\quad(1\leq i<j\leq3).
$$

At $a_k$, $N_i(a_k)=\delta_{ik}$ and all $N_{ij}(a_k)$ vanish. At $m_{kl}$, exactly $\lambda_k$ and $\lambda_l$ equal $1/2$, while the third is zero. Thus every $N_i$ vanishes at all three edge [midpoints](../../../../midpoint.md), and $N_{ij}(m_{kl})$ is one for the matching unordered pair and zero otherwise.

These six [polynomials](../../../../polynomial-split.md) have the cardinal property for the six [point evaluation functionals](../../../../point-evaluation-functional.md). Evaluating any vanishing [linear combination](../../../../linear-combination.md) at the nodes forces each of its [coefficients](../../../../coefficient.md) to vanish. They are therefore six [linearly independent](../../../../linear-independence.md) members of a six-dimensional [vector space](../../../../vector-space-split.md), hence a [basis](../../../../basis.md).

In particular, every $p\in\mathcal P_2(K)$ has the unique expansion

$$
\boxed{p=\sum_{i=1}^3p(a_i)\lambda_i(2\lambda_i-1)+\sum_{1\leq i<j\leq3}p(m_{ij})\,4\lambda_i\lambda_j.}
$$

This proves both existence and uniqueness for arbitrary six prescribed nodal values, which is precisely an [unisolvent finite element](../../../../unisolvent-finite-element.md). It also identifies the [finite element degrees of freedom](../../../../finite-element-degree-of-freedom.md) and shape functions of the [quadratic Lagrange triangle](../../../../quadratic-lagrange-triangle.md) explicitly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
