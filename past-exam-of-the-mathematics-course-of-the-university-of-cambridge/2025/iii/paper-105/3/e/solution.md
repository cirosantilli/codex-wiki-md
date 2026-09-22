<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write the [Inviscid Burgers equation](../../../../../../inviscid-burgers-equation.md) in [conservation form](../../../../../../scalar-conservation-law.md) as

$$
u_t+\left(\frac{u^2}{2}\right)_x=0.
$$

A bounded function $u$ is a weak solution with initial datum $u_0$ when

$$
\int_0^\infty\!\int_{\mathbb R}
\left(u\varphi_t+\frac{u^2}{2}\varphi_x\right)dx\,dt
+\int_{\mathbb R}u_0(x)\varphi(0,x)\,dx=0
$$

for every compactly supported $C^1$ [test function](../../../../../../test-function.md) $\varphi$.

Across a straight discontinuity $x=\sigma t$, [integration by parts](../../../../../../integration-by-parts.md) on its two sides shows that the boundary terms cancel exactly when the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) holds:

$$
\sigma(u_+-u_-)=\frac{u_+^2-u_-^2}{2},
\qquad
\sigma=\frac{u_-+u_+}{2}
$$

when $u_-\ne u_+$. For every $c>0$, define

$$
u_c(t,x)=
\begin{cases}
-c,&-ct/2<x<0,\\
c,&0<x<ct/2,\\
0,&\text{otherwise}.
\end{cases}
$$

The three jumps have left and right states $(0,-c)$, $(-c,c)$, and $(c,0)$, so their Rankine-Hugoniot speeds are respectively $-c/2$, $0$, and $c/2$, exactly the speeds of the displayed lines. Hence each $u_c$ satisfies the weak equation away from the origin and across every jump. Moreover, its nonzero support at time $t$ has length $ct$, so $u_c(t,\cdot)\to0$ in $L^1_{\mathrm{loc}}$ as $t\downarrow0$; its initial datum is therefore zero in the weak identity.

The zero function and all the distinct functions $u_c$ are bounded weak solutions with the same zero initial datum. Thus weak solutions are not unique. The central jump from $-c$ to $c$ is an expansion shock, which an [entropy condition](../../../../../../entropy-solution.md) would exclude.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
