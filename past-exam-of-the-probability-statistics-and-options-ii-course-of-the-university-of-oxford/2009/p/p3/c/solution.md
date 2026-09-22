<h1 id="p/p3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $x$ is a node, both sides vanish and any $\xi\in(a,b)$ works. Otherwise put $\omega(t)=\prod_i(t-x_i)$ and $C=(f(x)-p_n(x))/\omega(x)$. The function $H(t)=f(t)-p_n(t)-C\omega(t)$ has $n+2$ distinct zeros, at the nodes and at $x$. Repeated application of [Rolle's theorem](../../../../../rolle-theorem.md) gives an interior point $\xi$ where $H^{(n+1)}(\xi)=0$. As $p_n^{(n+1)}=0$ and $\omega^{(n+1)}=(n+1)!$, this gives $C=f^{(n+1)}(\xi)/(n+1)!$. Therefore

$$
\boxed{f(x)-p_n(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}\prod_{i=0}^n(x-x_i).}
$$

The distinct nodes and $n\ge1$ ensure $a<b$, so the interior point is meaningful.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
