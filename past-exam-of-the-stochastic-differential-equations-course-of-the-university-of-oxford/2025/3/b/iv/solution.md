<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Since $X_0=0$, its [supremum](../../../../../supremum.md) $X^\star$ is nonnegative. For $b>0$, continuity gives

$$
\{X^\star>b\}=\bigcup_{n\geq1}\{T_{b+1/n}<\infty\}.
$$

The events increase with $n$. Part (iii) therefore yields $\mathbb P(X^\star>b)=\lim_ne^{-(b+1/n)}=e^{-b}$. Letting $b\downarrow0$ gives $\mathbb P(X^\star>0)=1$; letting $b\to\infty$ gives finiteness [almost surely](../../../../../almost-sure-convergence.md). Consequently

$$
\boxed{X^\star\sim\operatorname{Exp}(1),\qquad
\mathbb P(X^\star\leq x)=
\begin{cases}0,&x<0,\\1-e^{-x},&x\geq0.\end{cases}}
$$

Its [probability density function](../../../../../probability-density-function.md) is $e^{-x}\mathbf1_{\{x>0\}}$, with no atom at zero. Using strict exceedances above also avoids presupposing that the infinite-horizon [supremum](../../../../../supremum.md) is attained.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
