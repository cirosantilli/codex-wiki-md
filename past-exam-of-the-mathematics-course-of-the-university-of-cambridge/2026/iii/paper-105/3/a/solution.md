<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic flow map](../../../../../../characteristic-flow-map.md) solves the [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\frac{d}{dt}Z_{s,t}(x)=Z_{s,t}(x),
\qquad
Z_{s,s}(x)=x,
$$

and hence

$$
Z_{s,t}(x)=e^{t-s}x.
$$

Along this [characteristic curve](../../../../../../characteristic-curve.md), the [chain rule](../../../../../../chain-rule.md) gives

$$
\frac d{dt}u(t,Z_{s,t}(x))
=u_t+Z_{s,t}(x)u_x=0.
$$

The value is therefore constant, and tracing $(t,x)$ back to time zero gives the [classical solution](../../../../../../classical-solution.md)

$$
u(t,x)=u_0(e^{-t}x).
$$

Direct differentiation verifies both the [linear transport equation](../../../../../../linear-transport-equation.md) and its initial value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
