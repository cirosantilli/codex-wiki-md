<h1 id="22i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F(y)=y_1^2y_2+y_2^2y_3+y_3^2y_1$. The [proper transform](../../../../../../strict-transform.md) is

$$
\boxed{\widetilde Y=\{(x,[y]):x_iy_j=x_jy_i\ (i<j),\ F(y)=0\}\subset\mathbb A^3\times\mathbb P^2.}
$$

Indeed, in the blowup chart $y_i\ne0$, write $x=t y$ with $y_i=1$. Homogeneity gives $F(x)=t^3F(y)$. Away from the [exceptional divisor](../../../../../../exceptional-divisor.md) $t=0$, the equation is $F(y)=0$, and its closure retains that equation, removing the exceptional factor $t^3$. Every point with $t=0,F(y)=0$ is approached algebraically along the line $(t y,[y])$, so no component in this displayed [set](../../../../../../set-split.md) is extraneous.

For $x\ne0$, the fibre is the single point $[y]=[x]$, and the projection is an [isomorphism](../../../../../../isomorphism.md) over $Y\setminus\{0\}$. Over $0$ the fibre is the projective plane cubic $F(y)=0$. In characteristic zero this cubic is smooth: a coordinate zero in the three [derivative](../../../../../../derivative.md) equations would force all coordinates zero; with all nonzero, multiplying $2y_1y_2=-y_3^2$, $y_1^2=-2y_2y_3$, $y_2^2=-2y_3y_1$ gives $1=-8$, impossible. Thus **the exceptional fibre is a smooth [genus](../../../../../../genus-of-a-surface.md)-one plane cubic**. The fibre description itself does not require this optional smoothness conclusion; characteristic $3$ requires separate treatment.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22I](../../22i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
