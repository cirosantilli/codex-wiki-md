<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now treat the seventh observation as an actual event at $t_4$, not as a censoring at that time. The [risk sets](../../../../../../risk-set.md) are $(7,6,5,4,2,1)$ and the event counts are $(1,1,1,2,1,1)$. The [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) therefore gives

$$
\boxed{\widehat F_5^0=\frac47\left(1-\frac24\right)\left(1-\frac12\right)=\frac17.}
$$

Conditional on reaching $t_4$, the two events at that time have total probability $2/4=1/2$. Surviving them has probability $1/2$, which is then divided equally between the remaining two event times. Thus

$$
\boxed{(\widehat p_4^0,\widehat p_5^0,\widehat p_6^0)=(1/2,1/4,1/4).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
