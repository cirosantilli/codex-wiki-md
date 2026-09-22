<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the time-homogeneous [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) displayed in part ii. Write $Z(t)$ for the state at time $t$, $Q=(q_{rs})$ for its [generator matrix](../../../../../../generator-matrix.md), and

$$
p_{rs}(u)=\Pr\{Z(t+u)=s\mid Z(t)=r\},\qquad P(u)=e^{uQ}.
$$

For $r\ne s$, $q_{rs}=\lim_{h\downarrow0}p_{rs}(h)/h$ is the [transition intensity](../../../../../../transition-intensity.md), and $q_{rr}=-\sum_{s\ne r}q_{rs}$. Condition on the observed initial state, and treat the clinic observation process and administrative end of follow-up as noninformative. A panel-observed interval contributes its [transition probability](../../../../../../transition-probability.md), not the density of a jump at the examination date; the transitions inside that interval need not have been observed.

For the first patient, the two clinic intervals contribute $p_{11}(2)p_{13}(2)$. The subsequent death is observed at elapsed time $u=0.2$ after the last clinic state, so its contribution is the conditional death-time density

$$
g_{35}(u)=\sum_{s=1}^4p_{3s}(u)q_{s5}=p_{33}(u)q_{35}+p_{34}(u)q_{45}.
$$

The equality uses the permitted directions: starting from state 3, only living states 3 and 4 can be occupied before death. To obtain this density directly, survival in a living state $s$ until time $u$, followed by death in $(u,u+du)$, has [probability](../../../../../../probability.md) $p_{3s}(u)q_{s5}\,du+o(du)$; add over the unobserved state $s$. Hence the [mixed panel and exact-death likelihood](../../../../../../mixed-panel-and-exact-death-likelihood.md) contribution is

$$
\boxed{L_1=p_{11}(2)p_{13}(2)\{p_{33}(0.2)q_{35}+p_{34}(0.2)q_{45}\}.}
$$

It includes the possibility of an unrecorded transition $3\to4\to5$ between the last clinic visit and death. Keeping only $p_{33}(0.2)q_{35}$ would exclude that allowed history, while $p_{35}(0.2)$ would be the [probability](../../../../../../probability.md) of death by that time rather than the density of death at that time. With dates recorded in whole days, an exact interval-likelihood treatment integrates this density over the relevant day; the density formulation is its fine-time approximation.

For the second patient, the three successive intervals with state 1 at both ends, then the interval ending in state 2, and the last interval remaining in state 2 give the [panel-observed multi-state likelihood](../../../../../../panel-observed-multi-state-likelihood.md)

$$
\boxed{L_2=p_{11}(2)^3p_{12}(2)p_{22}(2).}
$$

There is no additional death contribution after the final administrative observation. Each likelihood contribution already accounts for being alive in the observed state at that visit. For independent patients their joint conditional [likelihood](../../../../../../likelihood-function.md) contribution is $L_1L_2$.

For an explicit form, put $\lambda_r=-q_{rr}$. Irreversibility gives

$$
p_{rr}(u)=e^{-\lambda_ru},\qquad
p_{1s}(u)=\frac{q_{1s}}{\lambda_s-\lambda_1}(e^{-\lambda_1u}-e^{-\lambda_su})\quad(s=2,3),
$$

and

$$
p_{34}(u)=\frac{q_{34}}{\lambda_4-\lambda_3}(e^{-\lambda_3u}-e^{-\lambda_4u}).
$$

These formulas follow by integrating the density of the one possible intermediate jump time; at equal exit rates the limiting expression is $q_{rs}u e^{-\lambda_ru}$. Thus

$$
g_{35}(u)=q_{35}e^{-\lambda_3u}+\frac{q_{34}q_{45}}{\lambda_4-\lambda_3}(e^{-\lambda_3u}-e^{-\lambda_4u}).
$$

Using the displayed fitted rates as numerical values gives $g_{35}(0.2)\approx0.289314$ per year, $L_1\approx0.017596$ per year and $L_2\approx0.016048$, providing a check of the probability-versus-density distinction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
