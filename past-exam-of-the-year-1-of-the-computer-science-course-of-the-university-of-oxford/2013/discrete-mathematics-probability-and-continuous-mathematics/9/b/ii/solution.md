<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $W=U^2$. On $0\leq U\leq1$, squaring preserves order. Therefore for $0\leq w\leq1$,

$$
F_W(w)=\mathbb P(U^2\leq w)=\mathbb P(U\leq\sqrt w)=\sqrt w.
$$

Including the tails gives the [cumulative distribution function](../../../../../../cumulative-distribution-function.md)

$$
\boxed{F_W(w)=\begin{cases}0&w<0,\\\sqrt w&0\leq w\leq1,\\1&w>1.\end{cases}}
$$

Differentiating on the interior of the support gives the [probability density function](../../../../../../probability-density-function.md)

$$
\boxed{f_W(w)=\begin{cases}\dfrac1{2\sqrt w}&0<w<1,\\0&\text{otherwise}.\end{cases}}
$$

The divergence near zero is integrable: $\int_0^1(2\sqrt w)^{-1}\,dw=1$. There is no point mass at zero, and the assigned value of a [probability density function](../../../../../../probability-density-function.md) at a single endpoint does not affect the [probability distribution](../../../../../../probability-distribution-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
