<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

A [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) $ax^2+bxy+cy^2$ satisfies $|b|\leq a\leq c$, with $b\geq0$ when $|b|=a$ or $a=c$. These inequalities select representatives under [proper equivalence of binary quadratic forms](../../../../../proper-equivalence-of-binary-quadratic-forms.md); the changes of variables have integer entries and [determinant](../../../../../determinant.md) $1$.

For the first [binary quadratic form](../../../../../binary-quadratic-form.md), put $x=u-v$, $y=v$. For the second, put $x=-u-3v$, $y=u+2v$. Both changes preserve [coprime integers](../../../../../coprime-integers.md), and give

$$
f=3u^2+2uv+4v^2=3(u+v/3)^2+\frac{11}{3}v^2,\qquad g=u^2+11v^2.
$$

Proper representation means using $\gcd(u,v)=1$. For $f$, $|v|\geq2$ gives a value greater than $5$, while $v=0$ forces $u=\pm1$. For $|v|=1$, the smallest values are $4$ and $5$. For $g$, $v=0$ again gives only $1$ primitively; $|v|=1$ gives $11,12,15,\ldots$, and $|v|\geq2$ gives at least $44$. Thus **the three smallest properly represented values** are

$$
\boxed{f:3,4,5;\qquad g:1,11,12.}
$$

For example the original variables can be chosen as $(1,0),(-1,1),(-2,1)$ for $f$, and $(-1,1),(-3,2),(-4,3)$ for $g$.

Every positive definite [binary quadratic form](../../../../../binary-quadratic-form.md) can be reduced: integer shears first make $|b|\leq a$, and interchanging the variables when $c<a$ decreases the positive leading coefficient, so this procedure terminates. To enumerate the [reduced forms of discriminant minus forty-four](../../../../../reduced-forms-of-discriminant-minus-forty-four.md), reduction gives $3a^2\leq44$, hence $1\leq a\leq3$. Checking $b^2-4ac=-44$ with the reduced inequalities gives exactly

$$
(1,0,11),\quad(2,2,6),\quad(3,2,4),\quad(3,-2,4).
$$

The second represents only even integers. The last two have the same represented values, by $u\mapsto-u$. The first and third are the reduced versions of $g$ and $f$. Therefore **every represented odd integer occurs in at least one of $f,g$**, whether or not its original representation was primitive.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
