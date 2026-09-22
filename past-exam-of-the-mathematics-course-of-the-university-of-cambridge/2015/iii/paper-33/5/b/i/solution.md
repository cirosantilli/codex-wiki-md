<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md) is $\widehat S(t)=\prod_{t_j\leq t}(1-d_j/r_j)$, with event count $d_j$ and [risk set](../../../../../../../risk-set.md) size $r_j$. Its median is the first event time with estimated survival at most $1/2$. Since $\widehat S(2)=0.5749$ and $\widehat S(3)=0.4286$, **the estimated median completion time is $3$ minutes**.

The original last event exhausts the final [risk set](../../../../../../../risk-set.md), so the fitted [survival function](../../../../../../../survival-function.md) drops to zero at $18$ and its conventional full area is finite. Integrate the right-continuous step function: its height is one before time one, and after each event the height is the newly computed survival value. There are three-minute gaps from $12$ to $15$ and from $15$ to $18$. Thus

$$
\widehat\mu=1+\sum_{j=1}^{11}\widehat S(j)+3\widehat S(12)+3\widehat S(15)
\simeq\boxed{4.188\text{ minutes}.}
$$

Using the exact risk-set products rather than rounded printed survival values gives $4.187856$. This is not the sample mean of the observed event-or-censoring times; [right censoring](../../../../../../../right-censoring.md) changes the estimated survival weights.

If the final observation at $18$ is instead censored, every earlier [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md) value is unchanged and no event factor is inserted at $18$. The median remains **$3$ minutes**, but the curve stays at $\widehat S(15)\simeq0.0107$ at the end of follow-up. By [terminal censoring and survival-mean identifiability](../../../../../../../terminal-censoring-and-survival-mean-identifiability.md), **a full unrestricted mean is no longer determined nonparametrically by these observations**. Extending the final positive step forever would give an infinite integral, but that plotting convention does not establish an infinite population mean. Extra assumptions about the unobserved tail would be needed for a finite full-mean estimate.

The [restricted mean survival time](../../../../../../../restricted-mean-survival-time.md) through $18$ is still **$4.187856$ minutes** in either version: the two curves differ only at or after the endpoint, which does not affect the area up to it. All these interpretations require [independent censoring](../../../../../../../independent-censoring.md). Giving up may be related to how long a person would have taken to finish, so that assumption needs scientific justification in this study.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
