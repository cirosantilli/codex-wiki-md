<h1 id="p/p3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $x$ is a node the error and the product both vanish, and any interior $\xi$ works. Otherwise put $\omega(t)=\prod_{i=0}^n(t-x_i)$ and $C=(f(x)-p_n(x))/\omega(x)$. The [function](../../../../../function-split.md)

$$
R(t)=f(t)-p_n(t)-C\omega(t)
$$

has $n+2$ distinct zeros, at the nodes and at $x$. Repeated [Rolle's theorem](../../../../../rolle-theorem.md) gives a point $\xi$ between the extreme zeros, and therefore in $(a,b)$, where $R^{(n+1)}(\xi)=0$. Since $p_n^{(n+1)}=0$ and $\omega^{(n+1)}=(n+1)!$, one gets $C=f^{(n+1)}(\xi)/(n+1)!$. Substitution gives

$$
\boxed{f(x)-p_n(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}\prod_{i=0}^n(x-x_i)}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
