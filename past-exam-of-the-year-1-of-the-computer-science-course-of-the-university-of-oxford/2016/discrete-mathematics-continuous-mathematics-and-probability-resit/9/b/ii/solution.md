<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reversing sign reverses the inequality. Since $X$ has a [probability density function](../../../../../../probability-density-function.md), it has no point masses, so

$$
F_Y(y)=\mathbb P(X\geq-y)=1-\mathbb P(X<-y)=\boxed{1-F_X(-y)}.
$$

Differentiating the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) gives

$$
\boxed{f_Y(y)=f_X(-y)}
$$

almost everywhere: the minus sign outside $F_X$ cancels the minus sign from the [chain rule](../../../../../../chain-rule.md). If point masses were allowed, the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) would instead require the left limit $1-F_X((-y)^-)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
