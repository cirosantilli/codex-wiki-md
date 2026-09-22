<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use equal individual allocation, a two-sided 5% test as in part (a), 80% power, complete four-week ascertainment and the supplied fatal-overdose endpoint. Then $p_0=1/200=0.005$, $p_1=0.7p_0=0.0035$, and $\bar p=0.00425$. Substituting into the [sample size for comparing two proportions](../../../../../../../sample-size-for-comparing-two-proportions.md) gives

$$
n\simeq
\frac{\left[1.959964\sqrt{2(0.00425)(0.99575)}+
0.841621\sqrt{(0.005)(0.995)+(0.0035)(0.9965)}\right]^2}
{(0.0015)^2}
\simeq29524.1.
$$

Rounding upward for equal allocation gives

$$
\boxed{29525\text{ consented eligible prisoners per arm},\qquad
59050\text{ in total, approximately }59000.}
$$

The corresponding expected endpoint counts are about 148 in the control arm and 103 in the active arm. The one-third eligibility proportion affects how many prisoners must be screened, not the number of eligible participants randomized; at full consent and eligibility ascertainment, roughly three times this randomized total would need screening. Loss to follow-up, nonadherence or a changed baseline mortality risk would require a separate design adjustment.

The wording needs an endpoint qualification. The supplied risk is death from overdose, and the proposed effect concerns preventing those deaths. It does not give the incidence of all overdoses. Thus the calculation above sizes **fatal overdoses**, the intended endpoint supported by the data. For a literal 30% reduction in all overdoses, the unknown baseline incidence $q$ must replace $0.005$ in the formula, with $p_1=0.7q$. This is the [endpoint-specific rare-event sample size](../../../../../../../endpoint-specific-rare-event-sample-size.md) issue: the same fatal risk can coexist with many nonfatal rates. For example $q=0.005$ gives about 29525 per arm, whereas $q=0.05$ gives about 2838; knowing only the fatal rate cannot determine that latter [sample size](../../../../../../../sample-size.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
