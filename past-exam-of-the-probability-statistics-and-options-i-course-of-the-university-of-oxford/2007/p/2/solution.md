<h1 id="p/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Richardson extrapolation](../../../../richardson-extrapolation.md) combines approximations with a known leading error power to cancel that error. If $A(h)=I+ch^p+O(h^{p+q})$, then $(2^pA(h)-A(2h))/(2^p-1)$ removes $ch^p$.

Let $x_j=a+jh$ for an even number $n$ of equal subintervals, with $x_n=b$. The [composite trapezoidal rule](../../../../composite-trapezoidal-rule.md) is

$$
T_h=h\left[\frac{f_0+f_n}{2}+\sum_{j=1}^{n-1}f_j\right].
$$

The [Simpson's rule](../../../../simpson-s-rule.md) is

$$
S_h=\frac h3\left[f_0+f_n+
4\sum_{\substack{1\leq j<n\\j\ {\rm odd}}}f_j+
2\sum_{\substack{2\leq j<n\\j\ {\rm even}}}f_j\right].
$$

Assume an error expansion $T_h=I+c_2h^2+O(h^4)$, with the same coefficient $c_2$ on refined uniform meshes; $f\in C^4([a,b])$ is sufficient for this form. The coarser rule is $T_{2h}=h[f_0+f_n+2\sum_{\rm even}f_j]$. Direct coefficient collection gives

$$
\boxed{\frac{4T_h-T_{2h}}3=S_h.}
$$

The leading $h^2$ errors cancel, leaving $S_h=I+O(h^4)$. The identity of the [numerical integration](../../../../numerical-integration-split.md) weights is exact; the error-order conclusion additionally uses the smoothness and even-power error assumptions.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [P](../../p.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
