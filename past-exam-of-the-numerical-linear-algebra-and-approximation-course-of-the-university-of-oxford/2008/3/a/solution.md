<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e_j=x-x^{(j)}$. The underlying [Richardson iteration](../../../../richardson-iteration.md) gives $e_j=(I-A)^je_0$. The polynomials $1,(1-t),\ldots,(1-t)^k$ form a basis for polynomials of degree at most $k$. Thus write

$$
p_k(t)=\sum_{j=0}^kc_j(1-t)^j,\qquad\sum_{j=0}^kc_j=p_k(0)=1.
$$

Define $y^{(k)}=\sum_{j=0}^kc_jx^{(j)}$. Since the coefficients sum to one,

$$
\boxed{x-y^{(k)}=\sum_jc_je_j=p_k(A)e_0.}
$$

The [spectral theorem for real symmetric matrices](../../../../spectral-theorem-for-real-symmetric-matrices.md) supplies an [orthonormal basis](../../../../orthonormal-basis.md) of [eigenvectors](../../../../eigenvector.md). In that basis $p_k(A)$ has diagonal entries $p_k(\lambda_i)$, so

$$
\boxed{\|x-y^{(k)}\|_2\leq\max_i|p_k(\lambda_i)|\,\|x-x^{(0)}\|_2.}
$$

The algebraic recombination is valid in exact arithmetic even if the original unaccelerated iterates themselves fail to converge.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
