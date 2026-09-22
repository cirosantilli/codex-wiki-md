<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By [conditional probability](../../../../../../conditional-probability.md) and continuity of event times,

$$
\mathbb P(J=A\mid T<\tau)=\frac{F_A(\tau)}{F_A(\tau)+F_B(\tau)}.
$$

When $\tau>0$ and $q=\theta_A+\theta_B>0$, the common factor $1-e^{-q\tau}$ cancels, giving

$$
\boxed{\mathbb P(J=A\mid T<\tau)=\frac{\theta_A}{\theta_A+\theta_B}.}
$$

Before $\tau$, the constant [cause-specific hazards](../../../../../../cause-specific-hazard.md) divide the total event intensity in these proportions, regardless of how long the interval is. If $\tau=0$ or both intensities are zero, the conditioning event has [probability](../../../../../../probability.md) zero and this [conditional probability](../../../../../../conditional-probability.md) is undefined, not a ratio assigned by convention.

## ↑ Ancestors (11)

1. [D](../d.md)
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
