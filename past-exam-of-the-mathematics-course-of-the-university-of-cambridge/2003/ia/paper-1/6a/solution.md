<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

For a [linear map](../../../../../linear-map.md) $\alpha$, its [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) and [image of a linear map](../../../../../image-of-a-linear-map.md) are

$$
K=\{x\in\mathbb R^3:\alpha x=0\},\qquad I=\{\alpha x:x\in\mathbb R^3\}.
$$

By the definition of the image, $\alpha x=y$ has a solution exactly when $y\in I$. If $x_0$ is one solution, every other solution is $x_0+k$ for some $k\in K$: subtracting the two equations proves necessity, and linearity proves sufficiency. Thus a solvable equation has a unique solution exactly when $K=\{0\}$.

Write the columns of the given matrix as $c_1=(1,0,1)^T$, $c_2=(1,t,t)^T$ and $c_3=(t,-2b,0)^T$. Its [determinant](../../../../../determinant.md) is

$$
\det\alpha=-t^2+2bt-2b=-D,\qquad D=t^2-2bt+2b.
$$

The columns $c_1,c_2$ are [linearly independent](../../../../../linear-independence.md) for every real $t$: proportionality would require the proportionality factor to be one from the first coordinate, then simultaneously $t=0$ from the second and $t=1$ from the third. Thus the [rank](../../../../../rank-one-quadratic-form.md) is always at least two.

If $D\ne0$, the matrix is invertible and

$$
\boxed{K=\{0\},\qquad I=\mathbb R^3.}
$$

If $D=0$, the rank is exactly two. A direct substitution verifies the nonzero kernel vector $k=(-t^2,t,t-1)^T$: its first and third row products vanish identically and its second is $D$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) then gives

$$
\boxed{K=\operatorname{span}\{(-t^2,t,t-1)^T\}.}
$$

In that case the image is the plane spanned by $c_1,c_2$. Their [cross product](../../../../../cross-product.md) is $(-t,1-t,t)^T$, so an equivalent description is

$$
\boxed{I=\operatorname{span}\{(1,0,1)^T,(1,t,t)^T\}=\{y:-ty_1+(1-t)y_2+ty_3=0\}.}
$$

These formulas include the singular case $t=b=0$, giving kernel $\mathbb R(0,0,1)$ and image $y_2=0$; no exceptional case was lost by dividing by $t$.

Finally, when $0<b<2$,

$$
D=(t-b)^2+b(2-b)>0\quad\text{for every real }t.
$$

Therefore **the equation has a unique solution for every $t$ and every $y\in\mathbb R^3$**, in particular for every $y\in I$. Outside this parameter range, the singular cases are precisely $t=b\pm\sqrt{b(b-2)}$ when that square root is real.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
