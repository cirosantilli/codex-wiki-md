<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\Delta=fb$ and $v=u_1+\Delta/2$, the mean of the two wall velocities. The [zero-potential-vorticity rotating channel flow](../../../../../../zero-potential-vorticity-rotating-channel-flow.md) has $h_2=h_1-\Delta v/g$. Substitution into the [volume flux](../../../../../../volumetric-flow-rate.md) formula gives

$$
Q=b h_1v-\frac{b\Delta}{2g}v^2.
$$

The resulting quadratic equation has two roots, $v=gh_1/\Delta\pm\sqrt{g^2h_1^2/\Delta^2-2gQ/(b^2f)}$. The positive-depth condition $h_2>0$ selects the minus sign. Thus

$$
\boxed{u_1=-\frac{bf}{2}+\frac{gh_1}{bf}-\sqrt{\frac{g^2h_1^2}{b^2f^2}-\frac{2gQ}{b^2f}}.}
$$

The discarded sign would make $h_2<0$. On the retained branch $h_2=\sqrt{h_1^2-2fQ/g}$, which also shows the admissibility condition $h_1^2\ge2fQ/g$.

The depth-based specific energy at the first wall is

$$
\boxed{E(h_1;Q,b)=h_1+\frac{1}{2g}\left[-\frac{bf}{2}+\frac{gh_1}{bf}-\sqrt{\frac{g^2h_1^2}{b^2f^2}-\frac{2gQ}{b^2f}}\right]^2.}
$$

Because $\partial_y(h+u^2/(2g))=0$, this same specific energy holds everywhere across the channel at fixed $x$. Its sum with the bed elevation is the [Bernoulli function](../../../../../../bernoulli-function.md) divided by $g$. Zero [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) makes that [Bernoulli function](../../../../../../bernoulli-function.md) constant throughout the connected steady channel flow, so

$$
\boxed{E(x)+H(x)=B_0/g.}
$$

Consequently the depth-based specific energy decreases as the bed rises and increases as it falls. It is constant along a level-bed channel, even if the width varies; that width variation instead changes the wall depths and velocities compatible with the conserved [volume flux](../../../../../../volumetric-flow-rate.md) and [Bernoulli function](../../../../../../bernoulli-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
