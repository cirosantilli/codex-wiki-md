<h1 id="m/m4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $a,b>0$, the [standard deviations](../../../../../../standard-deviation.md). Substitute the two [normal densities](../../../../../../normal-density.md) into (ii):

$$
f_V(v)=\frac1{\pi ab}\int_0^\infty u\exp\left[-\frac{u^2}2\left(\frac1{a^2}+\frac{v^2}{b^2}\right)\right]du=\frac{ab}{\pi(b^2+a^2v^2)}.
$$

The last step uses $\int_0^\infty ue^{-Au^2/2}du=1/A$. With $c=b/a$ this is $\boxed{f_V(v)=c/[\pi(c^2+v^2)]}$, the centered [Cauchy](../../../../../../cauchy-sequence.md) [density](../../../../../../probability-density-function.md) of scale $c$.

The desired event is $|V|<1$, outside the null event $X=0$. Integrating the [density](../../../../../../probability-density-function.md) gives

$$
\boxed{P(|Y|<|X|)=\frac2\pi\arctan(1/c)=\frac2\pi\arctan(a/b).}
$$

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [M4](../../../m4.md)
4. [M](../../../../m.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
