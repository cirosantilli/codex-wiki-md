<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the upper half-disc of radius $R$, with a clockwise semicircular indentation of radius $\varepsilon$ above zero. The integrand is [holomorphic](../../../../../holomorphic-function-split.md) inside that indented contour, so its total integral is zero. On the large arc,

$$
f(z)=\frac{e^{i(a+b)z}-e^{i(a-b)z}}{2iz^2},\qquad |f(z)|\leq R^{-2},
$$

because $a+b>0$, $a-b>0$ and $\operatorname{Im}z\geq0$. Its integral has modulus at most $\pi/R$ and vanishes as $R\to\infty$.

On the small clockwise arc, $f(z)=b/z+O(1)$, so the integral tends to $-i\pi b$. Therefore the remaining real-axis integral satisfies

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{iax}\sin(bx)}{x^2}\,dx=i\pi b.
$$

The [imaginary part](../../../../../imaginary-part.md) is [even](../../../../../even-function.md) and is an ordinary [absolutely convergent integral](../../../../../absolutely-convergent-improper-integral.md): near zero its integrand tends to $ab$, and at infinity it is $O(x^{-2})$. Taking imaginary parts gives

$$
2\int_0^\infty\frac{\sin(ax)\sin(bx)}{x^2}\,dx=\pi b,\qquad\boxed{\int_0^\infty\frac{\sin(ax)\sin(bx)}{x^2}\,dx=\frac{\pi b}{2}.}
$$

The complex integral needs the [Cauchy principal value](../../../../../cauchy-principal-value.md) because its [real part](../../../../../real-part.md) has a $b/x$ [singularity](../../../../../complex-singularity.md); the requested sine-product integral does not. This [sine-product integral with inverse-square weight](../../../../../sine-product-integral-with-inverse-square-weight.md) is an application of the [upper-half-plane indentation rule](../../../../../upper-half-plane-indentation-rule.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
