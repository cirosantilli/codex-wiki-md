<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $g_j=G_{1/L}(x^j)$, $r_j=\|x^j-x^*\|^2$ and $\delta_j=\phi(x^j)-\phi(x^*)$. Here $g_j$ is the [proximal gradient mapping](../../../../proximal-gradient-mapping.md), $r_j$ is a squared [Euclidean distance](../../../../euclidean-distance.md), and $\delta_j\geq0$ because $x^*$ is a [global minimizer](../../../../global-minimizer.md). The update gives $x^{j+1}=x^j-g_j/L$.

First use the supplied inequality (1) with $z=x^j$:

$$
\phi(x^{j+1})\leq\phi(x^j)-\frac1{2L}\|g_j\|^2\leq\phi(x^j).
$$

Thus the [objective function](../../../../objective-function.md) values, and hence the errors $\delta_j$, are nonincreasing. Next use (1) with $z=x^*$:

$$
\delta_{j+1}\leq g_j^T(x^j-x^*)-\frac1{2L}\|g_j\|^2.
$$

Expansion of the squared [Euclidean norm](../../../../euclidean-norm.md) gives

$$
r_{j+1}=r_j-\frac2L g_j^T(x^j-x^*)+\frac1{L^2}\|g_j\|^2,
$$

so the last bound is exactly $\delta_{j+1}\leq L(r_j-r_{j+1})/2$.

The [telescoping sum](../../../../telescoping-sum.md) over $j=0,\ldots,k-1$ therefore gives

$$
\sum_{j=0}^{k-1}\delta_{j+1}\leq\frac L2(r_0-r_k)\leq\frac L2r_0.
$$

Since each summand is at least $\delta_k$, we obtain the [proximal gradient objective error bound](../../../../proximal-gradient-objective-error-bound.md)

$$
\boxed{\phi(x^k)-\phi(x^*)\leq\frac L{2k}\|x^0-x^*\|^2,\qquad k\geq1.}
$$

**The bound holds for the last iterate.** The monotonicity of the [objective function](../../../../objective-function.md) values is what converts an averaged estimate into this last-iterate estimate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
