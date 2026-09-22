<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $\theta>0$, the [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\frac{\sqrt n(\overline X-\theta)}{\sqrt\theta}\ \xrightarrow{d}\ N(0,1).
$$

The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $\overline X\to\theta$, so [Slutsky theorem](../../../../../../slutsky-theorem.md) permits replacing $\theta$ in the standard error by $\overline X$. With $z=z_{0.025}\approx1.96$, an approximate 95% [confidence interval](../../../../../../confidence-interval.md) is

$$
\boxed{\left[\overline X-z\sqrt{\frac{\overline X}{n}},\quad
\overline X+z\sqrt{\frac{\overline X}{n}}\right].}
$$

The lower endpoint may be truncated at zero because the parameter is nonnegative. This is a large-sample normal approximation for fixed positive $\theta$; an all-zero or very sparse sample does not justify the plug-in normal approximation. At the degenerate parameter value zero, every observation is zero almost surely.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
