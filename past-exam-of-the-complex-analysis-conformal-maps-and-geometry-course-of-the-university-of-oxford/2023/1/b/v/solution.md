<h1 id="1/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use $h(\sqrt r\,e^{i\theta})^2=\phi(re^{2i\theta})$. As $\theta$ runs around the circle, the doubled angle goes around it twice, so [iv](../iv.md) gives

$$
\boxed{\frac1{2\pi}\int_0^{2\pi}|\phi(re^{i\theta})|d\theta=M(\sqrt r)\leq\frac r{1-r}}.
$$

The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) for the [Taylor coefficients](../../../../../taylor-coefficient.md) now implies

$$
|a_n|\leq\frac1{2\pi r^n}\int_0^{2\pi}|\phi(re^{i\theta})|d\theta\leq\frac{r^{1-n}}{1-r}.
$$

For $n\geq2$, choosing $r=(n-1)/n$ gives the [linear coefficient bound for normalized univalent functions](../../../../../linear-coefficient-bound-for-normalized-univalent-functions.md),

$$
\boxed{|a_n|\leq n\left(1+\frac1{n-1}\right)^{n-1}\leq ne}.
$$

The last inequality follows from $\log(1+x)\leq x$ for $x>-1$.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../../split.md)
6. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
