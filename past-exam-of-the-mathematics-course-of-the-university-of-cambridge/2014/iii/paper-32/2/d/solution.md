<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [mean holding time from a transition intensity matrix](../../../../../../mean-holding-time-from-a-transition-intensity-matrix.md) is $-1/q_{rr}$. Apply this to the fitted exit rates and use monotonic inversion for each [confidence interval](../../../../../../confidence-interval.md):

$$
\begin{aligned}
\text{mild: }&\frac1{0.0115}=86.96\text{ months},&\quad95\%\text{ CI }&=\left[\frac1{0.0130},\frac1{0.0102}\right]=[76.92,98.04],\\
\text{severe: }&\frac1{0.0318}=31.45\text{ months},&95\%\text{ CI }&=\left[\frac1{0.0352},\frac1{0.0287}\right]=[28.41,34.84].
\end{aligned}
$$

Thus the expected state durations are **86.96 months** and **31.45 months**, respectively. A [confidence interval for a reciprocal rate](../../../../../../confidence-interval-for-a-reciprocal-rate.md) reverses the endpoint order; the negative diagonal rates must first be converted to positive exit rates.

For the [expected absorption time in an illness-death model](../../../../../../expected-absorption-time-in-an-illness-death-model.md), the time spent initially in the mild state is followed by an additional severe-state duration only if progression occurs before death. That [probability](../../../../../../probability.md) is $0.0072/0.0115$. Therefore

$$
\boxed{E_1(T_{\mathrm{death}})=\frac1{0.0115}+\frac{0.0072}{0.0115}\frac1{0.0318}=106.64\text{ months}\approx8.89\text{ years}.}
$$

This is an unconditional mean including both possible paths to death, not a mean conditional on progression.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
