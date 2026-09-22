<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For independent exponential survival times with total observed [person-time at risk](../../../../../../person-time-at-risk.md) $T_\bullet$ and $d$ events, the maximum-likelihood rate is $\widehat h=d/T_\bullet$. A two-group exponential model is a proportional-hazards model because both hazards are constant, so their ratio is constant.

Here

$$
\widehat h_0=\frac{1+k}{t_1+t_4},
\qquad
\widehat h_1=\frac1{t_2+c}.
$$

Thus the group-1 to group-0 hazard-ratio estimate is

$$
\boxed{\widehat\lambda
=\frac{t_1+t_4}{(1+k)(t_2+c)}}.
$$

It decreases continuously as $c$ increases. The parametric exponential likelihood uses exact exposure times through each arm's person-time, whereas the Cox partial likelihood uses only which subjects belong to each event's risk set. For $t_2<c<t_4$, changing $t_4$ alters group 0 person-time and hence $\widehat\lambda$, but subject 4 is alone if it fails at $t_4$, so that event contributes one to the partial likelihood and $\widehat\theta$ is unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
