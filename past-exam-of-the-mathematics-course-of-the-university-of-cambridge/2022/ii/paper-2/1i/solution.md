<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

Write an integral [binary quadratic form](../../../../../binary-quadratic-form.md) as $[a,b,c]=ax^2+bxy+cy^2$. It is positive definite when $a>0$ and its [discriminant](../../../../../discriminant-of-a-binary-quadratic-form.md) $D=b^2-4ac$ is negative. Two forms are [properly equivalent](../../../../../proper-equivalence-of-binary-quadratic-forms.md) when one is obtained from the other by a change of variables in $\operatorname{SL}_2(\mathbb Z)$. A [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) satisfies

$$
|b|\leq a\leq c,
$$

with $b\geq0$ when $|b|=a$ or $a=c$.

To prove reduction, choose in a proper equivalence class a form whose positive leading coefficient $a$ is minimal. Replacing $x$ by $x+ny$ changes $b$ by $2an$, so choose $n$ to arrange $|b|\leq a$. If the resulting $c<a$, the determinant-one substitution $(x,y)\mapsto(-y,x)$ would put $c$ in the leading position, contradicting minimality. Thus $a\leq c$. Sign changes on the boundary give the stated convention. Hence every positive definite form is properly equivalent to a reduced one.

A unimodular integral substitution is a bijection of $\mathbb Z^2$, so properly equivalent forms represent exactly the same integers.

Both given forms have discriminant $-23$. Reduction gives

$$
[6,5,2]\sim[2,1,3],
\qquad
[9,25,18]\sim[2,-1,3].
$$

The two reduced forms represent the same integers because

$$
[2,-1,3](x,y)=[2,1,3](x,-y),
$$

an integral change of variables of determinant $-1$. They are not properly equivalent: the uniqueness theorem for reduced positive definite forms says that each proper class has one reduced representative, and $[2,1,3]\ne[2,-1,3]$. Therefore the original forms represent the same integers but are not equivalent in the required proper sense.

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
