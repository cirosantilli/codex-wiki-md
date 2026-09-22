<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $Z=\int_a^\infty x^{\alpha-1}e^{-\beta x}\,dx$. A proper target requires $\beta>0$, and a proper proposal requires $b>0$. Normalization gives $f(x)=x^{\alpha-1}e^{-\beta x}/Z$ and the [Pareto distribution](../../../../../../../pareto-distribution.md) proposal $g(x)=ba^b x^{-b-1}$ on $x>a$. Their ratio is

$$
\frac{f(x)}{g(x)}=\frac{x^{\alpha+b}e^{-\beta x}}{ba^bZ}.
$$

The derivative of its logarithm is $(\alpha+b)/x-\beta$. It is positive before $x_*=(\alpha+b)/\beta$ and negative after it. Since $a<\alpha/\beta<x_*$, the maximum occurs within the proposal support. Consequently the tight envelope for [truncated gamma rejection sampling with a Pareto envelope](../../../../../../../truncated-gamma-rejection-sampling-with-a-pareto-envelope.md) is

$$
\boxed{M=\left(\frac{\alpha+b}{\beta}\right)^{\alpha+b}e^{-(\alpha+b)}\left(ba^b\int_a^\infty x^{\alpha-1}e^{-\beta x}\,dx\right)^{-1}.}
$$

The accompanying acceptance rule can be evaluated without $Z$:

$$
\frac{f(x)}{Mg(x)}=\left(\frac{x}{x_*}\right)^{\alpha+b}\exp[-\beta(x-x_*)]\le1.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
