<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

All the following [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md) and sums lie in the [field with two elements](../../../../../field-with-two-elements.md), so $a+a=0$. For the constant [polynomial](../../../../../polynomial-split.md),

$$
a=(x+1)\cdot0+a.
$$

For the linear [polynomial](../../../../../polynomial-split.md), subtracting the leading multiple means adding it:

$$
ax+b=(x+1)a+(a+b).
$$

For the quadratic [polynomial](../../../../../polynomial-split.md), first cancel $ax^2$ using $ax(x+1)$, leaving $(a+b)x+c$; then cancel $(a+b)x$ using $(a+b)(x+1)$. Thus

$$
ax^2+bx+c=(x+1)\bigl(ax+a+b\bigr)+(a+b+c).
$$

The requested [polynomial quotients](../../../../../quotient-of-polynomial-division.md) and [polynomial remainders](../../../../../remainder-of-polynomial-division.md) are therefore

$$
\boxed{\begin{aligned}
a &: &&Q=0, &&R=a,\\
ax+b &: &&Q=a, &&R=a+b,\\
ax^2+bx+c &: &&Q=ax+a+b, &&R=a+b+c.
\end{aligned}}
$$

For a general [polynomial](../../../../../polynomial-split.md) $P(x)=\sum_{i=0}^{n}p_i x^i$, write $P=(x+1)Q+R$ with constant $R$. Since $1+1=0$, [polynomial evaluation](../../../../../polynomial-evaluation.md) at $x=1$ gives $P(1)=R$. This is the [polynomial remainder theorem](../../../../../polynomial-remainder-theorem.md) with $-1=1$ in the [field with two elements](../../../../../field-with-two-elements.md). Hence

$$
\boxed{P(x)\bmod(x+1)=P(1)=p_0+p_1+\cdots+p_n.}
$$

The [polynomial remainder](../../../../../remainder-of-polynomial-division.md) is precisely the [parity bit](../../../../../parity-bit.md) obtained by taking the [exclusive or](../../../../../exclusive-or.md) of all the [polynomial coefficients](../../../../../coefficient-of-a-polynomial.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
