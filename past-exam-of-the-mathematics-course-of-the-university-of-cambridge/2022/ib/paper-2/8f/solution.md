<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

Let $f_1,f_2\in V^*$ satisfy $f_1(v)f_2(v)=0$ for every [vector](../../../../../vector.md) $v$. If $f_1=0$ there is nothing to prove. Otherwise choose $u$ with $f_1(u)\ne0$. For every $v\in\ker f_1$ and every [real number](../../../../../real-number.md) $t$,

$$
f_1(u+tv)=f_1(u)\ne0,
$$

so the hypothesis gives $f_2(u+tv)=0$. Taking two values of $t$ shows that $f_2(u)=f_2(v)=0$. Since

$$
V=\mathbb Ru+\ker f_1,
$$

we obtain $f_2=0$. Thus one of the two [linear functionals](../../../../../linear-functional.md) is zero.

[Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) says that, in a suitable [basis](../../../../../basis.md), every real [quadratic form](../../../../../quadratic-form.md) is

$$
q=x_1^2+\cdots+x_p^2-x_{p+1}^2-\cdots-x_{p+m}^2.
$$

The [rank](../../../../../rank-one-quadratic-form.md) is $r=p+m$, and the [signature](../../../../../signature-of-a-quadratic-form.md) is $\sigma=p-m$; both are independent of the chosen basis.

If $q=f_1f_2$, its [polar form](../../../../../polarization-identity.md) has image contained in $\operatorname{span}\{f_1,f_2\}$, so $r\leq2$. If $r=2$, the two functionals must be independent and, after taking their sum and difference, $q$ is a difference of two squares. Hence $\sigma=0$. If $r=1$, then $|\sigma|=1$. In every case,

$$
r+|\sigma|\leq2.
$$

Conversely, this inequality leaves only

$$
q=0,\qquad q=\pm x_1^2,qquad q=x_1^2-x_2^2,
$$

up to a [linear change of coordinates](../../../../../change-of-basis.md). These factor respectively as $0$, $(\pm x_1)x_1$, and $(x_1-x_2)(x_1+x_2)$. Therefore

$$
\boxed{q=f_1f_2\quad\Longleftrightarrow\quad r+|\sigma|\leq2}.
$$

Finally suppose that $q$ takes both positive and negative values. Sylvester's law supplies normalized basis vectors

$$
e_1,\ldots,e_p,\quad f_1,\ldots,f_m,\quad z_1,\ldots,z_k
$$

with $q(e_i)=1$, $q(f_j)=-1$, and the $z_l$ spanning the [radical](../../../../../radical-of-a-bilinear-form.md). The $p+m+k$ vectors

$$
e_1+f_1,\ e_1-f_1,\ e_i+f_1\ (i\geq2),\ e_1+f_j\ (j\geq2),\ z_l
$$

are linearly independent and all satisfy $q(v)=0$. They form the required basis of [isotropic vectors](../../../../../isotropic-vector.md).

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
