<h1 id="38a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the linear test equation $f(y)=\lambda y$ put $z=h\lambda$. The second stage solves $(1-az)k_2=\lambda y[1+(1-a)z]$, and substitution into the update gives the [stability function](../../../../../../stability-function.md)

$$
\boxed{R(z)=\frac{1+(1-a)z+(1/2-a)z^2}{1-az}.}
$$

[A-stability](../../../../../../a-stability.md) requires no [poles](../../../../../../pole.md) and $|R(z)|\leq1$ throughout the closed left half-plane. If $a\ne1/2$, the quadratic numerator gives unbounded magnitude as $z\to-\infty$; when $a=0$ the denominator is constant and the same conclusion holds. Thus $a=1/2$ is necessary. At this value $R(z)=(1+z/2)/(1-z/2)$, whose only [pole](../../../../../../pole.md) is at positive $z=2$. Moreover

$$
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z\geq0
$$

on the left half-plane. Hence **the method is A-stable exactly for $\boxed{a=1/2}$**. Its limit at negative infinity is $-1$, so it is not [L-stable](../../../../../../l-stability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38A](../../38a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
