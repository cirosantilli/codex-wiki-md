<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Orient the triangular boundary from $P=(1,0,0)$ to $Q=(0,1,0)$ to $R=(0,0,1)$ and back to $P$. This orientation corresponds to the positive [normal vector](../../../../../normal-vector.md) $(Q-P)\times(R-P)=(1,1,1)$. The cyclic coordinate rotation $(x,y,z)\mapsto(z,x,y)$ sends the three directed edges to one another and transforms the [vector field](../../../../../vector-field.md) by the same rotation. Since rotations preserve [dot products](../../../../../dot-product.md), the three edge contributions to the [line integral](../../../../../line-integral.md) are equal.

On the first edge use $x=1-t$, $y=t$, $z=0$, $0\le t\le1$. Then

$$
A\cdot\frac{d\mathbf x}{dt}=(-t^2,(1-t)^2,t^2-(1-t)^2)\cdot(-1,1,0)=t^2+(1-t)^2.
$$

Its integral is $2/3$, so the required [circulation](../../../../../circulation-physics.md) is

$$
\boxed{\oint_C A\cdot d\mathbf x=3\cdot\frac23=2}.
$$

For a sufficiently smooth [vector field](../../../../../vector-field.md) on an oriented piecewise smooth surface $T$, with induced boundary orientation on $C=\partial T$, the [Stokes theorem](../../../../../stokes-theorem.md) states

$$
\int_T(\nabla\times A)\cdot n\,dS=\oint_C A\cdot d\mathbf x.
$$

Therefore the requested [surface integral](../../../../../surface-integral.md), with all normal components positive, is also **$2$**.

To verify it directly, parametrize the triangle by $\mathbf r(y,z)=(1-y-z,y,z)$ on $y\ge0$, $z\ge0$, $y+z\le1$. Its two tangent vectors are $\mathbf r_y=(-1,1,0)$ and $\mathbf r_z=(-1,0,1)$, giving the [vector area element](../../../../../vector-area-element.md)

$$
\boxed{d\mathbf S=(\mathbf r_y\times\mathbf r_z)\,dy\,dz=(1,1,1)\,dy\,dz}.
$$

Differentiation of the [vector field](../../../../../vector-field.md) gives $\nabla\times A=2(y+z,z+x,x+y)$. On the triangle $x+y+z=1$, so its [dot product](../../../../../dot-product.md) with $(1,1,1)$ is $4$. Consequently

$$
\int_T(\nabla\times A)\cdot d\mathbf S=\int_0^1\int_0^{1-y}4\,dz\,dy=2,
$$

confirming both the magnitude and the orientation sign.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
