<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p_n(x)=\sum_{j=0}^nc_jx^j$. The allowed [orthogonal projection](../../../../orthogonal-projection.md) characterization, applied to the [basis](../../../../basis.md) $1,x,\ldots,x^n$, gives the [normal equations](../../../../normal-equation.md)

$$
\boxed{\sum_{j=0}^nG_{ij}c_j=d_i\quad(0\leq i\leq n),\qquad G_{ij}=\int_{-1}^1x^{i+j}\,dx,\quad d_i=\int_{-1}^1u(x)x^i\,dx.}
$$

Explicitly $G_{ij}=0$ if $i+j$ is odd and $G_{ij}=2/(i+j+1)$ if it is even. These equations can also be derived by differentiating $\int(u-\sum c_jx^j)^2dx$ with respect to each coefficient.

The [Gram matrix](../../../../gram-matrix.md) $G$ is a [symmetric positive-definite matrix](../../../../symmetric-positive-definite-matrix.md). For any nonzero real coefficient [vector](../../../../vector.md) $z$,

$$
z^TGz=\int_{-1}^1\left(\sum_{j=0}^nz_jx^j\right)^2dx>0.
$$

The [polynomial](../../../../polynomial-split.md) inside the square is nonzero, so its square is positive on some interval. Hence $G$ has zero [kernel](../../../../kernel-of-a-linear-map-split.md) and is invertible. Thus **the normal equations have exactly one solution**, giving exactly one best [least-squares polynomial](../../../../polynomial-least-squares-approximation.md). This proves both existence and uniqueness. For completeness, if the residual is [orthogonal](../../../../orthogonal-vectors.md) to $\Pi_n$, then for every $q\in\Pi_n$ the [Pythagorean theorem](../../../../pythagorean-theorem.md) gives $\|u-q\|^2=\|u-p_n\|^2+\|p_n-q\|^2$, directly verifying minimality and uniqueness.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
