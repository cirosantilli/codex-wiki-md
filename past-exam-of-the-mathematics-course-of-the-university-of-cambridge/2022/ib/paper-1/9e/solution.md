<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

A [Euclidean domain](../../../../../euclidean-domain.md) is an integral domain $R$ equipped with a function $\delta:R\setminus\{0\}\to\mathbb N$ such that for $a,b\in R$, $b\ne0$, there are $q,r\in R$ with

$$
a=bq+r,\qquad r=0\ \text{or}\ \delta(r)<\delta(b).
$$

For the [Gaussian integers](../../../../../gaussian-integer.md) $\mathbb Z[i]$, take $\delta(z)=N(z)=|z|^2$. Choosing a Gaussian integer nearest to $a/b$ makes the remainder norm smaller than $N(b)$.

The units are precisely the elements of norm one:

$$
\boxed{\{\pm1,\pm i\}}.
$$

Unique factorization in this Euclidean domain gives

$$
\boxed{
2=-i(1+i)^2,\qquad
5=(2+i)(2-i),\qquad
1+3i=(1+i)(2+i)}.
$$

The displayed factors have prime norms $2$ or $5$, so they are irreducible; factors appearing together are nonassociate.

Now suppose $x^2+4=y^3$. Necessarily $y>0$. First let $y$ be odd. Then $x$ is odd, and $x+2i$ and $x-2i$ are coprime in $\mathbb Z[i]$: a common Gaussian prime would divide $4i$, while their product has odd norm. Hence

$$
x+2i=(a+bi)^3
$$

up to a unit, which can be absorbed into the cube. Comparing imaginary parts gives

$$
b(3a^2-b^2)=2.
$$

Checking $b\mid2$ yields only $b=-2$, $a=\pm1$, and therefore

$$
(x,y)=(\pm11,5).
$$

If $y$ is even, congruence modulo $8$ gives $x=2X$ with $X$ odd and $y=2Y$, where

$$
X^2+1=2Y^3.
$$

Each of $X\pm i$ contains exactly one factor $1+i$, so the coprime quotients are cubes up to units. Thus

$$
X+i=u(1+i)(a+bi)^3.
$$

Comparing the imaginary part after the four possible units reduces to

$$
|(a-b)(a^2+4ab+b^2)|=1
\quad\text{or}\quad
|(a+b)(a^2-4ab+b^2)|=1.
$$

Each integer factor must have absolute value one. Substitution then gives $a^2+b^2=1$, so $Y=1$ and $X=\pm1$. Hence

$$
(x,y)=(\pm2,2).
$$

All four pairs satisfy the equation, so the complete answer is

$$
\boxed{(x,y)=(\pm2,2),\ (\pm11,5)}.
$$

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
