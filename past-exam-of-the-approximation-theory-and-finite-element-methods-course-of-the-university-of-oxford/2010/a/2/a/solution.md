<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e=u-p$. If $p$ minimizes the squared [L2 norm](../../../../../l2-norm.md) error, then for any $q\in A$ the real quadratic $\|e-tq\|_2^2=\|e\|_2^2-2t(e,q)+t^2\|q\|_2^2$ has its minimum at $t=0$. Its [derivative](../../../../../derivative.md) there is zero, giving $(e,q)=0$.

Conversely, if $e$ is [orthogonal](../../../../../orthogonal-vectors.md) to $A$, then for every $q\in A$, $p-q\in A$ and the [Pythagorean theorem for inner product spaces](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\boxed{\|u-q\|_2^2=\|u-p\|_2^2+\|p-q\|_2^2\geq\|u-p\|_2^2.}
$$

This proves the equivalence and identifies $p$ as an [orthogonal projection](../../../../../orthogonal-projection.md). It characterizes a minimizer whenever one exists; a general nonclosed [vector subspace](../../../../../vector-subspace.md) need not admit a projection for every $u$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
