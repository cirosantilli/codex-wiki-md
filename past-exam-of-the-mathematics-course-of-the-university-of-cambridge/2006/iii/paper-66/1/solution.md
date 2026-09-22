<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [closest points on two line segments](../../../../../closest-points-on-two-line-segments.md) as a small constrained [convex optimization](../../../../../convex-optimization-split.md) problem. Write the two [line segments](../../../../../line-segment.md) as

$$
R_1(s)=P_1+sd,\qquad R_2(t)=P_2+te,\qquad d=Q_1-P_1,\quad e=Q_2-P_2,\quad 0\leq s,t\leq1,
$$

and put $w=P_1-P_2$. Minimize the squared [Euclidean distance](../../../../../euclidean-distance.md) $D(s,t)=\|w+sd-te\|^2$; minimizing its square also minimizes the distance. Compute the [dot products](../../../../../dot-product.md)

$$
\alpha=d\cdot d,\quad\beta=d\cdot e,\quad\gamma=e\cdot e,\quad\delta=d\cdot w,\quad\varepsilon=e\cdot w.
$$

For nonzero, nonparallel directions, an interior minimum must satisfy the two derivative equations

$$
\alpha s-\beta t=-\delta,\qquad -\beta s+\gamma t=\varepsilon.
$$

Their determinant is $\Delta=\alpha\gamma-\beta^2>0$, so the stationary candidate is

$$
s_*={\beta\varepsilon-\gamma\delta\over\Delta},\qquad t_*={\alpha\varepsilon-\beta\delta\over\Delta}.
$$

Retain this candidate only when both parameters lie in the unit interval.

The other possibilities are on the boundary. Define $\operatorname{clip}(x)=\max(0,\min(1,x))$. Minimizing the same quadratic on each of the four edges gives these candidates by [orthogonal projection](../../../../../orthogonal-projection.md) onto a [line segment](../../../../../line-segment.md):

$$
\begin{array}{c|c}
s&t\\\hline
0&\operatorname{clip}(\varepsilon/\gamma)\\
1&\operatorname{clip}((\beta+\varepsilon)/\gamma)\\
\operatorname{clip}(-\delta/\alpha)&0\\
\operatorname{clip}((\beta-\delta)/\alpha)&1
\end{array}
$$

Evaluate $D$ at every retained candidate and choose the smallest. **The resulting $R_1(s),R_2(t)$ are the required closest points.** The quadratic is convex because it is the squared norm of an [affine map](../../../../../affine-map.md). A minimum in the interior is stationary, and a minimum on the boundary minimizes one of these edge restrictions, so the list is exhaustive. Ties correspond to multiple equally valid answers.

Handle degenerate [line segments](../../../../../line-segment.md) before dividing: if $\alpha=0$ and $\gamma>0$, set $s=0$ and $t=\operatorname{clip}(\varepsilon/\gamma)$; if $\gamma=0$ and $\alpha>0$, set $t=0$ and $s=\operatorname{clip}(-\delta/\alpha)$; if both vanish, use the two endpoints. For exactly parallel directions, $\Delta=0$. The distance depends on a single linear combination of $s,t$; any interior minimizing level line reaches the boundary, so the four edge candidates still include a minimum.

For nearly parallel directions, compare $\Delta$ with the scale $\alpha\gamma$, and solve the interior least-squares problem using [QR decomposition](../../../../../qr-decomposition.md) or [singular value decomposition](../../../../../singular-value-decomposition.md) if necessary. A small determinant should trigger a stable solve, not arbitrary rejection of a possibly valid interior solution. In particular, do not merely clip both coordinates of the infinite-line solution: the [dot product](../../../../../dot-product.md) $\beta$ couples the two parameters, and changing one changes the optimum for the other.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
