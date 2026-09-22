<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Krylov subspace](../../../../krylov-subspace.md) is $\boxed{K_k(A,b)=\operatorname{span}\{b,Ab,\ldots,A^{k-1}b\}}$. If $y\in K_k$, write $y=q(A)b$ with $\deg q\leq k-1$. Since $b=Ax$,

$$
x-y=[I-Aq(A)]x=p(A)x,\qquad p(t)=1-tq(t),
$$

which has degree at most $k$ and $p(0)=1$. Conversely, if $x-y=p(A)x$ with these properties, then $q(t)=(1-p(t))/t$ is a polynomial of degree at most $k-1$ and

$$
\boxed{y=Aq(A)x=q(A)b\in K_k(A,b).}
$$

This is the polynomial description of the admissible errors in a [Krylov subspace method](../../../../krylov-subspace-method.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
