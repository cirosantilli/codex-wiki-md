<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $z_i=(S_i,E_i,A_i)^T$ contain sex, the education indicator, and age at diagnosis. Write $\overline z$ for the sample means. The output's baseline [transition intensities](../../../../../../../transition-intensity.md) are evaluated at those means, so use the centred [log-linear transition intensity model](../../../../../../../log-linear-transition-intensity-model.md)

$$
q_{rs}(z_i)=q_{rs}(\overline z)\exp\{\beta_{rs}^T(z_i-\overline z)\},
\qquad (r,s)\in\{(1,2),(1,3),(2,3)\}.
$$

The full [transition intensity matrix](../../../../../../../transition-intensity-matrix.md) is

$$
Q_i=\begin{pmatrix}
-q_{12}(z_i)-q_{13}(z_i)&q_{12}(z_i)&q_{13}(z_i)\\
0&-q_{23}(z_i)&q_{23}(z_i)\\
0&0&0
\end{pmatrix}.
$$

The fitted centred baselines are $(q_{12},q_{13},q_{23})(\overline z)=(0.1821,0.0126,0.0450)$, and fitted slope vectors in sex–education–age order are

$$
\widehat\beta_{12}=(0.09534,-0.4306,0.007627)^T,\qquad
\widehat\beta_{13}=(0,1.223,0.1262)^T,\qquad
\widehat\beta_{23}=(0,-1.490,0.07984)^T.
$$

The two sex coefficients displayed as zero are fixed by the specified constraints; they are not estimated to be exactly zero. There are three free baseline [transition intensities](../../../../../../../transition-intensity.md) and seven free covariate slopes. The sample means are not printed, so uncentred intercepts at $z=0$ cannot be recovered numerically from this output.

Conditional on fixed [covariates](../../../../../../../covariate.md), subjects follow independent, correctly classified [continuous-time multi-state models](../../../../../../../continuous-time-multi-state-model.md) obeying the [time-homogeneous Markov property](../../../../../../../time-homogeneous-markov-property.md), with $P_i(u)=e^{uQ_i}$. The progression is irreversible and death absorbing, with constant [transition intensities](../../../../../../../transition-intensity.md) during follow-up for each subject. In particular, the model uses fixed age at diagnosis rather than attained age. It assumes noninformative observation and [censoring](../../../../../../../censoring-statistics.md), and treats death times as exact through the [mixed panel and exact-death likelihood](../../../../../../../mixed-panel-and-exact-death-likelihood.md). The [Markov property](../../../../../../../markov-property.md) rules out an additional effect of elapsed time in the current state after conditioning on it and the recorded predictors.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
