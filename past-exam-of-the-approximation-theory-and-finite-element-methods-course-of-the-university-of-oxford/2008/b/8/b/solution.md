<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Test the discrete equation with $v_h=u_h^{m+1/2}$. The identity $(a-b,a+b)=\|a\|^2-\|b\|^2$ yields

$$
\frac{\|u_h^{m+1}\|_2^2-\|u_h^m\|_2^2}{2\Delta t}
+a(u_h^{m+1/2},u_h^{m+1/2})=0.
$$

Since $e^x\geq1$ on the interval, $a(v,v)\geq\|v\|_{H^1}^2$. Therefore the requested inequality holds:

$$
\boxed{\frac{\|u_h^{m+1}\|_2^2-\|u_h^m\|_2^2}{2\Delta t}
+\|u_h^{m+1/2}\|_{H^1}^2\leq0.}
$$

Discarding the nonnegative second term and iterating proves $\|u_h^m\|_2\leq\|u_h^0\|_2$ for every positive $\Delta t$, with no restriction relating it to $h$. This is unconditional $L^2$ stability; the initial projection also satisfies $\|u_h^0\|_2\leq\|u_0\|_2$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
