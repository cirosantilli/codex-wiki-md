<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The best approximation in the $L^2$ norm is the [orthogonal projection](../../../../../orthogonal-projection.md) onto $\operatorname{span}\{\phi_0,\phi_1\}$. Therefore

$$
p_1=\frac{(x^k,\phi_0)}{\|\phi_0\|_2^2}\phi_0
+\frac{(x^k,\phi_1)}{\|\phi_1\|_2^2}\phi_1.
$$

Using $\int_0^1x^k\,dx=1/(k+1)$,

$$
(x^k,\phi_1)=\frac1{k+2}-\frac1{2(k+1)}
=\frac{k}{2(k+1)(k+2)}.
$$

It follows that

$$
\boxed{p_1(x)=\frac{2(1-k)+6kx}{(k+1)(k+2)}.}
$$

The error is orthogonal to every linear polynomial, so the Pythagorean identity proves optimality and uniqueness. At $k=0$, this gives $p_1=1$; at $k=1$, it gives $p_1=x$. Both are exact because the target itself then belongs to $P_1$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
