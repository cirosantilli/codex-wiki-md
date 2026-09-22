<h1 id="25h/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**False.** Vanishing torsion only controls each connected region on which the curvature is nonzero. A smooth curve can pass through a flat point or straight segment and emerge in a different plane.

For an explicit local construction on $(-1,1)$, put $\eta(s)=e^{-1/s^2}$ for $s\ne0$ and $\eta(0)=0$, and define a unit tangent field

$$
T(s)=
\begin{cases}
(\sqrt{1-\eta(s)^2},\eta(s),0),&s<0,\\
(1,0,0),&s=0,\\
(\sqrt{1-\eta(s)^2},0,\eta(s)),&s>0.
\end{cases}
$$

This field is smooth because $\eta$ is flat at zero. Its integral $\alpha(s)=\int_0^sT(u)\,du$ is parametrized by arc length, has nonzero curvature for $s\ne0$, and has zero torsion on both sides. Its negative half lies nontrivially in the $xy$-plane and its positive half lies nontrivially in the $xz$-plane, so the whole curve is not planar.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [25H](../../../25h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
