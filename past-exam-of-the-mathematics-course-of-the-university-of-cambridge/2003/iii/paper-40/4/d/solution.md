<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For equal allocation, let $n$ be the required [sample size](../../../../../../sample-size.md) per arm, $p_C=0.0045$, $p_T=0.003$ and $\Delta=0.0015$. In the standard [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md) calculation, a [two-sided test](../../../../../../two-sided-hypothesis-test.md) at 5% with 80% [statistical power](../../../../../../statistical-power.md) requires

$$
\Delta\sqrt n\simeq z_{0.975}\sqrt{2\bar p(1-\bar p)}+z_{0.8}\sqrt{p_C(1-p_C)+p_T(1-p_T)},\qquad \bar p=0.00375.
$$

Using $z_{0.975}=1.95996$ and $z_{0.8}=0.84162$ gives $n\simeq26063.64$, which is rounded upward for actual recruitment. Thus

$$
\boxed{N_{\rm total}\simeq52128,\quad\text{about }52.1\text{ thousand participants, or about }53\text{ thousand when planning in whole thousands}.}
$$

Since the risks are small, dropping the $(1-p)$ corrections and using $1.96+0.84$ gives $N_{\rm total}\simeq2(2.8)^2(0.0075)/(0.0015)^2=52266.7$, conventionally about 52.3 thousand. These are slightly different approximations to the same planning requirement. Add an allowance if outcome ascertainment is incomplete or the allocation is clustered. A prespecified [one-sided test](../../../../../../one-sided-hypothesis-test.md) would need a different, smaller [sample size](../../../../../../sample-size.md); the calculation here uses the conventional two-sided interpretation consistently with part (b).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
