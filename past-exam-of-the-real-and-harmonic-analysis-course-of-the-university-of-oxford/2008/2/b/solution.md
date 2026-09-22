<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A set $H$ is Lebesgue measurable when the [Caratheodory measurability criterion](../../../../caratheodory-s-criterion.md) holds:

$$
\mathcal L^*(E)=\mathcal L^*(E\cap H)+\mathcal L^*(E\setminus H)\quad\text{for every }E\subseteq\mathbb R^n.
$$

Subadditivity always gives the inequality with left side at most right side. For $H=\{x_i>t\}$, split each covering box $Q_j$ across the plane $x_i=t$. Its two pieces have total volume $|Q_j|$. The piece with a closed cut face can be enlarged by arbitrarily little into an open box; hence its [outer measure](../../../../outer-measure.md) is at most its corresponding volume, just as for the other piece. Subadditivity applied separately on the two sides consequently gives

$$
\mathcal L^*(E\cap H)+\mathcal L^*(E\setminus H)\leq\sum_j|Q_j|.
$$

For finite [outer measure](../../../../outer-measure.md) take a covering sum arbitrarily close to $\mathcal L^*(E)$; infinite [outer measure](../../../../outer-measure.md) follows already from subadditivity. Thus **every coordinate half space is measurable**.

Carathéodory's theorem says that the [measurable sets](../../../../measurable-set.md) form a [sigma-algebra](../../../../sigma-algebra.md) and the [outer measure](../../../../outer-measure.md) restricted to it is a [complete measure](../../../../complete-measure.md). Coordinate half spaces generate all open boxes and then all open sets, using countably many rational-endpoint boxes. They therefore generate the [Borel sigma-algebra](../../../../borel-sigma-algebra.md). Hence **every [Borel set](../../../../borel-set.md) is Lebesgue measurable**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
