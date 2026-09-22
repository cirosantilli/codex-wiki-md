<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

For an integral [binary quadratic form](../../../../../binary-quadratic-form.md) $[a,b,c]=ax^2+bxy+cy^2$ with $a>0$ and $D=b^2-4ac<0$, the [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) convention is $|b|\le a\le c$, with $b\ge0$ on either boundary $|b|=a$ or $a=c$. Since $|D|=4ac-b^2\ge3a^2$, the [enumeration of reduced binary quadratic forms](../../../../../enumeration-of-reduced-binary-quadratic-forms.md) for $D=-23$ has $a\le\sqrt{23/3}<3$. The integer $b$ is odd. For $a=1$, only $b=1$ is retained and $c=6$; for $a=2$, both $b=\pm1$ give $c=3$. Thus the complete list is

$$
\boxed{x^2+xy+6y^2,\qquad2x^2+xy+3y^2,\qquad2x^2-xy+3y^2.}
$$

A proper representation of a prime uses a primitive representing vector. Completing that vector to a matrix in $\operatorname{SL}_2(\mathbb Z)$ transforms a representing form to $[p,b,c]$, so its [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) gives $b^2\equiv-23\pmod p$. Conversely, choose an odd $b$ satisfying this congruence and put $c=(b^2+23)/(4p)$. This is integral, and $[p,b,c]$ is positive definite and represents $p$ at $(1,0)$. This proves the [discriminant criterion for prime representation by a binary quadratic form](../../../../../discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form.md) here.

For $p\ne23$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives $(-23/p)=(p/23)$. Including the ramified prime, the answer is therefore

$$
\boxed{p=23\quad\text{or}\quad p\bmod23\in\{1,2,3,4,6,8,9,12,13,16,18\}.}
$$

For example $[23,23,6]$ supplies a proper representation of $23$. Reduction transfers every such representation to one of the three displayed forms.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
