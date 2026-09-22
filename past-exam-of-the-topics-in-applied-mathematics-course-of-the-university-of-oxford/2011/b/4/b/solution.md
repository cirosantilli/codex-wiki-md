<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A positive equilibrium must have $v=u=s$. Let

$$
D=\sqrt{(1-a-d)^2+4d},\qquad\boxed{s=\frac{1-a-d+D}{2}\in(0,1).}
$$

It is the unique positive root of $(1-s)(s+d)=as$. At this point the [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J_* =\begin{pmatrix}L&-(1-s)\\b&-b\end{pmatrix},\qquad L=\frac{s(1-d-2s)}{s+d}.
$$

Consequently

$$
\boxed{\operatorname{tr}J_*=L-b,\qquad\det J_*=\frac{bsD}{s+d}>0.}
$$

It is linearly asymptotically stable when $b>L$, and unstable when $0<b<L$. In either region it is a node or focus according as $(L-b)^2-4bsD/(s+d)$ is nonnegative or negative. At $b=L>0$ the linear [eigenvalues](../../../../../eigenvalue.md) are purely imaginary. If $L\leq0$, it is stable for every $b>0$.

The requested boundary follows from $1-d-2s=a-D$ and $s/(s+d)=(1-s)/a$:

$$
\boxed{b=L=\frac1{2a}(a-D)(1+a+d-D).}
$$

To prove a [limit cycle](../../../../../limit-cycle.md) exists in the unstable case, a compact trapping set must stay away from the singular boundary $u=0$. The following construction supplies it. Choose $M>1$ large enough to contain the positive equilibrium and the orbit being considered. On $u=M$, $\dot u<0$, and on $v=M$ with $u\leq M$, $\dot v\leq0$. Put $P=ue^{-v}$. Using $u+d\geq d$ and completing the square in $v$ gives

$$
\frac{\dot P}{P}=\frac{\dot u}u-\dot v\geq1-u-(a/d+b)v+\frac{bv^2}u\geq1-u\left[1+\frac{(a/d+b)^2}{4b}\right].
$$

Choose $\varepsilon>0$ so small that $\varepsilon e^M$ times the square bracket is less than $1/2$, and then choose $0<\eta<\varepsilon$. The set

$$
\mathcal K=\{u\leq M,\ \eta\leq v\leq M,\ ue^{-v}\geq\varepsilon\}
$$

is compact in the positive quadrant and forward invariant. On the curved boundary $P=\varepsilon$, $u\leq\varepsilon e^M$ and $\dot P>0$. On $v=\eta$, $u\geq\varepsilon>\eta$ gives $\dot v>0$. Its other boundaries were checked above. The constants can be chosen so the equilibrium is interior.

When $b<L$, the equilibrium is a hyperbolic repeller. Remove a sufficiently small outward-flow neighborhood of it from $\mathcal K$. This leaves a compact trapping region containing no equilibria. The [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) gives a periodic omega-limit orbit of a nonequilibrium trajectory, hence a [limit cycle](../../../../../limit-cycle.md). The analytic vector field excludes an accumulating family of periodic return-map zeros unless the whole local return map is the identity, which is incompatible with the repelling equilibrium and the nonperiodic approaching trajectory. This is the [positive trapping construction for the Leslie-Gower model](../../../../../positive-trapping-construction-for-the-leslie-gower-model.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
