<h1 id="5/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Take the event to mean three smoking-free weeks in succession, $Y_{i1}=Y_{i2}=Y_{i3}=1$. The initial cumulative count is zero. Along this path it equals $0,1,2$ in weeks one, two, three, respectively. In the [cumulative-response logistic model](../../../../../../../cumulative-response-logistic-model.md), define

$$
\pi_c=\frac{\exp(-1.417630+0.001224(20)+0.399296c)}
{1+\exp(-1.417630+0.001224(20)+0.399296c)}.
$$

The [chain rule for probabilities](../../../../../../../chain-rule-for-probabilities.md) then gives

$$
\boxed{\Pr(Y_{i1}=Y_{i2}=Y_{i3}=1\mid S_i=0,A_i=20,T_i=0,\mathcal H_{i0})
=\pi_0\pi_1\pi_2\simeq0.01911.}
$$

The three conditional [probabilities](../../../../../../../probability.md) are approximately $0.19891,0.27015,0.35559$. If “stop during the first three weeks” instead means at least one smoking-free week by week three, its different event has [probability](../../../../../../../probability.md) $1-(1-\pi_0)^3\simeq0.48590$: along the all-failure path the cumulative count stays zero. Stating the event resolves this wording ambiguity.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
