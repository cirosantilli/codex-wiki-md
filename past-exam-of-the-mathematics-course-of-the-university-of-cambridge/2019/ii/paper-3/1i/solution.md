<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

A [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) $f=[a,b,c]=ax^2+bxy+cy^2$ satisfies

$$
|b|\leq a\leq c,
$$

with $b\geq0$ when $|b|=a$ or $a=c$. Its [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) is $d=b^2-4ac<0$. The first displayed inequality already gives $|b|\leq a$, while $c\geq a$ gives

$$
|d|=4ac-b^2\geq4a^2-a^2=3a^2.
$$

Taking the positive [square root](../../../../../square-root.md) yields

$$
\boxed{|b|\leq a\leq\sqrt{|d|/3}.}
$$

Moreover, $d=b^2-4ac\equiv b^2\equiv b\pmod2$, so $b\equiv d\pmod2$. For fixed negative $d$, the displayed bounds leave only [finitely many](../../../../../finite-set.md) possible [integers](../../../../../integer.md) $a$ and $b$, and then $c=(b^2-d)/(4a)$ is uniquely determined. Hence only finitely many reduced forms have discriminant $d$.

For $d=-15$, the bound gives $a\leq\sqrt5$, so $a\in\{1,2\}$. The [modular congruence](../../../../../modular-congruence.md) condition makes $b$ [odd](../../../../../odd-number.md). If $a=1$, then $b=\pm1$ and $c=4$; the boundary convention $|b|=a\Rightarrow b\geq0$ retains $[1,1,4]$. If $a=2$, then $b=\pm1$ and $c=2$; the boundary convention $a=c\Rightarrow b\geq0$ retains $[2,1,2]$. Thus the complete list is

$$
\boxed{[1,1,4],\qquad [2,1,2].}
$$

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
