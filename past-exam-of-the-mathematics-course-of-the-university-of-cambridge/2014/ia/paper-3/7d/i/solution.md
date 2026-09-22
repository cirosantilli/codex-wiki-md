<h1 id="7d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Identify the [projective line](../../../../../../projective-line.md) with one-dimensional subspaces of $\mathbb F_p^2$: use $v_t=(t,1)^T$ for finite $t$, and $v_\infty=(1,0)^T$. This convention turns the [matrix](../../../../../../matrix.md) action into the stipulated [Möbius transformation](../../../../../../mobius-transformation.md).

Since $x$ and $z$ are distinct projective points, $v_z,v_x$ are a [basis](../../../../../../basis.md). Write $v_y=A v_z+B v_x$. Both $A$ and $B$ are nonzero, because $y$ is different from $x,z$. The [matrix](../../../../../../matrix.md) with columns $A v_z$ and $B v_x$ is invertible and sends the lines of $(1,0)^T,(0,1)^T,(1,1)^T$ to those of $z,x,y$, respectively. This constructs the requested map without separate exceptional formulas at infinity.

A [matrix](../../../../../../matrix.md) fixing $0$ and $\infty$ is diagonal, say $\operatorname{diag}(a,d)$ with $a,d\ne0$. To fix $1$ it must also satisfy $a=d$, so the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) of $(0,1,\infty)$ is precisely $\{\lambda I:\lambda\in\mathbb F_p^\times\}$. Any two solutions differ on the right by one of these [matrices](../../../../../../matrix.md). Thus

$$
\boxed{\text{There are exactly }p-1\text{ matrices for each distinct target triple.}}
$$

Equivalently, after dividing out [scalar matrices](../../../../../../scalar-matrix.md) the [projective general linear group action on the projective line](../../../../../../projective-general-linear-group-action-on-the-projective-line.md) is [sharply three-transitive on a projective line](../../../../../../sharply-three-transitive-on-a-projective-line.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
