<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the coefficient form of the [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md): if a polynomial of degree $\sum_i t_i$ has nonzero coefficient at $\prod_i x_i^{t_i}$, then it cannot vanish on every product set $\prod_iS_i$ with $|S_i|>t_i$.

Write the terms as $(a_i,b_i)$ and, over $\mathbb F_p$, put

$$
A=\sum_i a_ix_i,
\qquad B=\sum_i b_ix_i,
\qquad S=\sum_i x_i,
$$

and

$$
E_p(x)=\sum_{|J|=p}\prod_{j\in J}x_j.
$$

Consider

$$
F(x)=
(1-A^{p-1})(1-B^{p-1})
\left[(1-S^{p-1})(2-E_p(x))
-2\prod_i(1-x_i)\right].
$$

A direct multinomial-coefficient calculation, using [Wilson's theorem](../../../../../../wilson-s-theorem.md), shows that the coefficient of $\prod_{i=1}^{4p-2}x_i$ in $F$ is nonzero. The Combinatorial Nullstellensatz with every $S_i=\{0,1\}$ therefore gives an indicator vector $x$ for which $F(x)\ne0$.

The zero indicator does not work. The first two factors force the selected vectors to have both coordinate sums zero. If the support size is not divisible by $p$, [Fermat's little theorem](../../../../../../fermat-little-theorem.md) makes $1-S^{p-1}=0$, while the final product also vanishes; hence the support has size $p$, $2p$, or $3p$. Size $p$ proves the claim, and size $3p$ reduces to part (a). For size $2p$,

$$
E_p(x)=\binom{2p}{p}\equiv2\pmod p,
$$

so the bracket vanishes, again contradicting $F(x)\ne0$. Only the size-$p$ and reducible size-$3p$ cases remain, and either yields the required zero-sum $p$-subsequence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
