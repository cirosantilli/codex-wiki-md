<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

For a parametrized [curve](../../../../../curve.md) on the surface, the [energy of a curve](../../../../../energy-of-a-curve.md) is

$$
\mathcal E(\gamma)=\frac12\int_a^b|\dot\gamma(t)|^2\,dt=\frac12\int_a^b\left(E\dot u^2+2F\dot u\dot v+G\dot v^2\right)\,dt,
$$

where the [first fundamental form](../../../../../first-fundamental-form.md) coefficients are evaluated at $(u(t),v(t))$. A [fixed-endpoint variation of a curve](../../../../../fixed-endpoint-variation-of-a-curve.md) has coordinate variation fields $\eta,\xi$ vanishing at $a,b$. Differentiating under the integral and integrating their derivative terms by parts gives

$$
\delta\mathcal E=\int_a^b\!\left[\left(\frac{E_u\dot u^2+2F_u\dot u\dot v+G_u\dot v^2}{2}-\frac d{dt}(E\dot u+F\dot v)\right)\eta+\left(\frac{E_v\dot u^2+2F_v\dot u\dot v+G_v\dot v^2}{2}-\frac d{dt}(F\dot u+G\dot v)\right)\xi\right]dt.
$$

The fields can be chosen independently with compact support in $(a,b)$. Stationarity and the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore force both coefficients to vanish. These [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are the [geodesic equations](../../../../../geodesic-equation.md):

$$
\boxed{\frac d{dt}(E\dot u+F\dot v)=\frac12(E_u\dot u^2+2F_u\dot u\dot v+G_u\dot v^2),\qquad\frac d{dt}(F\dot u+G\dot v)=\frac12(E_v\dot u^2+2F_v\dot u\dot v+G_v\dot v^2).}
$$

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
