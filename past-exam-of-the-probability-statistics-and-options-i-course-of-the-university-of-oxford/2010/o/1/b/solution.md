<h1 id="o/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $s_e=S_D/\sqrt{17}$. By symmetry of the $t_{16}$ distribution, $\mathbb P(Z>-1.746)=0.95$. Rearranging $Z=(\overline D-\mu)/s_e>-1.746$ gives $\mu<\overline D+1.746s_e$. Thus the interval printed in the question has endpoint

$$
\boxed{b=\overline D+1.746S_D/\sqrt{17}.}
$$

There is a direction mismatch in the question. Since $D_i=X_i-Y_i$ is before minus after, a reduction corresponds to $H_1:\mu>0$. The upper interval $(-\infty,b)$ excludes zero when $b<0$, which instead tests against a negative [mean](../../../../../expected-value-split.md) difference.

For the stated reduction alternative, use the lower 95% interval $(\overline D-1.746s_e,\infty)$. It excludes zero exactly when

$$
\boxed{\frac{\overline D}{S_D/\sqrt{17}}>1.746.}
$$

This is the level-$0.05$ one-sided [paired t-test](../../../../../paired-t-test.md) of $H_0:\mu=0$ against $H_1:\mu>0$. Both the requested upper endpoint and the correctly directed test are thus determined without silently reversing the difference convention.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
