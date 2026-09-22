<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Bendixson-Dulac theorem](../../../../bendixson-dulac-theorem.md) states that if $(P,Q)$ is a continuously differentiable planar [vector field](../../../../vector-field.md) on a [simply connected](../../../../simply-connected-space.md) open region $D$, and a continuously differentiable [Dulac function](../../../../dulac-function.md) $B$ makes

$$
\frac{\partial(BP)}{\partial x}+\frac{\partial(BQ)}{\partial y}
$$

have one weak sign throughout $D$, without vanishing identically on any nonempty open subset, then there is no nonconstant [periodic orbit](../../../../periodic-orbit.md) contained in $D$. To see why, a hypothetical simple [periodic orbit](../../../../periodic-orbit.md) bounds a region in $D$. The [divergence theorem](../../../../divergence-theorem.md) gives the [integral](../../../../integral-split.md) of this expression as the outward flux of $B(P,Q)$ across the orbit. The flux is zero because the [vector](../../../../vector.md) field is tangent to its orbit, whereas the one-sign area [integral](../../../../integral-split.md) is nonzero, a contradiction. The usual stricter version assumes a strictly positive or strictly negative expression everywhere.

For the printed [polynomial](../../../../polynomial-split.md) system, the origin is an [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) and

$$
M(0,0)=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad\lambda=\pm i.
$$

Thus **its [linearization](../../../../linearization.md) is a [centre equilibrium](../../../../center-equilibrium.md)**. For the full system take $B=1$. The [divergence](../../../../divergence.md) is

$$
P_x+Q_y=x^4-3x^2+x^2y^2=x^2(x^2+y^2-3).
$$

On the open disk $x^2+y^2<3$ this is nonpositive, and is negative wherever $x\ne0$. Its zero set inside the disk is a line, so it cannot vanish on any open subset. The [Bendixson-Dulac theorem](../../../../bendixson-dulac-theorem.md) therefore proves

$$
\boxed{\text{There are no nonconstant periodic orbits contained in }x^2+y^2<3.}
$$

This also exposes a terminology problem in the source: a nonlinear [centre equilibrium](../../../../center-equilibrium.md) has surrounding closed orbits, so the printed claim of a centre cannot hold in that sense. The imaginary [eigenvalues](../../../../eigenvalue.md) establish only a centre of the linearized system. In fact the full [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is an **asymptotically stable [weak focus](../../../../weak-focus.md)**, as the following direct check shows.

A [quartic Lyapunov correction for a weak focus](../../../../quartic-lyapunov-correction-for-a-weak-focus.md) makes the nonlinear damping visible. Put $r^2=x^2+y^2$ and consider the [Lyapunov function](../../../../lyapunov-function.md)

$$
V(x,y)=\frac{x^2+y^2}{2}-\frac{5x^3y+3xy^3}{8}=\frac{r^2}{2}+O(r^4).
$$

It is positive definite sufficiently close to zero. Differentiating along the [polynomial](../../../../polynomial-split.md) [vector](../../../../vector.md) field gives

$$
\dot V=-\frac38(x^2+y^2)^2+O(r^6)=-\frac38r^4+O(r^6).
$$

For clarity, the quartic terms come from $-x^4$ in the [derivative](../../../../derivative.md) of $r^2/2$, and from applying $y\partial_x-x\partial_y$ to the quartic correction. Their sum is $-3x^4/8-3x^2y^2/4-3y^4/8$; all other terms have degree at least six. Therefore $\dot V<0$ in a sufficiently small punctured neighbourhood, proving [asymptotic stability](../../../../asymptotic-stability.md) by [Second Lyapunov theorem](../../../../second-lyapunov-theorem.md). Finally

$$
\dot\theta=\frac{xQ-yP}{r^2}=-1+O(r^2),
$$

so nonconstant nearby orbits turn clockwise as they converge. The [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is a weak focus despite the centre in its [linearization](../../../../linearization.md). This interpretation resolves both the local dynamics and the absence of closed orbits without changing the printed [coefficients](../../../../coefficient.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
