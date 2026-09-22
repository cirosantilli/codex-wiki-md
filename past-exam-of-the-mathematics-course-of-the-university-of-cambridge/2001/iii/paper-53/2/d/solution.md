<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the local [Taylor series](../../../../../../taylor-series.md) at the [critical point](../../../../../../critical-point.md) as

$$
g(x)=1+c x^d+O(x^{d+2}),\qquad c<0,
$$

where $d$ is even, and put $a=g(1)$. The fixed-point equation first gives $g(g(0))=g(1)=a$, consistently with normalization. Expanding the inner function at zero and the outer one at one,

$$
g(ax)=1+c a^d x^d+O(x^{d+2}),
$$



$$
a^{-1}g(g(ax))=1+c a^{d-1}g'(1)x^d+O(x^{d+2}).
$$

The quadratic remainder in the outer expansion is of order $x^{2d}$, at least $x^{d+2}$ because $d\geq2$. Comparing the nonzero $x^d$ coefficients proves the exact identity

$$
\boxed{a^{d-1}g'(1)=1.}
$$

To obtain the requested first-order relation, use the [leading polynomial approximation to a renormalization fixed point](../../../../../../leading-polynomial-approximation-to-a-renormalization-fixed-point.md): retain only $g(x)\approx1+c x^d$. Then $a\approx1+c$, while $g'(1)\approx dc$, giving the truncated equation

$$
\boxed{d(a-1)a^{d-1}=1\quad\text{in the first-order polynomial approximation}.}
$$

The equality belongs to this truncation; higher analytic coefficients generally change $g'(1)$ and $a$, so it is not an additional exact equation for the full [fixed point](../../../../../../fixed-point.md).

For $d=2$, solve $2a(a-1)=1$. The root compatible with $-1<a<0$ is $a=(1-\sqrt3)/2$; the other root is inadmissible. Thus

$$
\boxed{g(x)\approx1-\frac{1+\sqrt3}{2}x^2,\qquad
\alpha\approx-\frac1a=1+\sqrt3\simeq2.73205.}
$$

This is a coarse leading approximation, not the more accurate universal value $2.5029\ldots$ obtained after retaining higher coefficients.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
