<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Parameterize the two [line segments](../../../../../line-segment.md) by

$$
P(s)=A+su,\quad Q(t)=C+tv,\qquad u=B-A,\quad v=D-C,\quad 0\leq s,t\leq1.
$$

Put $w=A-C$ and abbreviate $a=u\cdot u$, $b=u\cdot v$, $c=v\cdot v$, $d=u\cdot w$, and $e=v\cdot w$. Minimizing the [Euclidean distance](../../../../../euclidean-distance.md) is equivalent to minimizing the [convex quadratic function](../../../../../convex-quadratic-function.md)

$$
F(s,t)=\|w+su-tv\|^2=a s^2-2bst+ct^2+2ds-2et+\|w\|^2
$$

over a closed square. For nonzero nonparallel segment directions, $\Delta=ac-b^2=\|u\times v\|^2>0$. An interior minimum must satisfy

$$
as-bt=-d,\qquad -bs+ct=e,
$$

whose unique solution is

$$
\boxed{s_0=\frac{be-cd}{\Delta},\qquad t_0=\frac{ae-bd}{\Delta}.}
$$

Keep it as a candidate only if both parameters lie in $[0,1]$.

Every remaining minimum lies on the boundary. Define $[x]_{[0,1]}=\max(0,\min(1,x))$. The four edge minima are the point-to-segment [orthogonal projections](../../../../../orthogonal-projection.md)

$$
\begin{array}{c|c}
s=0&t=[e/c]_{[0,1]}\\
s=1&t=[(e+b)/c]_{[0,1]}\\
t=0&s=[-d/a]_{[0,1]}\\
t=1&s=[(b-d)/a]_{[0,1]}.
\end{array}
$$

Evaluate $F$ at those four pairs and at the admissible interior pair, and return a pair with the smallest value. This solves [closest points on two line segments](../../../../../closest-points-on-two-line-segments.md) completely: [continuity](../../../../../continuous-function.md) guarantees a minimum, and every interior or boundary location has been tested. **Do not independently clamp $s_0$ and $t_0$**: the mixed term couples them. For example, $A=(0,0)$, $B=(1,0)$, $C=(2,-2)$ and $D=(3,-1)$ give the line minimizer $(s_0,t_0)=(4,2)$. Its independently clamped pair $(1,1)$ has squared distance $5$, whereas the correct edge minimizer $(1,1/2)$ has squared distance $9/2$.

Without general position, explicitly handle these configurations:

- If either segment has zero length, solve a point-to-segment projection; if both do, return the two points. This avoids division by $a$ or $c$.
- If the directions are parallel, $\Delta=0$ and the interior [linear system](../../../../../system-of-linear-equations.md) is singular. The four edge projections still contain a minimum. Overlapping projected parameter intervals can yield a whole family of closest pairs.
- Collinear segments may overlap, touch, or be disjoint. Overlap gives zero distance with many choices; disjoint intervals give their nearest endpoints.
- Coplanar nonparallel segments can intersect, including endpoint contacts. The same candidate tests return zero distance if the line-intersection parameters lie in the square. Coincident endpoints and equal candidate distances need no arbitrary division or uniqueness assumption.

In floating-point arithmetic, almost-parallel directions require a condition-aware or higher-precision solve; they must not be declared exactly parallel solely because the computed determinant is small. The returned distance is $\boxed{\sqrt{\min F}}$, and the returned points are obtained by substitution into $P(s),Q(t)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
