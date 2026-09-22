<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is a [birth-death master equation](../../../../birth-death-master-equation.md): $q_n$ is the [transition rate](../../../../transition-intensity.md) $n\to n+1$ and $r_n$ is the [transition rate](../../../../transition-intensity.md) $n\to n-1$. The first two terms are incoming [probability](../../../../probability.md) flows from the adjacent states; the last removes [probability](../../../../probability.md) at the total escape rate $q_n+r_n$. Rates must be nonnegative. For a population on the nonnegative integers, take $r_0=0$ and no incoming flux from negative states.

Summing over all states and shifting the two incoming indices gives

$$
\frac d{dt}\sum_nP_n=\sum_n r_nP_n+\sum_nq_nP_n-\sum_n(q_n+r_n)P_n=0.
$$

Thus an initially normalized [probability distribution](../../../../probability-distribution-split.md) remains normalized. The cancellation assumes no boundary flux and legitimate summation; on an infinite state space this means the nonexplosive process or a boundary prescription that conserves total [probability](../../../../probability.md). All rates used in the later parts satisfy this requirement.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
