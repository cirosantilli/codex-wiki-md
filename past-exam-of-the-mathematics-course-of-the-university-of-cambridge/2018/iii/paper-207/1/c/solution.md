<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the frozen-age [exponential distribution](../../../../../../exponential-distribution.md) convention, the mean waiting time is the reciprocal of the outgoing [transition intensity](../../../../../../transition-intensity.md). The beliefs therefore specify

$$
q_{12}(50)=\frac1{10},\quad q_{12}(60)=\frac15,\qquad
q_{23}(50)=\frac12,\quad q_{23}(60)=1.
$$

Both rates double over ten years. Consequently

$$
\boxed{a=0.1\ \text{year}^{-1},\qquad b=0.5\ \text{year}^{-1},\qquad
\beta_{12}=\beta_{23}=\frac{\log2}{10}\ \text{year}^{-1}.}
$$

These calibrate the age-specific constant-rate means; they are not exact mean ages of future events when age-dependent rates continue increasing throughout the waiting time.

For a literal continuously ageing interpretation, a rate $q e^{\beta u}$ gives a [Gompertz distribution](../../../../../../gompertz-distribution.md) for the waiting time. For $\beta>0$, its mean is

$$
m(q,\beta)=\int_0^\infty\exp\!\left[-\frac q\beta(e^{\beta u}-1)\right]du
=\frac{e^{q/\beta}}\beta E_1(q/\beta),\qquad
E_1(z)=\int_z^\infty\frac{e^{-v}}v\,dv.
$$

Here $E_1$ is the [exponential integral](../../../../../../exponential-integral.md). Solving $m(a,\beta_{12})=10$ and $m(ae^{10\beta_{12}},\beta_{12})=5$, and the analogous pair with means 2 and 1, instead gives

$$
(a,\beta_{12})\approx(0.0391767,0.1136031),\qquad
(b,\beta_{23})\approx(0.4328981,0.0763367),
$$

with rates and slopes in inverse years. These are an alternative continuous-age calibration, not the frozen-age answer boxed above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
