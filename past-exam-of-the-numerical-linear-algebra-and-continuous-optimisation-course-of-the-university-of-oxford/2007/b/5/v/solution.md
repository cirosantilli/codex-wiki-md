<h1 id="b/5/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $D=f(x)-m(s)$ for the predicted decrease, assuming a nonstationary point and a step at least as good as the [Cauchy point](../../../../../cauchy-point.md). When $\Delta\leq\|g\|_2$, part (ii) gives $D\geq\tfrac12\|g\|_2\Delta$. Part (iv), using its weaker requested bound, then gives

$$
|1-\rho|=\frac{|f(x+s)-m(s)|}{D}\leq\frac{2\Delta}{\|g\|_2}.
$$

Consequently $\Delta\leq\tfrac12(1-\eta)\|g\|_2$ implies $\boxed{\rho\geq\eta}$.

For the radius conclusion, use the standard update rules from part (i). Suppose no subsequence of the generated gradient norms tends to zero. Then some $\varepsilon>0$ bounds those norms below eventually. If $\Delta_k\to0$, eventually $\Delta_k\leq\tfrac12(1-\eta_2)\varepsilon$, so every subsequent step is very successful by the preceding estimate. The radius is then maintained or increased, contradicting convergence to zero. Hence **a radius tending to zero forces a subsequence of gradient norms to tend to zero**. The conclusion uses the trust-region update rules as well as the model estimates.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [5](../../5.md)
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
