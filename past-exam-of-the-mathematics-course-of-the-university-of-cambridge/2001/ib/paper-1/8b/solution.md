<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

The [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) is $d=b^2-4ac$. If the form is [positive-definite](../../../../../positive-definite-bilinear-form.md), evaluating it at $(1,0)$ gives $a>0$. For $a\ne0$, [completing the square](../../../../../completing-the-square.md) gives

$$
q(x,y)=a\left(x+\frac b{2a}y\right)^2+\frac{4ac-b^2}{4a}y^2.
$$

Evaluating along $x=-by/(2a)$ shows that positivity also requires $d<0$. Conversely these two inequalities make both displayed coefficients positive, proving

$$
\boxed{q\text{ is positive definite}\Longleftrightarrow a>0>d}.
$$

A [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) satisfies $|b|\leq a\leq c$, with $b\geq0$ if $|b|=a$ or $a=c$. The last convention avoids counting both boundary representatives. For fixed negative [discriminant](../../../../../discriminant.md), these inequalities imply

$$
|d|=4ac-b^2\geq3a^2,\qquad 1\leq a\leq\sqrt{|d|/3}.
$$

There are finitely many such integers $a$, finitely many integers $b$ with $|b|\leq a$, and then $c=(b^2-d)/(4a)$ is determined. Hence **the number of reduced forms is finite**. If no admissible integer coefficients have the given [discriminant](../../../../../discriminant.md), this number is zero.

For $d=-39$, the bound gives $a=1,2,3$. The integrality of $c=(b^2+39)/(4a)$ and the boundary sign convention give respectively

$$
(a,b,c)=(1,1,10),\quad(2,1,5),(2,-1,5),\quad(3,3,4).
$$

These are all the [reduced positive definite binary quadratic forms of discriminant minus thirty-nine](../../../../../reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-nine.md). Thus

$$
\boxed{h(-39)=4},
$$

represented by $x^2+xy+10y^2$, $2x^2+xy+5y^2$, $2x^2-xy+5y^2$, and $3x^2+3xy+4y^2$.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
