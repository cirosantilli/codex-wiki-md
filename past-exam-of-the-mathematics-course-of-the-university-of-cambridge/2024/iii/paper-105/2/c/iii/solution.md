<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiply the differential equation by $v\in H$ and integrate. The [Hardy inequality on an interval](../../../../../../../hardy-inequality-on-an-interval.md) makes the terms containing $u/x$ and $v/x$ integrable. For smooth $v$, [integration by parts](../../../../../../../integration-by-parts.md) gives

$$
-\int_0^1u''v
=\int_0^1u'v'-[u'v]_0^1
=\int_0^1u'v',
$$

because $v(0)=0$ and the [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) is $u'(1)=0$. Therefore

$$
\boxed{
\int_0^1u'v'
+\int_0^1\frac{uv}{x^2}
-\int_0^1u'v
=\int_0^1\frac{fv}{x^2}.}
$$

The [density of smooth functions in a Sobolev space](../../../../../../../density-of-smooth-functions-in-a-sobolev-space.md) and continuity of all four terms extend this [weak formulation](../../../../../../../weak-formulation.md) to every $v\in H$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
