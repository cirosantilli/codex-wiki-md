<h1 id="14c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define

$$
N=S+I,
\qquad
\theta=\frac IN,
$$

so $S=N(1-\theta)$ and $I=N\theta$. Part (a) already gives

$$
\boxed{\dot N=N(1-N).}
$$

Using the [quotient rule](../../../../../../quotient-rule.md),

$$
\dot\theta
=\frac{\dot I N-I\dot N}{N^2}
=\theta\{\beta N(1-\theta)-1\},
$$

and hence the reduced [Plant SI model with logistic total population](../../../../../../plant-si-model-with-logistic-total-population.md) is

$$
\boxed{
\dot N=N(1-N),
\qquad
\dot\theta=\theta\{\beta N(1-\theta)-1\}.}
$$

For every $N(0)>0$, logistic growth gives $N(t)\to1$. The asymptotic prevalence equation is therefore

$$
\dot\theta=\theta\{(\beta-1)-\beta\theta\}.
$$

If $\beta<1$, its only nonnegative equilibrium is $\theta=0$, which attracts all prevalences. If $\beta>1$, $	heta=0$ is unstable and the stable value is $\theta_*=1-1/\beta$. Combining these values with $N_*=1$ recovers exactly the equilibria and outcomes in part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
