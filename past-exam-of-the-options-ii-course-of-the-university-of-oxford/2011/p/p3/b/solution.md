<h1 id="p/p3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $p$ is a minimizer, then for each $q\in\Pi_n$ the quadratic

$$
\|u-p-tq\|^2=\|u-p\|^2-2t(u-p,q)+t^2\|q\|^2
$$

has a minimum at $t=0$, so $(u-p,q)=0$. Conversely, if this orthogonality holds, then for every $q\in\Pi_n$ the [Pythagorean theorem](../../../../../pythagorean-theorem.md) in the [inner product space](../../../../../inner-product-space.md) gives

$$
\|u-q\|^2=\|u-p\|^2+\|p-q\|^2\geq\|u-p\|^2.
$$

Thus the minimizers are exactly the [orthogonal projections](../../../../../orthogonal-projection.md) characterized by

$$
\boxed{(u-p,q)=0\quad\text{for all }q\in\Pi_n.}
$$

For existence, write $p=\sum_{j=0}^n c_jx^j$. The conditions form the [normal equations](../../../../../normal-equations-for-linear-least-squares.md) $Gc=b$, with [Gram matrix](../../../../../gram-matrix.md) $G_{ij}=(x^i,x^j)$ and $b_i=(u,x^i)$. For every nonzero coefficient vector $v$,

$$
v^TGv=\int_{-1}^1x^2\left(\sum_jv_jx^j\right)^2\,dx>0.
$$

Indeed a nonzero [polynomial](../../../../../polynomial-split.md) is nonzero on some open [interval](../../../../../interval-mathematics.md) away from $0$, where the weight is positive. Hence $G$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md) and is invertible, proving existence and uniqueness of $c$. Uniqueness also follows from the preceding [Pythagorean theorem](../../../../../pythagorean-theorem.md) identity. The zero of the weight at one point therefore causes no degeneracy on continuous functions or polynomials.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
