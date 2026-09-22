<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

An integral positive definite [binary quadratic form](../../../../../binary-quadratic-form.md)

$$
[a,b,c](x,y)=ax^2+bxy+cy^2
$$

is [reduced](../../../../../reduced-positive-definite-binary-quadratic-form.md) when

$$
|b|\le a\le c,
$$

with $b\ge0$ when $|b|=a$ or $a=c$. Its [discriminant](../../../../../discriminant-of-a-binary-quadratic-form.md) is $D=b^2-4ac$.

For $D=-20$, reduction gives $3a^2\le20$, so $a=1$ or $2$. Since $b^2\equiv D\pmod4$, $b$ is even. If $a=1$, then $|b|\le1$ forces $b=0$, and $c=5$. If $a=2$, then $b\in\{-2,0,2\}$; integrality of

$$
c=\frac{b^2+20}{8}
$$

leaves $b=\pm2$ and $c=3$, and the boundary convention retains only $b=2$. Hence the complete list is

$$
\boxed{[1,0,5]\quad\text{and}\quad[2,2,3]}.
$$

Now suppose the prime $p\ne5$ is represented by $x^2+5y^2$. If $p=2$, the equation is impossible modulo four, so $p$ is odd. The integers $x$ and $y$ then have opposite parity, and therefore

$$
p=x^2+5y^2\equiv1\pmod4.
$$

Also $x\not\equiv0\pmod5$, since otherwise $5\mid p$; hence

$$
p\equiv x^2\equiv1\ \text{or}\ 4\pmod5.
$$

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives the stronger conclusion

$$
p\equiv1\ \text{or}\ 9\pmod{20}.
$$

In particular,

$$
\boxed{p\equiv1,3,7,\text{ or }9\pmod{20}},
$$

as required.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
