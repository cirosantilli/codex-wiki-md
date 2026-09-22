<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [tridiagonal matrix](../../../../tridiagonal-matrix.md) with subdiagonal $a_i$, diagonal $b_i$ and superdiagonal $c_i$, [banded Gaussian elimination](../../../../banded-gaussian-elimination.md) introduces no fill beyond the original band. The [Thomas algorithm](../../../../tridiagonal-matrix-algorithm.md) uses

$$
p_1=b_1,\qquad\ell_i=a_i/p_{i-1},\qquad p_i=b_i-\ell_ic_{i-1}\quad(i=2,\ldots,n).
$$

Update the right side by $d_1=f_1$, $d_i=f_i-\ell_id_{i-1}$. Then [back substitution](../../../../back-substitution.md) gives

$$
\boxed{x_n=d_n/p_n,\qquad x_i=(d_i-c_ix_{i+1})/p_i\quad(i=n-1,\ldots,1).}
$$

Each row requires only a fixed number of arithmetic operations, so both work and storage are $\boxed{O(n)}$. The assumed absence of a need for pivoting includes nonzero elimination pivots $p_i$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
