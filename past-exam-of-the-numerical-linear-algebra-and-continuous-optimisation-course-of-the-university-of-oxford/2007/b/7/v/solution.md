<h1 id="b/7/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [Armijo condition](../../../../../armijo-condition.md) with $p_k=-g(x_k)$ gives $f(x_k)-f(x_{k+1})\geq\beta\alpha_k\|g(x_k)\|_2^2$. Summing these inequalities telescopes to

$$
\boxed{f(x_0)-f(x_{j+1})\geq\beta\sum_{k=0}^j\alpha_k\|g(x_k)\|_2^2.}
$$

If $f\geq f_{\inf}$, these partial sums of nonnegative terms are bounded above by $(f(x_0)-f_{\inf})/\beta$. The resulting series converges, so its terms tend to zero: $\boxed{\alpha_k\|g(x_k)\|_2^2\to0}$.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [7](../../7.md)
3. [B](../../../b.md)
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
