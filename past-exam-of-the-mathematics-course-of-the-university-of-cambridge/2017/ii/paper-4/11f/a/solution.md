<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u(t)=\gamma(t)/|\gamma(t)|$, a [continuous map](../../../../../../continuous-map.md) into the [unit circle](../../../../../../complex-unit-circle.md). By [uniform continuity](../../../../../../uniform-continuity.md), partition $[0,1]$ so finely that on each interval beginning at $t_j$, $|u(t)/u(t_j)-1|<1$. This ratio lies in the right half-plane and has a continuous [complex argument](../../../../../../argument-complex-analysis.md) with value zero at $t_j$. Starting from $\theta_0$, add these local arguments successively, matching endpoint values. This constructs a continuous real lift with $u(t)=e^{i\theta(t)}$.

Any two such lifts with the same initial value differ by a [continuous function](../../../../../../continuous-function.md) taking values in $2\pi\mathbb Z$, and hence coincide. Since the curve closes, $e^{i(\theta(1)-\theta(0))}=1$. Define its [winding number](../../../../../../winding-number.md) by

$$
\boxed{w(\gamma)=\frac{\theta(1)-\theta(0)}{2\pi}\in\mathbb Z.}
$$

Changing the chosen initial argument adds a constant multiple of $2\pi$ to the whole lift, so the [winding number](../../../../../../winding-number.md) is independent of that choice. No [differentiability](../../../../../../differentiability.md) of the curve is required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
