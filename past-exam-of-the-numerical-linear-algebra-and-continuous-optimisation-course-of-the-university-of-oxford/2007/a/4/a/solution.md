<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Krylov subspace](../../../../../krylov-subspace.md) is $K_k(A,r)=\operatorname{span}\{r,Ar,\ldots,A^{k-1}r\}$. Write $x_k-x_0=q(A)r_0$ with $\deg q\leq k-1$. For the exact solution, $r_0=A(x-x_0)$, so

$$
\boxed{x-x_k=[I-Aq(A)](x-x_0)=p(A)(x-x_0),\quad p(t)=1-tq(t).}
$$

This polynomial has degree at most $k$ and $p(0)=1$. It is the error-polynomial representation for a [Krylov subspace method](../../../../../krylov-subspace-method.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
