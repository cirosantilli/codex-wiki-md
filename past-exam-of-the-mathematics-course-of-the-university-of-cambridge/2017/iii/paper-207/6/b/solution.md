<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Only times up to $\tau$ contribute to the [cumulative incidence function](../../../../../../cumulative-incidence-function.md) for type $B$, because its [cause-specific hazard](../../../../../../cause-specific-hazard.md) vanishes afterwards. With $q=\theta_A+\theta_B>0$,

$$
F_B(t)=\int_0^{\min(t,\tau)}\theta_B e^{-qu}\,du,
$$

so

$$
\boxed{F_B(t)=\frac{\theta_B}{\theta_A+\theta_B}\left(1-e^{-(\theta_A+\theta_B)\min(t,\tau)}\right).}
$$

This increases before $\tau$ and then remains constant; it includes the protection from type $B$ events produced by earlier type $A$ events. If both intensities vanish, $F_B=0$; if $\theta_B=0$, it is also identically zero.

## ↑ Ancestors (11)

1. [B](../b.md)
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
