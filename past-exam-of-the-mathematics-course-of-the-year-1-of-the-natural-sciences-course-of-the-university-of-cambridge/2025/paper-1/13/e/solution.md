<h1 id="13/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [tangent half-angle substitution](../../../../../tangent-half-angle-substitution.md) $t=\tan(x/2)$, so $\cos x=(1-t^2)/(1+t^2)$ and $dx=2\,dt/(1+t^2)$. Then

$$
\int\frac{dx}{5+3\cos x}=\int\frac{2\,dt}{5(1+t^2)+3(1-t^2)}=\int\frac{dt}{t^2+4}.
$$

The [inverse tangent](../../../../../inverse-tangent.md) [antiderivative](../../../../../antiderivative.md) gives

$$
\boxed{\frac12\arctan\left(\frac12\tan\frac x2\right)+C.}
$$

This expression applies on each [interval](../../../../../interval-mathematics.md) $( (2j-1)\pi,(2j+1)\pi)$ for an integer $j$. Although $5+3\cos x\geq2$ everywhere, the chosen [inverse tangent](../../../../../inverse-tangent.md) expression jumps at the endpoints because the substitution has a pole there. A global continuous [antiderivative](../../../../../antiderivative.md) is obtained by adding $j\pi/2$ on that [interval](../../../../../interval-mathematics.md), using one common $C$, and extending by [continuity](../../../../../continuous-function.md) at the endpoints.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
