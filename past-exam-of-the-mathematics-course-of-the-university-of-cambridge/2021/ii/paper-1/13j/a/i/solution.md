<h1 id="13j/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Y_{go}$ be the count for treatment

$$
g\in\{C,L,S\}
$$

(Control, LD, or SD) and outcome

$$
o\in\{B,W\}
$$

(Better or Worse), and write $\mu_{go}=\mathbb E Y_{go}$. Both fits take the six cell counts to be independent [Poisson](../../../../../../../poisson-distribution.md) variables.

The additive [log-linear model](../../../../../../../log-linear-model.md) fitted by `fit1` is

$$
Y_{go}\sim\operatorname{Pois}(\mu_{go}),
\qquad
\log\mu_{go}=\lambda+\alpha_g+\beta_o,
$$

with reference constraints $\alpha_C=0$ and $\beta_B=0$. Thus treatment changes the overall group count but not the relative frequencies of the two outcomes.

The interaction model fitted by `fit2` is

$$
Y_{go}\sim\operatorname{Pois}(\mu_{go}),
\qquad
\log\mu_{go}
=\lambda+\alpha_g+\beta_o+\gamma_{go},
$$

where, under reference coding,

$$
\gamma_{CB}=\gamma_{CW}=\gamma_{LB}=\gamma_{SB}=0
$$

and the two free interactions are $\gamma_{LW}$ and $\gamma_{SW}$. This is the [saturated log-linear model](../../../../../../../saturated-log-linear-model.md) for the $3\times2$ table.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [13J](../../../13j.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
