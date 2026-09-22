<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $P(z)=\sum_{n\ge0}p_nz^n$, $F(z)=\sum_{j\ge1}f_jz^j$, and $G(z)=\sum_{k\ge0}g_kz^k$ be the count, claim-size and aggregate [probability generating functions](../../../../../probability-generating-function.md). Independence in the [aggregate claims model](../../../../../aggregate-claims-model.md) gives

$$
G(z)=\mathbb E\bigl(F(z)^N\bigr)=P(F(z)).
$$

The [Panjer claim-count class](../../../../../panjer-claim-count-class.md) recurrence can be written $np_n=(an+b)p_{n-1}$. Multiply by $z^{n-1}$ and sum to obtain

$$
P'(z)=a\bigl(zP'(z)+P(z)\bigr)+bP(z),
\qquad (1-az)P'(z)=(a+b)P(z).
$$

Using the [chain rule](../../../../../chain-rule.md) in $G=P\circ F$ then yields

$$
(1-aF(z))G'(z)=(a+b)F'(z)G(z).
$$

The coefficient of $z^{k-1}$ on the left is $kg_k-a\sum_{j=1}^k f_j(k-j)g_{k-j}$, where the $j=k$ term is zero. On the right it is $(a+b)\sum_{j=1}^k jf_jg_{k-j}$. Rearranging gives the [Panjer recursion](../../../../../panjer-recursion.md)

$$
\boxed{g_0=p_0,\qquad
 g_k=\sum_{j=1}^k\left(a+\frac{bj}{k}\right)f_jg_{k-j},\quad k\ge1.}
$$

The initial value is $p_0$ because all claim sizes are positive: zero total loss occurs exactly when $N=0$. Only already computed aggregate probabilities occur on the right. The count normalization determines $p_0$ from $a,b$ as well: with $w_0=1$ and $w_n=\prod_{j=1}^n(a+b/j)$, we have $p_n=p_0w_n$ and $p_0=(\sum_{n\ge0}w_n)^{-1}$. The assumed valid count law makes this sum finite.

Finally $p_0$ must be positive. If it were zero, the recurrence would make every $p_n$ zero, contradicting normalization. At $n=1$ the recurrence therefore gives

$$
\boxed{a+b=\frac{p_1}{p_0}\ge0.}
$$

This proves the sign constraint without assuming any particular count family. The three parts below also provide explicit initial probabilities for the aggregate recursion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
