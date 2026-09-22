<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Frailty makes a population hazard ratio mix the conditional treatment effect with changing survivor composition. Suppose

$$
h(t\mid U=u,Z=z)=u\theta e^{\beta z}
$$

and $U\sim\operatorname{Exponential}(1)$. Part (a)(ii), with $\theta$ replaced by $\theta e^{\beta z}$, gives

$$
\bar h_z(t)=\frac{\theta e^{\beta z}}
{1+\theta e^{\beta z}t}.
$$

Although conditional hazards are proportional with ratio $e^\beta$, the marginal ratio is

$$
\frac{\bar h_1(t)}{\bar h_0(t)}
=e^\beta\frac{1+\theta t}{1+\theta e^\beta t},
$$

which varies with time and tends to one. Thus an ordinary marginal [proportional hazards](../../../../../../proportional-hazards-model.md) interpretation can be misleading in the presence of unobserved heterogeneity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
