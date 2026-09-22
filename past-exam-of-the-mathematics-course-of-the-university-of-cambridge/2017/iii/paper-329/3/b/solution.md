<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is a squeezing motion, not the rotational motion of the previous part. The gap changes at rate $h_t=V\sin\theta$. The [Reynolds lubrication equation](../../../../../../reynolds-equation.md) therefore gives

$$
\frac1a q_\theta=-h_t,\qquad q=aV\cos\theta+C.
$$

The outer wall also has tangential speed $V\cos\theta$, but its local [Couette flow](../../../../../../couette-flow.md) flux is $O(V\Delta)$ compared with the squeezing flux $O(Va)$ and does not affect the leading [force](../../../../../../force.md). Thus $p_\theta=-12\mu a q/h^3$ at leading order. Periodic [pressure](../../../../../../pressure.md) gives $C=0$, because the [integral](../../../../../../integral.md) of $\cos\theta/h^3$ vanishes over a full circle. Balancing [pressure](../../../../../../pressure.md) traction on the fixed inner cylinder and using [integration by parts](../../../../../../integration-by-parts.md),

$$
F_z=a\int_0^{2\pi}p\sin\theta\,d\theta
=a\int_0^{2\pi}p_\theta\cos\theta\,d\theta
=-\frac{12\mu a^3V}{\Delta^3}\int_0^{2\pi}\frac{\cos^2\theta}{(1+\alpha\sin\theta)^3}\,d\theta.
$$

The supplied [integral](../../../../../../integral.md) gives the [squeeze resistance of an eccentric journal bearing](../../../../../../squeeze-resistance-of-an-eccentric-journal-bearing.md):

$$
\boxed{F_z=-\frac{12\pi\mu a^3V}{\Delta^3(1-\alpha^2)^{3/2}}.}
$$

The fluid tends to pull the inner cylinder upwards with the moving outer wall, so a downward holding [force](../../../../../../force.md) is required when $V>0$. At concentricity the translation resistance is $R_0=12\pi\mu a^3/\Delta^3$. The omitted wall-tangential flux and shear traction give smaller thin-gap contributions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
