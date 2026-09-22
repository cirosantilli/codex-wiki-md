<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $b_n=4^{-n}\binom{2n}{n}$. The given limiting identity and the [Cauchy coefficient formula](../../../../cauchy-coefficient-formula.md) from part (a) give the boundary [contour integral](../../../../contour-integral.md)

$$
J_n:=\int_{\gamma(0,1)}\frac{dz}{z^{n+1}\sqrt{1-z}}=2\pi i b_n.
$$

The [contour](../../../../complex-integration-contour.md) passes through $z=1$, so its value here is an [improper integral](../../../../improper-integral.md) using the one-sided branch values. Parametrize its open arc by $z=e^{i\theta}$, $0<\theta<2\pi$. Substitution of the [analytic branch of a square root](../../../../analytic-branch-of-a-square-root.md) calculated in part (b) gives

$$
J_n=\frac{i}{1-i}\int_0^{2\pi}\frac{e^{-i(n+1/4)\theta}}{\sqrt{\sin(\theta/2)}}\,d\theta.
$$

The factor $e^{-in\theta}$ comes from cancelling $e^{i\theta}$ in $dz$ against $z^{n+1}$; the extra $e^{-i\theta/4}$ comes from the chosen branch. Keeping both phases prevents a change in the half-integer frequency.

Now put $t=\theta/2$. Then

$$
J_n=\frac{2i}{1-i}\int_0^\pi\frac{e^{-i(2n+1/2)t}}{\sqrt{\sin t}}\,dt=(i-1)\int_0^\pi\frac{e^{-i(2n+1/2)t}}{\sqrt{\sin t}}\,dt.
$$

Dividing by $i-1$ gives

$$
\int_0^\pi\frac{e^{-i(2n+1/2)t}}{\sqrt{\sin t}}\,dt=\frac{2\pi i b_n}{i-1}=\pi b_n(1-i).
$$

Taking the [real part](../../../../real-part.md) therefore proves

$$
\boxed{\int_0^\pi\frac{\cos\bigl((2n+\tfrac12)t\bigr)}{\sqrt{\sin t}}\,dt=\frac{\pi}{4^n}\binom{2n}{n},\qquad n=0,1,2,\ldots.}
$$

All these [improper integrals](../../../../improper-integral.md) converge absolutely: the numerators are bounded, while $(\sin t)^{-1/2}$ is of order $t^{-1/2}$ at zero and $(\pi-t)^{-1/2}$ at $\pi$. Hence the substitutions and passage to the [real part](../../../../real-part.md) are legitimate. The [imaginary part](../../../../imaginary-part.md) also shows that the corresponding sine [integral](../../../../integral-split.md) has the same positive value, which checks the phase calculation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
