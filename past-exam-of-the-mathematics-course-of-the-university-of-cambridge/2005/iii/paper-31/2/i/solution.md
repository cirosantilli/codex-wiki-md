<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A useful strong form of the [Hensel lemma](../../../../../../hensel-s-lemma.md) is the following. Let $F$ be a [complete discretely valued field](../../../../../../complete-discretely-valued-field.md), with [valuation ring](../../../../../../valuation-ring.md) $\mathcal O$, normalized [valuation](../../../../../../valuation.md) $v$, and $P\in\mathcal O[T]$. If $a_0\in\mathcal O$ satisfies

$$
v(P(a_0))>2v(P'(a_0)),
$$

then there is a unique root $a\in\mathcal O$ in the ball $v(a-a_0)>v(P'(a_0))$. When $P(a_0)=0$ the assertion is immediate; otherwise the condition includes $P'(a_0)\ne0$.

Here is a proof by [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md). Write $c=v(P'(a_0))$ and $t_0=v(P(a_0))>2c$, and set

$$
a_{j+1}=a_j-\frac{P(a_j)}{P'(a_j)}.
$$

Suppose $v(P'(a_j))=c$ and $t_j=v(P(a_j))>2c$. The correction has [valuation](../../../../../../valuation.md) $t_j-c>c\geq0$, so $a_{j+1}\in\mathcal O$. [Taylor expansion](../../../../../../taylor-expansion.md) over $\mathcal O$ cancels the linear term and gives

$$
v(P(a_{j+1}))\geq2(t_j-c),\qquad
v(P'(a_{j+1})-P'(a_j))\geq t_j-c>c.
$$

Thus the derivative still has [valuation](../../../../../../valuation.md) $c$, and $t_{j+1}-2c\geq2(t_j-2c)$. Unless an exact root is reached earlier, the corrections tend to zero with exponentially increasing [valuations](../../../../../../valuation.md). [Completeness](../../../../../../completeness.md) gives $a_j\to a$, and [continuity](../../../../../../continuous-function.md) gives $P(a)=0$ and $v(a-a_0)=t_0-c>c$. For uniqueness, if $a,b$ are in this ball, [polynomial](../../../../../../polynomial-split.md) expansion around $a_0$ gives

$$
P(a)-P(b)=(a-b)\bigl(P'(a_0)+R\bigr),\qquad v(R)>c.
$$

The second factor has [valuation](../../../../../../valuation.md) exactly $c$ and is nonzero, so two roots in the ball must be equal. In particular, a simple residue root lifts uniquely: $v(P(a_0))\geq1$ and $v(P'(a_0))=0$ satisfy the hypothesis.

For the [square-class group of a p-adic field](../../../../../../square-class-group-of-a-p-adic-field.md), write every element as $p^r u$ with $u\in\mathbb Z_p^\times$. Multiplication by a square changes $r$ by an even [integer](../../../../../../integer.md), so [valuation](../../../../../../valuation.md) parity gives one independent factor $C_2$.

For odd $p$, a unit $u$ is a square if and only if its residue is a square in $\mathbb F_p^\times$. Necessity follows by reduction; sufficiency applies the simple-root [Hensel lemma](../../../../../../hensel-s-lemma.md) to $T^2-u$, whose derivative is a unit at a nonzero residue root. The [cyclic group](../../../../../../cyclic-group.md) $\mathbb F_p^\times$ has square [subgroup](../../../../../../subgroup.md) of index two. If $u_0$ is a unit with nonsquare residue, then

$$
\boxed{\mathbb Q_p^\times/(\mathbb Q_p^\times)^2\cong C_2^2,qquad\text{representatives }1,u_0,p,pu_0\quad(p\ne2).}
$$

For $p=2$, every odd square is one modulo eight. Conversely, if $u\equiv1\pmod8$, take $P(T)=T^2-u$ and $a_0=1$. Then $v_2(P(1))\geq3>2v_2(P'(1))=2$, so the strong [Hensel lemma](../../../../../../hensel-s-lemma.md) gives a [square root](../../../../../../square-root.md). Thus unit [square classes](../../../../../../square-class.md) are exactly their residues $1,3,5,7$ modulo eight. The classes $-1$ and $5$ generate this [group](../../../../../../group-split.md) of order four independently, and [valuation](../../../../../../valuation.md) parity supplies the class $2$. Hence

$$
\boxed{\mathbb Q_2^\times/(\mathbb Q_2^\times)^2\cong C_2^3,qquad\text{generators }-1,5,2,\quad\text{representatives }\pm1,\pm5,\pm2,\pm10.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
