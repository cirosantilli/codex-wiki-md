<h1 id="19/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $x\ne0$, induction gives

$$
f^{(n)}(x)=P_n(1/x)e^{-1/x^2},\qquad
P_0(t)=1,\qquad P_{n+1}(t)=2t^3P_n(t)-t^2P_n'(t),
$$

where each $P_n$ is a [polynomial](../../../../../../polynomial-split.md). This recurrence follows from the [product rule](../../../../../../product-rule.md) and $d(1/x)/dx=-1/x^2$. Since [Gaussian decay dominates every power](../../../../../../gaussian-decay-dominates-every-power.md),

$$
\boxed{\lim_{x\to0}f^{(n)}(x)=0\quad\text{for every integer }n\geq0.}
$$

These limits also describe the [derivatives](../../../../../../derivative.md) of the extension at zero. If $f^{(n)}(0)=0$, its next [difference quotient](../../../../../../difference-quotient.md) is $P_n(1/h)e^{-1/h^2}/h$, which again tends to zero. Induction proves existence and [continuity](../../../../../../continuous-function.md) of every [derivative](../../../../../../derivative.md), all zero there. This is a [flat function](../../../../../../flat-function.md), covered more generally by [polynomial multiples of a Gaussian flat function](../../../../../../polynomial-multiples-of-a-gaussian-flat-function.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [19](../../../19.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
