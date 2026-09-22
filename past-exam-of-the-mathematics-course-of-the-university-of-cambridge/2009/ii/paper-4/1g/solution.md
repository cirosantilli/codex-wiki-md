<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Write an integral [binary quadratic form](../../../../../binary-quadratic-form.md) as $[a,b,c]$. For [proper equivalence of binary quadratic forms](../../../../../proper-equivalence-of-binary-quadratic-forms.md), the allowed changes of variables have [determinant](../../../../../determinant.md) one. Here is the needed reduction rather than an appeal to class-number tables. A shear $(x,y)\mapsto(x+ny,y)$ changes $b$ to $b+2an$ without changing $a$ or the [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md). Choose $n$ so $-a<b\le a$. If the resulting $c<a$, the determinant-one change $(x,y)\mapsto(-y,x)$ replaces $[a,b,c]$ by $[c,-b,a]$, strictly decreasing the positive integer leading coefficient. Repeating must terminate with $|b|\le a\le c$. If $a=c$ and $b<0$, the same rotation makes $b$ positive; the choice $-a<b\le a$ already fixes the other boundary sign. This is a [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md).

Since $4ac-b^2=67$, the reduction inequalities give $67\ge3a^2$, so $a\in\{1,2,3,4\}$. The integer $b$ is odd. For $a=1$, only $b=1$ survives the boundary convention and $c=17$. For $a=2$, $b=\pm1$ gives $c=68/8$, not an integer. For $a=3$, $b=\pm1,\pm3$ gives $68/12$ or $76/12$; for $a=4$, $b=\pm1,\pm3$ gives $68/16$ or $76/16$. None is integral. Therefore **every form is properly equivalent to $x^2+xy+17y^2$**, establishing [class number one for discriminant minus sixty-seven](../../../../../class-number-one-for-discriminant-minus-sixty-seven.md).

For infinitude, its determinant-one shears produce

$$
\boxed{f_n(x,y)=x^2+(2n+1)xy+(n^2+n+17)y^2,\qquad n\in\mathbb Z.}
$$

Each has discriminant $-67$ and is positive definite because it is a change of variables of the displayed positive form. Their middle coefficients are distinct, so they are infinitely many distinct elements of the set.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
