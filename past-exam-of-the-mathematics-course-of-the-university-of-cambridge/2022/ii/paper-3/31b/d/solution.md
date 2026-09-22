<h1 id="31b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Poincaré-Bendixson theorem](../../../../../../poincare-bendixson-theorem.md) states that a nonempty compact $\omega$-limit set of a planar $C^1$ flow which contains no equilibrium is a periodic orbit.

The origin is the only equilibrium: at a nonzero equilibrium, putting $q=x^2+y^2-a$ would require

$$
\begin{pmatrix}q&3\\-1&q\end{pmatrix}
\binom xy=0,
$$

but its determinant $q^2+3$ is positive. By local asymptotic stability, choose a small simple closed Lyapunov level curve on which the original vector field points inward. On a sufficiently large circle,

$$
\frac12\frac d{dt}(x^2+y^2)
=(x^2+y^2)^2-a(x^2+y^2)+2xy>0,
$$

so the original vector field points outward.

Reverse time. The annulus between these two curves is then a compact positively invariant [trapping region](../../../../../../trapping-region.md): the reversed field points into it at both boundaries. It contains no equilibrium. The Poincaré--Bendixson theorem applied to any reversed trajectory in the annulus produces a periodic orbit. Reversing time does not change its image, so the original system also has a periodic orbit.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31B](../../31b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
