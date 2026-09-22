<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $P(z)=1/(2\sqrt\pi z^{1/4})$, choose a consistent branch, and truncate the corrected series after $r=n-1$, with $n=|\sigma|+O(1)$. The leading factorial tail in part (iii) is represented by the same indented integral as in part (ii):

$$
R_n\sim\frac{P(z)e^{\sigma/2}}{2\pi}\sum_{r=n}^{\infty}\frac{\Gamma(r)}{\sigma^r}
\quad\longleftrightarrow\quad
\frac{P(z)e^{-\sigma/2}}{2\pi}I(\sigma,n).
$$

Here the divergent sum means its lateral [Borel summation](../../../../../../borel-summation.md), not ordinary summation. To see why the [pole](../../../../../../pole.md) approximation controls this remainder, write $a_r=\sigma^rY_r$ and insert $\Gamma(r)=\int_0^\infty e^{-v}v^{r-1}dv$ in the leading late terms. Summing the geometric tail creates $1/(1-v/\sigma)$; $v=\sigma t$ produces $I(\sigma,n)$. The relative $O(r^{-1})$ corrections to the late coefficients give lower-order contributions on its saddle scale. More concretely, the [Borel transform](../../../../../../borel-transform-of-a-factorially-divergent-series.md) of the coefficient series is

$$
\sum_{r=1}^\infty\frac{a_r t^{r-1}}{\Gamma(r)}
=\frac d{dt}\,{}_2F_1\left(\frac16,\frac56;1;t\right)
=\frac1{2\pi(1-t)}+O(\log(1-t))\quad(t\to1).
$$

The [simple pole](../../../../../../simple-pole.md) supplies the leading [Stokes phenomenon](../../../../../../stokes-phenomenon.md); its weaker [logarithmic singularity](../../../../../../logarithmic-singularity.md) supplies the smaller corrections. This is the integral justification for retaining the factorial tail.

For $\arg\sigma=\phi/\sqrt{|\sigma|}$, expand $\sigma=n+i\phi\sqrt n+O(1)$. Part (i), with $\mu=\phi$, now gives

$$
\boxed{R_n\sim\frac{i e^{-\sigma/2}}{4\sqrt\pi z^{1/4}}
\left[1+\operatorname{erf}\left(\frac\phi{\sqrt2}\right)\right]}.
$$

This formula uses the upper-pole prescription and the upper [Airy function](../../../../../../airy-function.md) switching ray: near $\arg z=2\pi/3$, take $\arg\sigma=3\arg z/2-\pi$ near zero. The coefficient of the subdominant exponential changes smoothly from zero to $i$ across this ray and has value $i/2$ on it. The angular transition width is $O(|\sigma|^{-1/2})=O(|z|^{-3/4})$. The conjugate lower ray has the conjugate contour sign, rather than the same $+i$ on both rays. This is [error-function smoothing of a Stokes multiplier](../../../../../../error-function-smoothing-of-a-stokes-multiplier.md), not a discontinuity of the analytic [Airy function](../../../../../../airy-function.md). With the literal printed $r=1$ series, the missing $P(z)e^{\sigma/2}$ would invalidate this remainder formula.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
