<h1 id="11b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $u=(-y,x,\alpha)$, one has $\nabla\cdot u=0$, and therefore

$$
a_i=\partial_j(u_iu_j)
=(u\cdot\nabla)u_i
=(-x,-y,0)_i.
$$

Close the upper half-ellipsoid with its unit-disk base $D$ in the plane $z=0$. By symmetry,

$$
\int_V(-x,-y,0)\,dV=0.
$$

On the base, the outward normal is $n=(0,0,-1)$, so

$$
u_iu_jn_j=-\alpha u_i
=(\alpha y,-\alpha x,-\alpha^2)_i.
$$

The first two components integrate to zero over the disk, while the third integrates to $-\pi\alpha^2$. The closed-surface tensor identity therefore gives

$$
\int_Su_iu_jn_j\,dS
=(0,0,\pi\alpha^2)_i.
$$

Multiplying by $\beta^2$,

$$
\boxed{F=(0,0,\pi\alpha^2\beta^2)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
