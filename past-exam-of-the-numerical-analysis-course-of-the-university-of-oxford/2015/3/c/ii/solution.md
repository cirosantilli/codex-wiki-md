<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $r=\sqrt{x_i^2+x_j^2}$. If $r>0$, choose $\theta$ so that

$$
\cos\theta=\frac{x_i}{r},\qquad \sin\theta=\frac{x_j}{r}.
$$

Such an angle exists because the two ratios have squared sum one. Then the changed coordinates are

$$
y_i=\frac{x_i^2+x_j^2}{r}=r,\qquad
y_j=-\frac{x_jx_i}{r}+\frac{x_ix_j}{r}=0.
$$

All other coordinates satisfy $y_k=x_k$. If $r=0$, both input coordinates are zero; take $\theta=0$, giving the [identity matrix](../../../../../identity-matrix.md) on this pair. In all cases,

$$
\boxed{y_i=\sqrt{x_i^2+x_j^2},\qquad y_j=0,\qquad y_k=x_k\ (k\ne i,j).}
$$

This fixes a nonnegative retained coordinate and handles division by zero explicitly. For floating-point computation, the [stable construction of a Givens rotation](../../../../../stable-construction-of-a-givens-rotation.md) uses scaled [Euclidean norm](../../../../../euclidean-norm.md) evaluation to avoid unnecessarily overflowing or underflowing the squares.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
