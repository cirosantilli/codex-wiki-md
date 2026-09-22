<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The fitted formula and coefficient table describe a [random-slope linear mixed model](../../../../../../random-slope-linear-mixed-model.md):

$$
Y_{ij}=\beta_0+(\beta_1+b_j)t_{ij}+\varepsilon_{ij},\qquad
b_j\overset{\mathrm{iid}}\sim N(0,\tau^2),\qquad
\varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2),
$$

with [random effects](../../../../../../random-effect.md) independent of the errors. There is a common fixed intercept, a population slope $\beta_1$, and a laboratory [random slope](../../../../../../random-slope.md) deviation $b_j$. In `tumour1`, the three laboratory slopes are unrelated unknown fixed coefficients. Here they are modelled as draws from a common [normal distribution](../../../../../../normal-distribution.md); estimated laboratory deviations are shrunk toward zero. After integrating out $b_j$, observations in laboratory $j$ have [covariance](../../../../../../covariance.md) $\tau^2t_{ij}t_{kj}+\sigma^2\mathbf1_{\{i=k\}}$, so they are marginally dependent even when their conditional errors are independent.

The displayed command contains a source inconsistency: `size ~ 1 + (0 + days | lab)` would impose zero population slope and could not produce the displayed fixed `days` coefficient. **The output corresponds to `size ~ days + (0 + days | lab)`.** Its estimates are $\widehat\beta_0=0.6464$, $\widehat\tau^2=17.08$ and $\widehat\sigma^2=227.76$. The estimated daily increase averaged over the laboratory population is

$$
\boxed{\widehat\beta_1=10.7895\ \mathrm{mm/day},}
$$

because $\mathbb E b_j=0$.

A [random slope](../../../../../../random-slope.md) is appropriate if these laboratories can reasonably be viewed as exchangeable representatives of a larger population and the goal includes population inference or predictions for other laboratories. If these particular three laboratories are the whole set of interest, or have systematic differences incompatible with exchangeability, laboratory-specific fixed slopes are preferable. Only three groups give weak information about between-laboratory [variance](../../../../../../variance-split.md); the mixed model does not itself resolve possible nonlinear growth. Its population mean is distinct from a realized finite-group average $\beta_1+(b_A+b_B+b_C)/3$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
