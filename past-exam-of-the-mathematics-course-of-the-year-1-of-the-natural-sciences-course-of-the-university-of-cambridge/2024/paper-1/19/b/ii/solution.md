<h1 id="19/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The bound $|\cos(1/x)|\leq1$ gives $|f(x)-f(0)|\leq|x|^p$ when $x\ne0$. If $p>0$, given any $\varepsilon>0$, choose $\delta=\varepsilon^{1/p}$. Then $0<|x|<\delta$ implies

$$
|f(x)-f(0)|\leq|x|^p<\delta^p=\varepsilon;
$$

the inequality also holds at $x=0$. This proves [continuity](../../../../../../continuous-function.md) using the [epsilon-delta definition of continuity](../../../../../../epsilon-delta-definition-of-continuity.md).

For necessity, take the positive [sequence](../../../../../../sequence.md) $x_n=1/(2\pi n)\to0$. Then $\cos(1/x_n)=1$, so $f(x_n)=(2\pi n)^{-p}$. For $p=0$ this equals $1$; for $p<0$ it tends to $+\infty$. In neither case does it tend to $f(0)=0$, so [continuity](../../../../../../continuous-function.md) fails. Consequently

$$
\boxed{f\text{ is continuous at }0\iff p>0.}
$$

This is an instance of the general [continuity and differentiability thresholds for a damped oscillation](../../../../../../continuity-and-differentiability-thresholds-for-a-damped-oscillation.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [19](../../../19.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
