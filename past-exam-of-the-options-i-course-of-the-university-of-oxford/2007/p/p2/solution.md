<h1 id="p/p2/solution">Solution</h1>

↑ **Parent:** [P2](../p2.md)

[Richardson extrapolation](../../../../richardson-extrapolation.md) cancels a leading discretization error by combining two mesh sizes. If $A(h)=I+ch^p+O(h^q)$ with $q>p$, then

$$
\frac{2^pA(h/2)-A(h)}{2^p-1}=I+O(h^q).
$$

Use a uniform grid $x_i=a+ih$, $0\le i\le n$, with even $n$. The composite trapezium rule is

$$
T_h=h\left[\frac{f_0+f_n}{2}+\sum_{i=1}^{n-1}f_i\right],\qquad f_i=f(x_i).
$$

The composite Simpson rule, formed by integrating a quadratic interpolant on each pair of successive panels, is

$$
S_h=\frac h3\left[f_0+f_n+4\sum_{i\text{ odd}}f_i+2\sum_{\substack{0<i<n\\i\text{ even}}}f_i\right].
$$

Assume an even-power trapezium error expansion $T_h=I+c_2h^2+O(h^4)$; continuous fourth derivative is a standard sufficient smoothness hypothesis. The coarse grid has step $2h$, so one extrapolation step is $(4T_h-T_{2h})/3$. Its endpoint coefficients are $h/3$, its odd-index coefficients are $4h/3$, and its interior even-index coefficients are $2h/3$. Therefore

$$
\boxed{S_h=\frac{4T_h-T_{2h}}3=I+O(h^4)}.
$$

The algebraic identity between the two rules holds for any sampled values; the smoothness and error assumptions are used to infer the improved accuracy.

## ↑ Ancestors (12)

1. [P2](../p2.md)
2. [P](../../p.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
