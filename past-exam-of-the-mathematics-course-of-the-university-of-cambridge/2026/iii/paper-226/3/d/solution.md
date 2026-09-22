<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [OSSS inequality](../../../../../../osss-inequality.md) to the independent coordinates $(V_x,W_x)$ and to the indicator of the [one-arm event](../../../../../../one-arm-event.md) $A_R(a)$. Use the randomized [OSSS exploration of a one-arm event](../../../../../../osss-exploration-of-a-one-arm-event.md): choose $k$ uniformly from $\{1,\ldots,R\}$ and reveal the variables needed to explore the superlevel cluster meeting $\partial B_k$. A coordinate can be revealed only if a nearby vertex has an open connection over the relevant distance. Translation invariance, finite-range dependence and the [union bound](../../../../../../boole-s-inequality.md) therefore give the revealment estimate

$$
\delta_x\leq\frac{C_d}{R}\sum_{k=1}^R\theta_k
$$

for both kinds of coordinates, after enlarging the explored neighbourhood by a distance depending only on $d$.

For an increasing Gaussian threshold event, the resampling influence of $V_x$ is bounded by a universal constant times $\mathbb E[V_x\mathbf1_{A_R(a)}]$. The influence of $W_x$ is bounded by the sum of the corresponding $V$ influences at the $2d$ neighbours of $x$: indeed [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md) gives

$$
\mathbb E[W_x\mathbf1_{A_R(a)}]
=\frac1{2d}\sum_{z\sim x}\mathbb E[V_z\mathbf1_{A_R(a)}],
$$

first for smooth increasing approximations and then by a limit. Consequently the OSSS bound becomes

$$
\theta_R(1-\theta_R)
\leq C_d\left(\frac1R\sum_{k=1}^R\theta_k\right)
\sum_{x\in B_R}\mathbb E[V_x\mathbf1_{A_R(a)}].
$$

Part (c) identifies the final sum with $-\theta_R'(a)$. Dividing and putting $c=C_d^{-1}>0$ proves

$$
-\frac d{da}\theta_R
\geq c\,
\frac{\theta_R(1-\theta_R)}{R^{-1}\sum_{k=1}^R\theta_k}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
