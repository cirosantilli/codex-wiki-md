<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [ring](../../../../../ring.md) is [Artinian](../../../../../artinian-ring.md) when its [ideals](../../../../../ideal.md) satisfy the [descending chain condition](../../../../../descending-chain-condition.md): every chain $I_1\supseteq I_2\supseteq\cdots$ eventually becomes constant. It is [Noetherian](../../../../../noetherian-ring.md) when its [ideals](../../../../../ideal.md) satisfy the [ascending chain condition](../../../../../ascending-chain-condition.md), equivalently when every [ideal](../../../../../ideal.md) is finitely generated. We first prove [finite length of a commutative Artinian ring](../../../../../finite-length-of-a-commutative-artinian-ring.md); this gives the stronger structural reason for its [Noetherian](../../../../../noetherian-ring.md) property.

If $\mathfrak p$ is a [prime ideal](../../../../../prime-ideal.md) of an [Artinian ring](../../../../../artinian-ring.md), the quotient $R/\mathfrak p$ is an [Artinian](../../../../../artinian-ring.md) [integral domain](../../../../../integral-domain.md). For a nonzero element $x$ of that domain, the chain $(x)\supseteq(x^2)\supseteq\cdots$ stabilizes. Thus $x^n=bx^{n+1}$ for some $b$, and cancellation gives $bx=1$. The quotient is a [field](../../../../../field.md), so every [prime ideal](../../../../../prime-ideal.md) is a [maximal ideal](../../../../../maximal-ideal.md).

There are only finitely many [maximal ideals](../../../../../maximal-ideal.md). Otherwise, choose distinct ones $\mathfrak m_1,\mathfrak m_2,\ldots$. The intersections $\mathfrak m_1\cap\cdots\cap\mathfrak m_n$ form a strictly descending chain. To see strictness, for each $i\leq n$ choose $a_i\in\mathfrak m_i\setminus\mathfrak m_{n+1}$; their product belongs to the first $n$ [ideals](../../../../../ideal.md) but not to the next one, since $\mathfrak m_{n+1}$ is prime. This contradicts the [descending chain condition](../../../../../descending-chain-condition.md).

Put $J=\bigcap_i\mathfrak m_i$. This [Jacobson radical](../../../../../jacobson-radical.md) is also the [nilradical](../../../../../nilradical.md), since all primes are maximal. We need the stronger conclusion that **$J$ is nilpotent**, without assuming [Noetherianity](../../../../../noetherian-ring.md). Its powers stabilize, say $K=J^n=J^{n+1}=JK$. Suppose $K\neq0$. By the [descending chain condition](../../../../../descending-chain-condition.md), choose an [ideal](../../../../../ideal.md) $L$ minimal subject to $KL\neq0$. Some $x\in L$ has $Kx\neq0$, so minimality gives $L=Rx$. Moreover $K(JL)=KL\neq0$, and minimality gives $JL=L$. Hence $x=jx$ for some $j\in J$. But $1-j$ is a unit: it cannot lie in any [maximal ideal](../../../../../maximal-ideal.md), because $j$ lies in all of them. Thus $x=0$, a contradiction. Therefore $J^n=0$.

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives $R/J\cong\prod_iR/\mathfrak m_i$, a finite product of [fields](../../../../../field.md). Each quotient $J^i/J^{i+1}$ is an [Artinian module](../../../../../artinian-module.md) over this product, and each [field](../../../../../field.md) component must be a finite-dimensional [vector space](../../../../../vector-space-split.md); an infinite-dimensional [vector space](../../../../../vector-space-split.md) admits a strictly descending chain of subspaces. Consequently every layer has finite [composition length](../../../../../composition-length.md). The finite filtration

$$
R\supset J\supset\cdots\supset J^n=0
$$

shows that $R$ itself has finite [composition length](../../../../../composition-length.md). A strict inclusion of submodules strictly increases length, so an ascending chain cannot continue indefinitely. **Every commutative [Artinian ring](../../../../../artinian-ring.md) is therefore [Noetherian](../../../../../noetherian-ring.md).** This is the [Artinian rings are Noetherian](../../../../../artinian-commutative-ring-is-noetherian-theorem.md) result.

For the [formal power series ring](../../../../../formal-power-series.md), let $B=R[[X]]$ with $R$ [Noetherian](../../../../../noetherian-ring.md), and let $H$ be any [ideal](../../../../../ideal.md) of $B$. For $n\geq0$ define a coefficient [ideal](../../../../../ideal.md)

$$
A_n=\{a\in R:\text{some }f\in H\cap X^nB\text{ has coefficient }a\text{ at }X^n\}.
$$

These [coefficient ideals of a formal power series ideal](../../../../../coefficient-ideals-of-a-formal-power-series-ideal.md) satisfy $A_n\subseteq A_{n+1}$, by multiplication by $X$. The [ascending chain condition](../../../../../ascending-chain-condition.md) gives $A_n=A_N$ for all $n\geq N$. For each $0\leq n\leq N$, choose finitely many series $f_{n,j}\in H\cap X^nB$ whose coefficients at $X^n$ generate $A_n$.

We claim that these finitely many series generate $H$ as an ordinary [ideal](../../../../../ideal.md). Given $f\in H$, cancel its coefficient at $X^k$ successively. After coefficients below $k$ have vanished, its coefficient at $X^k$ lies in $A_k$. If $k\leq N$, use an $R$-linear combination of the $f_{k,j}$. If $k>N$, use a combination of $X^{k-N}f_{N,j}$, since $A_k=A_N$. The remainder then belongs to $H\cap X^{k+1}B$.

Collect all the cancellations against each fixed generator. For $n<N$ its multiplier is a polynomial, while the multipliers of the $f_{N,j}$ are well-defined [formal power series](../../../../../formal-power-series.md): at any fixed degree, only finitely many cancellation steps contribute. The remainder has every coefficient zero. Thus

$$
f=\sum_{n=0}^{N}\sum_j g_{n,j}(X)f_{n,j},\qquad g_{n,j}(X)\in R[[X]].
$$

This is a finite sum of [ideal](../../../../../ideal.md) generators, rather than merely a topological closure assertion. Since $H$ was arbitrary,

$$
\boxed{R\text{ Noetherian}\ \Longrightarrow\ R[[X]]\text{ Noetherian}.}
$$

This coefficient-cancellation argument proves [Noetherianity of a formal power series ring](../../../../../noetherianity-of-a-formal-power-series-ring.md).

The corresponding [Artinian](../../../../../artinian-ring.md) assertion is **false**. For any nonzero [ring](../../../../../ring.md) $R$, the [ideals](../../../../../ideal.md)

$$
(X)\supsetneq(X^2)\supsetneq(X^3)\supsetneq\cdots
$$

in $R[[X]]$ are strictly decreasing, since $X^n$ has a nonzero coefficient in degree $n$ and no multiple of $X^{n+1}$ does. In particular, a [field](../../../../../field.md) $k$ is [Artinian](../../../../../artinian-ring.md), but $k[[X]]$ is not. The zero [ring](../../../../../ring.md) is the harmless exception.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
