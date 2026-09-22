<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [fixed points](../../../../../fixed-point.md) satisfy $x[rx(1-x)-1]=0$. There is always $x=0$, and the other branches are

$$
x_\pm(r)=\frac{1\pm\sqrt{1-4/r}}2,\qquad r\ge4.
$$

They coincide at $(r,x)=(4,1/2)$. For $0<x<1$, $F(x)>0$ and its maximum occurs at $x=2/3$, with value $4r/27$. Consequently $\boxed{F((0,1))\subset(0,1)\iff0<r<27/4}$; equality at the upper endpoint fails because the maximum is attained inside the interval.

The [fixed-point multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) at zero is zero, so zero is attracting for every $r>0$. On either nonzero branch,

$$
F'(x)=\frac{2-3x}{1-x}.
$$

The lower branch has multiplier greater than one for $r>4$ and is repelling. The upper branch is attracting for $4<r<16/3$, reaches multiplier $-1$ at $x=3/4$, and is repelling for $r>16/3$. At $r=4$ the multiplier is $+1$, and the two branches are created in a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md). The fixed point there is attracting from one side and repelling from the other: $F(x)-x=-4x(x-1/2)^2$.

The second change is a supercritical [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md) at $\boxed{(r,x)=(16/3,3/4)}$. To check its type, expand at that fixed point. The local map has quadratic coefficient $a=-20/3$ and cubic coefficient $b=-16/3$ when the multiplier is $-1$. Its second iterate has cubic coefficient $-2(a^2+b)=-704/9<0$. The multiplier decreases through $-1$ as $r$ increases, so a small attracting two-cycle is born on the $r>16/3$ side. These exhaust the fixed-point [bifurcations](../../../../../bifurcation.md), since their multipliers have no other crossings of $\pm1$.

<a id="7e/image-fixed-point-branches-of-the-cubic-map-with-attracting-solid-curves-and-repelling-dashed-curves"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3-map-bifurcation.png)

**[Figure 1](#7e/image-fixed-point-branches-of-the-cubic-map-with-attracting-solid-curves-and-repelling-dashed-curves). Fixed-point branches of the cubic map, with attracting solid curves and repelling dashed curves**.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
