<h1 id="5b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [parametric equation of a straight line](../../../../../../parametric-equation-of-a-straight-line.md) through $a$ with unit direction $\widehat t$ is

$$
\boxed{r=a+s\widehat t,\qquad s\in\mathbb R.}
$$

If the two lines meet, then $a_1+s\widehat t_1=a_2+t\widehat t_2$ for some real $s,t$, so $a_1-a_2$ lies in the [linear span](../../../../../../linear-span.md) of their direction vectors. Its [dot product](../../../../../../dot-product.md) with their [cross product](../../../../../../cross-product.md) is consequently zero:

$$
\boxed{(a_1-a_2)\cdot(\widehat t_1\times\widehat t_2)=0.}
$$

This is not sufficient without excluding parallel lines. For instance $a_1=(0,0,0)$, $a_2=(0,1,0)$ and $\widehat t_1=\widehat t_2=(1,0,0)$ satisfy it, but the lines are distinct and never meet. For nonparallel lines the condition is sufficient, because the two directions span the plane perpendicular to their nonzero [cross product](../../../../../../cross-product.md).

For nonparallel [skew lines](../../../../../../skew-lines.md), put $n=(\widehat t_1\times\widehat t_2)/|\widehat t_1\times\widehat t_2|$. Every joining vector is $a_1-a_2+s\widehat t_1-t\widehat t_2$, with fixed component $(a_1-a_2)\cdot n$ along $n$. Its length is at least the absolute value of that component. Its perpendicular component can be canceled by a unique choice of $s,t$, since the two independent directions span $n^\perp$. This lower bound is attained, proving the [distance between skew lines](../../../../../../distance-between-skew-lines.md):

$$
\boxed{d=\frac{|(a_1-a_2)\cdot(\widehat t_1\times\widehat t_2)|}{|\widehat t_1\times\widehat t_2|}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5B](../../5b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
