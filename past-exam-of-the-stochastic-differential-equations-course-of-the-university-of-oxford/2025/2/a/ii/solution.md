<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Y_t=-\beta\int_0^tB_u\,dB_u-\int_0^th_u\,du$. Its [quadratic variation](../../../../../quadratic-variation.md) is $[Y]_t=\beta^2\int_0^tB_u^2du$. The [Itô formula](../../../../../ito-s-lemma.md) for $Z=e^Y$ gives

$$
dZ_t=-\beta Z_tB_t\,dB_t
+Z_t\left(\frac{\beta^2}{2}B_t^2-h_t\right)dt.
$$

Choose

$$
\boxed{h_t=\frac{\beta^2}{2}B_t^2,\qquad dZ_t=-\beta B_tZ_t\,dB_t,\quad Z_0=1.}
$$

The chosen process is continuous and [adapted](../../../../../adapted-process.md), hence [progressively measurable](../../../../../progressive-measurability.md). Its time integral is finite on compact intervals because Brownian paths are continuous. The resulting $Z$ is the [stochastic exponential](../../../../../doleans-dade-exponential.md) of $-\beta\int_0^\cdot B_u\,dB_u$, and is a positive [local martingale](../../../../../local-martingale.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
