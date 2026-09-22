<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [dimensionless variables](../../../../../../dimensionless-variable.md)

$$
A=\frac{a^2}{4R^2},\qquad x=\frac{r^2}{4R^2},\qquad\beta=\frac{v}{\sqrt{2gR}}.
$$

The stated $R>a/2$ gives $0<A<1$. Since $f(r)=4Rx(1-x)$, the inequality from [b](../b.md) factorizes as

$$
\boxed{D(r)=4R^3(x-A)\left[4x^2-4(1-A)x+\beta^2\right]\geq0.}
$$

The two additional possible [turning points](../../../../../../turning-point.md) are

$$
x_\pm=\frac{1-A\pm\sqrt{(1-A)^2-\beta^2}}2.
$$

They are real exactly when $\beta+A\leq1$. This exposes the intended critical value

$$
\boxed{\left(\frac{v}{\sqrt{2gR}}+\frac{a^2}{4R^2}\right)_{\rm crit}=1,}
$$

but the ordering of the initial radius $A$ relative to these roots must also be checked.

First suppose $0<A<1/3$. Then $A<(1-A)/2$. If $\beta<1-A$, the allowed branch starting at $A$ is trapped either between $x_-$ and $A$ or between $A$ and $x_-$, according to its initial direction. At the coincident-root value $\beta^2=4A(1-2A)$ it is exactly a [circular orbit](../../../../../../circular-orbit.md). For $\beta=0$, the inner radial bound is the axis rather than a nonzero [turning point](../../../../../../turning-point.md).

At $\beta=1-A$, the additional roots coalesce at $x_*=(1-A)/2>A$. The particle starts outward and approaches $x_*$, or

$$
r_*=R\sqrt{2(1-A)},
$$

without reaching it in finite time. Indeed $D$ is proportional to $(x-A)(x-x_*)^2$ and the radial [energy](../../../../../../energy-split.md) equation gives $dt/dx$ proportional to $1/|x-x_*|$ near $x_*$. Its integral diverges. This is a bounded [separatrix](../../../../../../separatrix.md) approaching an unstable [circular orbit](../../../../../../circular-orbit.md). For $\beta>1-A$, there is no outer root and the particle escapes. Thus **for $0<A<1/3$, boundedness holds exactly when $\beta+A\leq1$**, with the equality case included. At $A=1/3$, the same inequality characterizes boundedness, but equality is the exact [circular orbit](../../../../../../circular-orbit.md) at the starting radius.

**The source's weaker assumption $A<1$ is insufficient to make this single threshold a general criterion.** For $1/3<A<1/2$, the initial radius lies beyond the coalescing-root position. The transition is instead the unstable [circular orbit](../../../../../../circular-orbit.md) at

$$
\beta_{\rm circ}=2\sqrt{A(1-2A)}<1-A.
$$

Below this [speed](../../../../../../speed.md) the initial radial [acceleration](../../../../../../acceleration.md) is inward and the particle remains in the inner allowed interval. At equality it stays exactly circular; above it the initial [acceleration](../../../../../../acceleration.md) is outward and the accessible branch extends to infinity, even if $\beta+A<1$. For $A>1/2$, the [surface](../../../../../../topological-surface-split.md) slopes downward outward and every such launch escapes. At $A=1/2$, only $\beta=0$ remains at rest on the summit circle.

Consequently the complete classification for the intended azimuthal launch, including zero launch [speed](../../../../../../speed.md) and exact equilibria, is

$$
\boxed{\begin{array}{ll}
0<A\leq1/3:&\text{bounded iff }0\leq\beta\leq1-A,\\
1/3<A\leq1/2:&\text{bounded iff }0\leq\beta\leq2\sqrt{A(1-2A)},\\
1/2<A<1:&\text{unbounded for every }\beta\geq0.
\end{array}}
$$

For a concrete counterexample to the unqualified proposed criterion, take $A=3/4$ and $\beta=1/10$. Then $\beta+A=17/20<1$, but $f'(a)<0$ and the outward motion has no accessible outer barrier. This satisfies the printed radius assumption and escapes. A sufficient additional radius restriction for the intended threshold is $a\leq2R/\sqrt3$, with the equality and [circular orbit](../../../../../../circular-orbit.md) qualifications above.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
