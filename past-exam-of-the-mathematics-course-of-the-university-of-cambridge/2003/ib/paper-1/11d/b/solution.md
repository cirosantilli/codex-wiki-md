<h1 id="11d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First use a homogeneous solution to meet the nonzero endpoint values:

$$
y_h(x)=\frac{a\sin(k(\pi-x))+b\sin(kx)}{\sin(k\pi)}.
$$

It satisfies $y_h''+k^2y_h=0$, $y_h(0)=a$ and $y_h(\pi)=b$. The [Green-function representation](../../../../../../green-function-representation.md) then gives

$$
\boxed{y(x)=\frac{a\sin(k(\pi-x))+b\sin(kx)}{\sin(k\pi)}+\int_0^\pi G(x,\xi)f(\xi)\,d\xi.}
$$

Applying the differential operator to the integral gives $f(x)$ by the defining [Dirac delta](../../../../../../dirac-delta-function.md) property of $G$, and that integral vanishes at the endpoints. For continuous $f$ this is a classical solution; integrable $f$ also gives the corresponding weak solution. The same nonresonant homogeneous argument as in part (a) proves uniqueness.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
