<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Consider the graph

$$
\Gamma=\{(x,f(x)):1\leq x\leq N\}\subseteq\mathbb Z^2.
$$

The hypothesis says exactly that $\Gamma$ has at least $\delta N^3$ [additive quadruples](../../../../../../additive-quadruple.md). By the [Balog-Szemerédi-Gowers theorem](../../../../../../balog-szemeredi-gowers-theorem.md), it contains $\Gamma'$ with $|\Gamma'|\gg_\delta N$ and $|\Gamma'+\Gamma'|\ll_\delta|\Gamma'|$.

Part b gives a [Freiman s-isomorphism](../../../../../../freiman-s-isomorphism.md) from $\Gamma'$ to a set $D\subseteq\mathbb Z$, where it is enough to take any fixed $s\geq2$. The set $D$ has bounded doubling, with a bound depending only on $\delta$. Part c therefore provides a proper [generalized arithmetic progression](../../../../../../generalized-arithmetic-progression.md) $Q$ of rank $O_\delta(1)$ such that

$$
|D\cap Q|\gg_\delta|D|\gg_\delta|Q|.
$$

Write $Q$ as a proper parameter box. Since $|Q|\gg_\delta N$, one of its $O_\delta(1)$ side lengths tends to infinity with $N$. Averaging over all lines parallel to that side gives a line on which $D\cap Q$ has density bounded below in terms of $\delta$. The [Szemerédi theorem](../../../../../../szemeredi-s-theorem.md) quoted in the question then gives, once $N$ is sufficiently large in terms of $k$ and $\delta$, a nonconstant $k$-term [arithmetic progression](../../../../../../arithmetic-progression.md) in $D$.

The inverse Freiman isomorphism sends it to a $k$-term arithmetic progression in $\Gamma'\subseteq\Gamma$, because each relation between three consecutive terms is an additive-quadruple relation. Write this progression as

$$
(x_0,y_0),\ (x_0+d,y_0+e),\ldots,
(x_0+(k-1)d,y_0+(k-1)e).
$$

Its first-coordinate difference cannot be zero: the graph of a function has only one point above each $x$. Hence $d\ne0$. On the nonconstant progression

$$
P=\{x_0,x_0+d,\ldots,x_0+(k-1)d\}\subseteq\{1,\ldots,N\},
$$

we have

$$
f(x)=\frac edx+\left(y_0-\frac edx_0\right).
$$

Taking $a=e/d$ and $b=y_0-(e/d)x_0$, both in $\mathbb Q$, proves the claim.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
