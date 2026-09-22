<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

For $z=x+iy\in\mathbb H$, direct calculation gives

$$
|f(z)|^2=\frac{x^2+(y-1)^2}{x^2+(y+1)^2}<1.
$$

Conversely, solving $w=(z-i)/(z+i)$ gives

$$
z=i\frac{1+w}{1-w},\qquad\operatorname{Im}z=\frac{1-|w|^2}{|1-w|^2}>0\quad(|w|<1).
$$

The denominator cannot vanish inside the [unit disc](../../../../../unit-disc.md), so these inverse formulas prove $\boxed{f(\mathbb H)=\mathbb D}$. This is the [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md).

For $z\in U$, we also require $|z|>1$. In inverse coordinates this becomes

$$
\frac{|1+w|}{|1-w|}>1\ \Longleftrightarrow\ |1+w|^2-|1-w|^2=4\operatorname{Re}w>0.
$$

The equivalence holds in both directions, so

$$
\boxed{f(U)=\{w\in\mathbb C:|w|<1,\ \operatorname{Re}w>0\}}.
$$

Thus the exterior of the unit semicircle maps to the right half of the [unit disc](../../../../../unit-disc.md). The circular arc maps to its imaginary diameter, which is excluded because the source inequality is strict.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [6](../../../6.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
