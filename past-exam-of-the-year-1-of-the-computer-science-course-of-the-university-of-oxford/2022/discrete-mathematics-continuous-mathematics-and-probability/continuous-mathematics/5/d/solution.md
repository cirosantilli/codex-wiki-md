<h1 id="continuous-mathematics/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the computed function values as $f(x\pm h)+e_\pm$, where $|e_\pm|\le\delta$. The computed [central finite difference](../../../../../../central-finite-difference.md) $\widetilde d$ satisfies

$$
\boxed{|\widetilde d-d|=\left|\frac{e_+-e_-}{2h}\right|\le\frac\delta h,\qquad |\widetilde d-f'(x)|\le\frac{h^2}{6}+\frac\delta h.}
$$

The two contributions are respectively evaluation [absolute error](../../../../../../absolute-error.md) and [truncation error](../../../../../../truncation-error.md). For $\delta>0$, [step-size choice for a noisy central derivative](../../../../../../step-size-choice-for-a-noisy-central-derivative.md) minimizes their sum: its [derivative](../../../../../../derivative.md) is $h/3-\delta/h^2$, negative before and positive after

$$
\boxed{h=(3\delta)^{1/3},\qquad \min_{h>0}\left(\frac{h^2}{6}+\frac\delta h\right)=\frac{(3\delta)^{2/3}}2.}
$$

If $\delta=0$, the bound tends to zero as $h\downarrow0$ and has no positive minimizing step.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [Continuous mathematics](../../../continuous-mathematics.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
