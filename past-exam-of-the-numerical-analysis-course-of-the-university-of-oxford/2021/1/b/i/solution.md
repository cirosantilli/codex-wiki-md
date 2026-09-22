<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mathcal P_n$ for the [vector space](../../../../../vector-space-split.md) of [polynomials](../../../../../polynomial-split.md) of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $n$, and put $p_n(x)=\sum_{j=0}^na_jx^j$. As the question calls the weighted integral an [inner product](../../../../../inner-product-split.md), its finiteness is implicit; for example, a positive integrable weight $w$ suffices for all the [continuous functions](../../../../../continuous-function.md) involved here.

For every $q\in\mathcal P_n$, differentiating the squared [weighted norm](../../../../../weighted-norm.md) $\|f-p_n-tq\|_w^2$ at its minimum $t=0$ gives the [orthogonality](../../../../../orthogonal-vectors.md) equations

$$
\langle f-p_n,q\rangle_w=0.
$$

In particular, the requested [linear system](../../../../../system-of-linear-equations.md) is

$$
\boxed{\sum_{j=0}^n a_j\int_{-1}^1w(x)x^{j+k}\,dx
=\int_{-1}^1w(x)f(x)x^k\,dx,\qquad k=0,\ldots,n.}
$$

Its [Gram matrix](../../../../../gram-matrix.md) $G_{kj}=\int_{-1}^1w(x)x^{k+j}\,dx$ is a [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md): for any nonzero [vector](../../../../../vector.md) $a$,

$$
a^TGa=\int_{-1}^1w(x)\left(\sum_{j=0}^na_jx^j\right)^2dx>0.
$$

Indeed a nonzero [polynomial](../../../../../polynomial-split.md) is nonzero on some open interval, and the weight is positive. Therefore $G$ is an [invertible matrix](../../../../../invertible-matrix.md), proving uniqueness. Conversely, if these equations hold, the [Pythagorean theorem in an inner-product space](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives, for every $q\in\mathcal P_n$,

$$
\|f-(p_n+q)\|_w^2=\|f-p_n\|_w^2+\|q\|_w^2,
$$

so the solution really is the unique [best approximation](../../../../../best-approximation-in-a-normed-space.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
