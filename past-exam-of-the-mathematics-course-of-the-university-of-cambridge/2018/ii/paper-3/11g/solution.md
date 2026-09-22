<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Write an integral [binary quadratic form](../../../../../binary-quadratic-form.md) as $[a,b,c]=ax^2+bxy+cy^2$, with [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) $D=b^2-4ac$. It is positive definite when $a>0$ and $D<0$. Two forms are [equivalent](../../../../../proper-equivalence-of-binary-quadratic-forms.md) if one is obtained from the other by an integral linear change of variables whose matrix lies in $\operatorname{SL}_2(\mathbb Z)$. A positive definite form is [reduced](../../../../../reduced-positive-definite-binary-quadratic-form.md) when

$$
|b|\leq a\leq c,
$$

with $b\geq0$ when $|b|=a$ or $a=c$.

To reduce a form, apply a unimodular shear $x\mapsto x+ny$ with $n$ chosen so that the new middle coefficient has $|b'|\leq a$. If the new final coefficient $c'$ is smaller than $a$, exchange the variables, using a determinant-one rotation, so that the positive leading coefficient decreases from $a$ to $c'$. Repeating must stop because a positive integer cannot decrease indefinitely. At termination $|b|\leq a\leq c$, and elementary sign changes impose the boundary convention. This is the [reduction algorithm for a positive definite binary quadratic form](../../../../../reduction-algorithm-for-a-positive-definite-binary-quadratic-form.md), and proves that every positive definite form is equivalent to a reduced one.

The displayed forms have discriminant $1-36=-35$, so the intended discriminant is $-35$. For any reduced form of this discriminant, [enumeration of reduced binary quadratic forms](../../../../../enumeration-of-reduced-binary-quadratic-forms.md) gives

$$
1\leq a\leq\sqrt{\frac{35}{3}}<4,\qquad |b|\leq a,
\qquad c=\frac{b^2+35}{4a}\in\mathbb Z.
$$

The boundary convention and direct checking of $a=1,2,3$ leave only

$$
\boxed{f_1=[1,1,9]=x^2+xy+9y^2,\qquad
f_2=[3,1,3]=3x^2+xy+3y^2.}
$$

Suppose first that a prime $p>7$ is represented by $f_1$. The identity

$$
4f_1(x,y)=(2x+y)^2+35y^2
$$

shows modulo both $5$ and $7$ that $4p$ is a nonzero square. Hence

$$
\left(\frac p5\right)=\left(\frac p7\right)=1.
$$

Similarly,

$$
12f_2(x,y)=(6x+y)^2+35y^2.
$$

Modulo $5$, this says $2p$ is a square, while modulo $7$ it says $5p$ is a square. Since $(2/5)=(5/7)=-1$, the [multiplicativity of the Legendre symbol](../../../../../multiplicativity-of-the-legendre-symbol.md) gives

$$
\left(\frac p5\right)=\left(\frac p7\right)=-1.
$$

Conversely, suppose the two displayed [Legendre symbols](../../../../../legendre-symbol.md) have the same sign. By [quadratic reciprocity](../../../../../quadratic-reciprocity.md),

$$
\left(\frac{-35}{p}\right)
=\left(\frac p5\right)\left(\frac p7\right)=1.
$$

Choose an odd integer $B$ satisfying $B^2\equiv-35\pmod p$. Since $B$ is odd, $B^2+35$ is also divisible by $4$, so

$$
F=\left[p,B,\frac{B^2+35}{4p}\right]
$$

is a positive definite integral form of discriminant $-35$ that represents $p$. Reducing $F$ yields either $f_1$ or $f_2$, and equivalence preserves represented integers. The necessary symbol calculation above determines which one: the positive pair selects $f_1$, and the negative pair selects $f_2$. Therefore

$$
\boxed{
p\text{ is represented by }f_i
\iff
\left(\frac p5\right)=\left(\frac p7\right)
=
\begin{cases}
+1,&i=1,\\
-1,&i=2.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
