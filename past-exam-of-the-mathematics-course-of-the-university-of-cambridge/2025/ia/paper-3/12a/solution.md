<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

The product rule gives

$$
\partial_j(T_{ij}v_i)=(\partial_jT_{ij})v_i+T_{ij}\partial_jv_i.
$$

Integrating and applying the divergence theorem proves the identity.

Here $\operatorname{div}T=4(x,y,z)$ and $v=x(x,y,z)$, so

$$
\int_V\operatorname{div}T\cdot v\,dV
=4\int_Vx(x^2+y^2+z^2)\,dV=\frac73.
$$

On the boundary, $(Tn)\cdot v=x(x\cdot n)(x^2+y^2+z^2-1)$. The nonzero contributions from the faces $x=1,y=1,z=1$ are respectively $2/3,5/12,5/12$, totaling $3/2$.

Finally, direct contraction gives

$$
T_{ij}\partial_jv_i=2x(x^2+y^2+z^2)-4x,
$$

whose [integral](../../../../../integral.md) is $-5/6$. Thus the right side is $3/2-(-5/6)=7/3$, equal to the left side.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
