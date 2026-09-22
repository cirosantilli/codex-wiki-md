<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Statistician B uses the more appropriate analysis.** Its start–stop representation includes [left truncation](../../../../../../../left-truncation.md) as well as [right censoring](../../../../../../../right-censoring.md). Both entry and exit are ages since opening, so a business belongs to the [risk set](../../../../../../../risk-set.md) at age $t$ only when $\operatorname{ageatentry}<t\le\operatorname{obsage}$. The event indicator distinguishes closure from a censored end of observation. The counting-process representation does not mean that multiple closures per business have been observed.

Statistician A records only exit and status and treats every sampled business as at risk from opening. That incorrectly adds already-established businesses to [risk sets](../../../../../../../risk-set.md) at ages before they entered observation, ignoring their necessary survival to entry. Its first risk count is $60$, whereas B's is $25$. The extra non-events dilute early estimated closure hazards and here bias the estimated survival upward. Correcting [left truncation](../../../../../../../left-truncation.md) makes later [risk sets](../../../../../../../risk-set.md) capable of increasing as businesses enter at their respective ages.

For the [Kaplan–Meier estimator with delayed entry](../../../../../../../kaplan-meier-estimator-with-delayed-entry.md), at event ages $t_j$ with $d_j$ closures and $r_j$ businesses at risk,

$$
\widehat S(t)=\prod_{t_j\le t}\left(1-\frac{d_j}{r_j}\right),\qquad \widehat{\operatorname{se}}(\widehat S(t))=\widehat S(t)\left\{\sum_{t_j\le t}\frac{d_j}{r_j(r_j-d_j)}\right\}^{1/2}.
$$

The [standard error](../../../../../../../standard-error.md) follows from the [Greenwood formula](../../../../../../../greenwood-formula.md). Between event times this [survival function](../../../../../../../survival-function.md) estimate is constant. At age five the last preceding event is at $4.52$, and at age ten it is at $9.90$. Thus the requested estimates, including their precision, are

$$
\boxed{\widehat S(5)=0.462,\quad\operatorname{se}=0.0780,\quad95\%\ \operatorname{CI}=(0.332,0.643),}
$$

and

$$
\boxed{\widehat S(10)=0.280,\quad\operatorname{se}=0.0634,\quad95\%\ \operatorname{CI}=(0.180,0.436).}
$$

These correspond to estimated proportions 46.2% and 28.0%, not to the probability of surviving five or ten additional years conditional on being sampled at an arbitrary age. A's corresponding estimates $0.650$ and $0.407$ use the inappropriate [risk sets](../../../../../../../risk-set.md).

This interpretation assumes appropriately independent entry and censoring and a suitable common lifetime distribution across entry cohorts. A delayed-entry correction does not remove arbitrary informative sampling or calendar effects. More generally, if no observation covers the earliest ages, absolute survival from opening requires additional information about survival before the first observable age; the reported product-limit normalization is the one used in the supplied analysis.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 41](../../../../paper-41-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
