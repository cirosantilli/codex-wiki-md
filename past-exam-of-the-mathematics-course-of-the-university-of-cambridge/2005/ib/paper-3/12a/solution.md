<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

Project from the north pole $N=(0,0,1)$ along the line through a sphere point onto the equatorial plane $Z=0$, identified with $\mathbb C$. Parameterizing this line gives

$$
\boxed{\pi(X,Y,Z)=\frac{X+iY}{1-Z},\qquad\pi(N)=\infty}.
$$

The inverse [stereographic projection](../../../../../stereographic-projection.md) is

$$
(X,Y,Z)=\frac{(2\operatorname{Re}z,2\operatorname{Im}z,|z|^2-1)}{1+|z|^2}.
$$

Negating the three sphere coordinates consequently sends $z$ to $-1/\bar z$, with $0,\infty$ interchanged. This proves the [antipodal stereographic coordinate relation](../../../../../antipodal-stereographic-coordinate-relation.md).

A nonidentity [Möbius transformation](../../../../../mobius-transformation.md) $T(z)=(az+b)/(cz+d)$ has $ad-bc\ne0$. For $c\ne0$, its fixed points are the roots of $cz^2+(d-a)z-b=0$, giving one or two distinct points. If $c=0$ and $a\ne d$, there is one finite root and the fixed point infinity. If $c=0$, $a=d$, and $b\ne0$, it is a translation and only infinity is fixed. The remaining case is the identity, already excluded. Thus the claim includes fixed points at infinity, not just finite solutions of the quadratic.

A nontrivial rotation of the sphere fixes exactly the two poles on its axis, which are antipodal. It therefore gives exactly two fixed stereographic points with $z_2=-1/\bar z_1$. Here the nonzero rotation angle is understood modulo $2\pi$; an angle that is a whole multiple of $2\pi$ would be the identity.

Conversely, use a sphere rotation whose Möbius map $S$ sends the two antipodal fixed points to $0,\infty$. The conjugate $STS^{-1}$ fixes both, hence equals $z\mapsto az$ for some $a\ne0$. If $|a|=1$, write $a=e^{i\theta}$; the inverse stereographic formula shows that this rotates $X+iY$ while leaving $Z$ fixed. Conjugating back by the rotation $S$ gives a sphere rotation. If $|a|<1$, $a^nz\to0$ for every finite $z$. If $|a|>1$, $a^nz\to\infty$ for every $z\ne0$, in the sphere topology. Pulling these conclusions back proves the [antipodal fixed-point classification of Möbius transformations](../../../../../antipodal-fixed-point-classification-of-mobius-transformations.md): **either the map is a sphere rotation or one fixed point attracts every point except the other fixed point**.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
