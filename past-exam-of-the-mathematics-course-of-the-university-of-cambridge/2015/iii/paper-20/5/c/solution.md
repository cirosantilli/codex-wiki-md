<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The hyperplane sections through $P$ are spanned by the three linear forms $x_1,x_2,x_0-x_3$. Their common zero on $X$ is precisely $P$, so away from $P$ the [linear system of divisors](../../../../../../linear-system-of-divisors.md) is base-point-free and defines the [projection from a point on a smooth quadric](../../../../../../projection-from-a-point-on-a-smooth-quadric.md)

$$
\boxed{\varphi([x_0:x_1:x_2:x_3])=[x_1:x_2:x_0-x_3].}
$$

In particular, the chart-ratio construction in part (a) makes this a [morphism of schemes](../../../../../../morphism-of-schemes.md) on $X\setminus\{P\}$, not merely a rational map there.

Write a target point as $[u:v:w]$. The corresponding line through $P$ consists of points

$$
[\lambda+\mu w:\mu u:\mu v:\lambda].
$$

Substituting in the quadric equation gives

$$
\mu\bigl((u-v)\lambda+uw\mu\bigr)=0.
$$

Removing $P$ means $\mu\ne0$, so set $\mu=1$. Over the [residue field](../../../../../../residue-field.md) $K$ of the target point, its [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) is consequently

$$
\boxed{\operatorname{Spec}K[\lambda]/\bigl((u-v)\lambda+uw\bigr).}
$$

If $u\ne v$, this is one reduced point, with $\lambda=-uw/(u-v)$. If $u=v$ and $uw\ne0$, it is empty: the corresponding line meets the quadric only at the removed point, with intersection multiplicity two. If $u=v$ and $uw=0$, the line lies entirely on the quadric, and the [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) is $\mathbb A^1_K$, the line with $P$ removed.

The last case occurs at exactly $[0:0:1]$ and $[1:1:0]$. Their lines are respectively

$$
L_1=\{x_1=x_2=0\},\qquad L_2=\{x_0=x_3,\ x_1=x_2\},
$$

the two [rulings of a smooth quadric surface](../../../../../../rulings-of-a-smooth-quadric-surface.md) through $P$. Thus the image consists of the complement of the line $u=v$, together with those two points. The line $u=v$ parametrizes directions in the tangent plane $x_1=x_2$ at $P$. The calculation describes the [scheme-theoretic fibres](../../../../../../scheme-theoretic-fibre.md) over arbitrary target points and works in every characteristic.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
