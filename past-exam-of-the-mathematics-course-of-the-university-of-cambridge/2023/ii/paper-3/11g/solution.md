<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Write an integral [binary quadratic form](../../../../../binary-quadratic-form.md) as

$$
[a,b,c](x,y)=ax^2+bxy+cy^2,
\qquad
d=b^2-4ac<0.
$$

A positive definite form is a [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) when

$$
|b|\leq a\leq c,
$$

with $b\geq0$ on the boundary $|b|=a$ or $a=c$. The [class number of a negative discriminant](../../../../../class-number-of-a-negative-discriminant.md) $h(d)$ is the number of [proper equivalence classes](../../../../../proper-equivalence-of-binary-quadratic-forms.md) of primitive positive definite integral forms of discriminant $d$.

Every such class has a reduced representative. For a reduced form,

$$
4a^2\leq4ac=b^2+|d|\leq a^2+|d|,
$$

so

$$
a\leq\sqrt{\frac{|d|}{3}}.
$$

There are only finitely many possible integers $a$ and $b$, and then

$$
c=\frac{b^2-d}{4a}
$$

is determined. Hence $h(d)<\infty$. There is at least one class: the principal form is

$$
[1,0,-d/4]\quad\hbox{if }d\equiv0\pmod4,
$$

and

$$
[1,1,(1-d)/4]\quad\hbox{if }d\equiv1\pmod4.
$$

Thus $1\leq h(d)<\infty$, in agreement with the [enumeration of reduced binary quadratic forms](../../../../../enumeration-of-reduced-binary-quadratic-forms.md).

Now let $q\equiv3\pmod8$ be prime. The two forms

$$
f_0=[1,0,2q],
\qquad
f_1=[2,0,q]
$$

are primitive, positive definite, reduced, and have discriminant $-8q$. They are not [properly equivalent](../../../../../proper-equivalence-of-binary-quadratic-forms.md): $f_0$ represents one, while the least positive value of $f_1$ is two. Therefore

$$
\boxed{h(-8q)\geq2.}
$$

Assume henceforth that $h(-8q)=2$, so these are the only two classes. If

$$
p=x^2+2qy^2
$$

for a prime $p>q$, then $x$ is odd and

$$
p\equiv x^2+6y^2\equiv
\begin{cases}
1\pmod8,&y\text{ even},\\
7\pmod8,&y\text{ odd}.
\end{cases}
$$

Moreover $p\equiv x^2\pmod q$, so $p$ is a [quadratic residue](../../../../../quadratic-residue.md) modulo $q$. This proves the necessity.

Conversely, suppose $p\equiv\pm1\pmod8$ and $p$ is a quadratic residue modulo $q$. By [quadratic reciprocity](../../../../../quadratic-reciprocity.md), these two conditions imply

$$
\left(\frac{-8q}{p}\right)=1.
$$

Indeed, for $p\equiv1\pmod8$ both relevant signs are positive, while for $p\equiv7\pmod8$ the signs from $(-8/p)$ and reciprocity with $q\equiv3\pmod4$ cancel. Choose an even integer $b$ such that

$$
b^2\equiv-8q\pmod{4p}.
$$

Then

$$
[p,b,c],
\qquad
c=\frac{b^2+8q}{4p},
$$

is a primitive positive definite integral form of discriminant $-8q$ and represents $p$. It belongs to one of the two classes $f_0,f_1$.

The second form cannot represent such a prime. If

$$
p=2x^2+qy^2,
$$

then $y$ is odd and, since $q\equiv3\pmod8$,

$$
p\equiv
\begin{cases}
3\pmod8,&x\text{ even},\\
5\pmod8,&x\text{ odd}.
\end{cases}
$$

This contradicts $p\equiv\pm1\pmod8$. Hence $[p,b,c]$ lies in the principal class $f_0$, and [proper equivalence of binary quadratic forms](../../../../../proper-equivalence-of-binary-quadratic-forms.md) preserves represented integers. Therefore

$$
\boxed{
p=x^2+2qy^2
\quad\Longleftrightarrow\quad
p\equiv\pm1\pmod8
\ \hbox{and}\
\left(\frac pq\right)=1.}
$$

This is the [prime representation when h of minus eight q equals two](../../../../../prime-representation-when-h-of-minus-eight-q-equals-two.md).

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
