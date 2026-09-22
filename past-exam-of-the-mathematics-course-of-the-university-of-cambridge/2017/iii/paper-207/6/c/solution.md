<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two event types are disjoint and exhaustive among first events, so their [cumulative incidence functions](../../../../../../cumulative-incidence-function.md) sum to the [probability](../../../../../../probability.md) of any event by $t$. Equivalently their derivatives add to $S(t)(h_A(t)+h_B(t))=-S'(t)$. Therefore

$$
\boxed{F_A(t)+F_B(t)=1-S(t)=1-e^{-\theta_A t-\theta_B\min(t,\tau)}.}
$$

For the usual positive disease-death intensity $\theta_A>0$, the limit is one: eventually every individual has an event, even though treatment-side-effect events cease after $\tau$. If the permitted boundary $\theta_A=0$ is included, however,

$$
\boxed{\lim_{t\to\infty}(F_A+F_B)=1-e^{-\theta_B\tau}.}
$$

Then a fraction $e^{-\theta_B\tau}$ remains event-free forever, because all hazards vanish after $\tau$. This includes the no-event case $\theta_A=\theta_B=0$. Thus an assertion that the limit always equals one requires $\theta_A>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
