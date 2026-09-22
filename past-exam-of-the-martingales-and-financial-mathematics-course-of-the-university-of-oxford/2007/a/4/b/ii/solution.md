<h1 id="a/4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $C$ be the event that the sample averages have a limit in the [extended real number line](../../../../../../extended-real-number-line.md). It is measurable: the bounded sequence $\arctan S_n$ converges exactly when it is Cauchy, and the Cauchy condition is a countable combination of measurable inequalities. Limits at $\pm\pi/2$ correspond to extended limits $\pm\infty$.

For each fixed $m$, remove the first $m-1$ terms and set

$$
S_n^{(m)}=\frac1n\sum_{k=m}^nX_k\quad(n\geq m).
$$

The difference $S_n-S_n^{(m)}=n^{-1}\sum_{k<m}X_k$ tends to zero for every outcome, since the finitely many variables are real-valued. Thus these two sequences have an extended limit simultaneously. Equivalently their arctangents differ by a quantity tending to zero, because arctangent is Lipschitz. The event $C$ is therefore expressible using $X_m,X_{m+1},\ldots$ alone. Since this holds for every $m$, $C\in\mathcal T$.

Kolmogorov's law gives $\mathbb P(C)=0$ or one. In the latter case the measurable extended variable $\limsup S_n$, redefined on a [null set](../../../../../../null-set.md) if needed, is the [almost sure convergence](../../../../../../almost-sure-convergence.md). In the former there is almost surely no extended-real limit. Hence **extended convergence occurs almost surely, or divergence occurs almost surely**. The law need not make the value of a possible limit finite.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
