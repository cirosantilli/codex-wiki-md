<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Gibbs sampler](../../../../../../gibbs-sampler.md) draws each variable from its [full conditional distribution](../../../../../../full-conditional-distribution.md), so every proposed update is accepted. At the start of a sweep define $c_s=\widetilde c_s-E_s$, $y_s=\widetilde M_s-RE_s$, and

$$
d_s=\widetilde M_s-M_0-\beta\widetilde c_s,
\qquad
v_E=\left(\frac1{\sigma_c^2}+\frac{(R-\beta)^2}{\sigma_M^2}\right)^{-1},
$$



$$
m_{E,s}=v_E\left[
\frac{\widetilde c_s-c_0}{\sigma_c^2}
+\frac{(R-\beta)d_s}{\sigma_M^2}
-\frac1\tau
\right].
$$

First update the reddenings independently as

$$
E_s\mid\text{rest}\sim TN_{[0,\infty)}(m_{E,s},v_E).
$$

Recompute $c_s$ and $y_s$, then make the Gaussian updates

$$
c_0\mid\text{rest}\sim N\!\left(\bar c,\frac{\sigma_c^2}{N}\right),
$$



$$
M_0\mid\text{rest}\sim N\!\left(
\frac1N\sum_s(y_s-\beta c_s),\frac{\sigma_M^2}{N}
\right),
$$



$$
\beta\mid\text{rest}\sim N\!\left(
\frac{\sum_sc_s(y_s-M_0)}{\sum_sc_s^2},
\frac{\sigma_M^2}{\sum_sc_s^2}
\right),
$$

and

$$
R\mid\text{rest}\sim N\!\left(
\frac{\sum_sE_s[\widetilde M_s-M_0-\beta c_s]}{\sum_sE_s^2},
\frac{\sigma_M^2}{\sum_sE_s^2}
\right).
$$

With

$$
S_c=\sum_s(c_s-c_0)^2,
\qquad
S_M=\sum_s(y_s-M_0-\beta c_s)^2,
$$

the remaining full conditionals, in the parameterization given in the question, are the [scaled inverse chi-squared laws](../../../../../../scaled-inverse-chi-squared-distribution.md)

$$
\sigma_c^2\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(N-2,\frac{S_c}{N-2}\right),
$$



$$
\sigma_M^2\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(N-2,\frac{S_M}{N-2}\right),
$$



$$
\tau\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(2N-2,\frac{\sum_sE_s}{N-1}\right).
$$

Repeating these updates in the displayed order gives a complete Gibbs sweep. The formulas assume $N>2$ and nondegenerate sampled predictors; posterior propriety must be checked because the hyperpriors are improper.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
