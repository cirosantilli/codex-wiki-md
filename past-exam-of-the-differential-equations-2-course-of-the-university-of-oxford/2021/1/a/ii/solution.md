<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [homogeneous solution](../../../../../homogeneous-solution.md) is $A\cos x+B\sin x$. The left [boundary condition](../../../../../boundary-condition.md) removes $A$, and the right [boundary condition](../../../../../boundary-condition.md) gives $B\sin l=0$. Thus the [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) associated with this [boundary value problem](../../../../../boundary-value-problem-split.md) is

$$
\boxed{\ker\mathcal L=
\begin{cases}
\{0\},&l\notin\pi\mathbb N_{>0},\\
\operatorname{span}\{\sin x\},&l=m\pi,\quad m\in\mathbb N_{>0}.
\end{cases}}
$$

The [Fredholm alternative](../../../../../fredholm-alternative.md) now gives the complete classification:

$$
\boxed{\begin{array}{c|c|c}
l&\text{condition on }f&\text{solutions}\\\hline
l\notin\pi\mathbb N_{>0}&\text{any prescribed }f&\text{exactly one}\\
l=m\pi&\displaystyle\int_0^{m\pi}f(x)\sin x\,dx=0&\text{infinitely many}\\
l=m\pi&\displaystyle\int_0^{m\pi}f(x)\sin x\,dx\ne0&\text{none}.
\end{array}}
$$

For necessity at $l=m\pi$, multiply by the [homogeneous solution](../../../../../homogeneous-solution.md) $\sin x$ and use the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md) to obtain $\int_0^lf\sin x\,dx=0$. For sufficiency, the [particular solution](../../../../../particular-solution.md)

$$
z(x)=\int_0^x\sin(x-t)f(t)\,dt
$$

satisfies $z(0)=0$ and $z''+z=f$. At the other endpoint,

$$
z(m\pi)=(-1)^{m+1}\int_0^{m\pi}\sin t\,f(t)\,dt,
$$

which is zero under the compatibility condition. All solutions are then $z+B\sin x$, with $B$ arbitrary. The assumed [Lipschitz continuity](../../../../../lipschitz-continuity.md) of $f$ in particular makes $f$ continuous, so the displayed [integral](../../../../../integral-split.md) defines a classical solution. The length $l=0$ is excluded: it would not define a nonempty interval for this [boundary value problem](../../../../../boundary-value-problem-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
