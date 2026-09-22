<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $d=1/\sqrt2$. At the positive real endpoint the contour is real and crosses the [saddle point](../../../../../../../saddle-point.md) at zero. The [Gaussian integral](../../../../../../../gaussian-integral.md) gives

$$
f(0,\lambda)=\sqrt{\frac\pi\lambda}-\int_d^\infty e^{-\lambda x^2}dx-\int_1^\infty e^{-\lambda x^2}dx\sim\boxed{\sqrt{\frac\pi\lambda}}.
$$

Both omitted tails are exponentially small. At the negative real endpoint the contour is oriented leftward and does not cross the [saddle point](../../../../../../../saddle-point.md):

$$
f(\pi,\lambda)=-\int_d^1e^{-\lambda x^2}dx.
$$

The [endpoint contribution in steepest descent](../../../../../../../endpoint-contribution-in-steepest-descent.md), or one [integration by parts](../../../../../../../integration-by-parts.md), gives $\int_d^\infty e^{-\lambda x^2}dx\sim e^{-\lambda d^2}/(2\lambda d)$. The upper-end correction is $O(e^{-\lambda}/\lambda)$ and is much smaller. Therefore

$$
\boxed{f(\pi,\lambda)\sim-\frac{e^{-\lambda/2}}{\sqrt2\,\lambda}.}
$$

The sign comes from contour orientation, not from a different Gaussian convention.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
