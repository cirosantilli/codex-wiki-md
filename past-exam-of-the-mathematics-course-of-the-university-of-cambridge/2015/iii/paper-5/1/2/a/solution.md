<h1 id="1/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [characteristic curve](../../../../../../../characteristic-curve.md) has $x-at$ constant. Backtracking reaches the initial line if $x\ge at$ and the inflow boundary otherwise. Hence

$$
\boxed{u(t,x)=\begin{cases}u_0(x-at),&x\ge at,\\ f(t-x/a),&0\le x<at.\end{cases}}
$$

Values on the dividing [characteristic curve](../../../../../../../characteristic-curve.md) are immaterial for bounded [weak solutions](../../../../../../../weak-solution.md).

For a [classical solution](../../../../../../../classical-solution.md) on the closed quadrant, choose $u_0,f\in C^1([0,\infty))$ and impose the [corner compatibility for constant-speed transport](../../../../../../../corner-compatibility-for-constant-speed-transport.md)

$$
\boxed{f(0)=u_0(0),\qquad f'(0)=-a u_0'(0).}
$$

These make the values and both first derivatives agree across $x=at$; each branch solves the [transport equation](../../../../../../../transport-equation.md). They are also necessary for a $C^1$ solution up to the initial and inflow boundaries.

Spatial $C^\infty$ regularity for every $t\ge0$, up to $x=0$, holds precisely for smooth data with all matching jets:

$$
\boxed{f^{(n)}(0)=(-a)^n u_0^{(n)}(0)\quad(n=0,1,2,\ldots).}
$$

Indeed the spatial derivatives of order $n$ at $x=at$ are $u_0^{(n)}(0)$ and $(-1/a)^n f^{(n)}(0)$. Necessity of smooth $u_0$ follows at $t=0$; smoothness of $f$ on any finite interval follows by reading the boundary branch in a spatial slice at a larger time.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
