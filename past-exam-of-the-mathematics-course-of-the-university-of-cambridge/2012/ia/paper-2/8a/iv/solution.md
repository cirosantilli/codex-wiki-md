<h1 id="8a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the [shift derivative of a step response](../../../../../../shift-derivative-of-a-step-response.md), writing $y_3(t,b)=H(s)K(s)$ with $s=t-b$. Differentiate with respect to the forcing location:

$$
-\frac{\partial y_3}{\partial b}=\delta(s)K(s)+H(s)K'(s).
$$

The possible delta term vanishes because $K(0)=0$, while $K'(s)=g(s)$. Therefore, as a distribution and also as the ordinary piecewise response,

$$
\boxed{-\frac{\partial y_3(t,b)}{\partial b}=H(t-b)g(t-b)=y_2(t,b)}.
$$

Moving the start of a unit step differentiates its forcing into a negative impulse. The zero initial conditions and [linearity](../../../../../../linearity.md) ensure that the corresponding responses obey the same identity, including the zero-frequency cases.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
