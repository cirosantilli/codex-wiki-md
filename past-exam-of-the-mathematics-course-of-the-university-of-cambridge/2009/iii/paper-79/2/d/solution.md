<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A failed dam launches a [rarefaction wave](../../../../../../rarefaction-wave.md) back into the reservoir and an advancing current into the initially dry downstream channel. Take the failed dam as $x=0$, initial depth $h_0$ and zero velocity for $x<0$, and a dry bed for $x>0$. Locally assume a flat, prismatic triangular section, $S=Ch^2$. The early flow is governed by

$$
h_t+uh_x+\frac h2u_x=0,\qquad u_t+uu_x+gh_x=0,
\qquad c=\sqrt{gh/2}.
$$

Its [Riemann invariants](../../../../../../riemann-invariant.md) are $u\pm4c$, since $\int(g/c)dh=4c$. In the left-running simple wave, $u+4c=4c_0$, where $c_0=\sqrt{gh_0/2}$, and the expanding fan has $x/t=u-c$. Solving gives

$$
c=\frac{4c_0-x/t}{5},\qquad u=\frac45(c_0+x/t).
$$

Thus the [triangular-channel dry-bed dam break](../../../../../../triangular-channel-dry-bed-dam-break.md) profile is

$$
\boxed{h(x,t)=\begin{cases}
h_0,&x/t\leq-c_0,\\
h_0\left(\dfrac{4-x/(c_0t)}5\right)^2,&-c_0<x/t<4c_0,\\
0,&x/t\geq4c_0.
\end{cases}}
$$

The reservoir-side edge moves at $-c_0$, and the dry front moves at

$$
\boxed{U_f=4c_0=2\sqrt{2gh_0}.}
$$

Velocity is zero in the undisturbed reservoir and has the fan value above where water is present. This approximation applies before the rarefaction reaches the surviving dam and before channel variation, friction or finite-volume reflections substantially modify the flow. If water is already present downstream, a bore replaces the dry-bed front and requires a different matching problem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
