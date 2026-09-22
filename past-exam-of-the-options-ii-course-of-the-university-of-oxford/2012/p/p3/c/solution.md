<h1 id="p/p3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The columns outside indices $i,j$ are unchanged coordinate [vectors](../../../../../vector.md). The remaining two columns have nonzero entries only in rows $i,j$, with the $2\times2$ block $M(\theta)$. They have squared [norm](../../../../../norm.md) $\cos^2\theta+\sin^2\theta=1$ and mutual [inner product](../../../../../inner-product-split.md) zero; they are also [orthogonal](../../../../../orthogonal-vectors.md) to all the unchanged columns. Hence $J^TJ=I$.

Let $r=\sqrt{x_i^2+x_j^2}$. If $r>0$, choose $\theta\in[-\pi,\pi]$ with $\cos\theta=x_i/r$ and $\sin\theta=x_j/r$. Then

$$
y_i=\cos\theta\,x_i+\sin\theta\,x_j=r,\qquad
y_j=-\sin\theta\,x_i+\cos\theta\,x_j=0.
$$

Every other coordinate is unchanged. If $r=0$, choose $\theta=0$; the same conclusions hold. Therefore the procedure can be fixed with the nonnegative [pivot](../../../../../pivotal-quantity.md) convention

$$
\boxed{y_i=\sqrt{x_i^2+x_j^2},\qquad y_j=0,\qquad y_k=x_k\ (k\neq i,j).}
$$

This is a [Givens rotation](../../../../../givens-rotation.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
