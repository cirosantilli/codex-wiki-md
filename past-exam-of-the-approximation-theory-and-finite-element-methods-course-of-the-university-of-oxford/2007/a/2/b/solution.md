<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\omega(t)=\prod_{r=0}^n(t-x_r)$. For $x$ not one of the nodes, put $c=(u(x)-p_n(x))/\omega(x)$ and define

$$
F(t)=u(t)-p_n(t)-c\omega(t).
$$

This function has zeros at the $n+1$ [interpolation](../../../../../interpolation-split.md) nodes and at the additional point $x$. Repeated [Rolle's theorem](../../../../../rolle-theorem.md) gives a point $\eta$ between the outermost of these points such that $F^{(n+1)}(\eta)=0$. Since $p_n^{(n+1)}=0$ and $\omega^{(n+1)}=(n+1)!$,

$$
c=\frac{u^{(n+1)}(\eta)}{(n+1)!}.
$$

Substitution yields

$$
\boxed{u(x)-p_n(x)=
\frac{u^{(n+1)}(\eta)}{(n+1)!}\prod_{r=0}^n(x-x_r).}
$$

At an [interpolation](../../../../../interpolation-split.md) node both sides are zero, so any $\eta\in[-1,1]$ gives the identity there. The assumed $C^{n+1}$ regularity permits all applications of [Rolle's theorem](../../../../../rolle-theorem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
