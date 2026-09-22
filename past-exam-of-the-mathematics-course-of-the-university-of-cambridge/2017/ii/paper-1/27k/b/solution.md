<h1 id="27k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $r_i$ be the [probability](../../../../../../probability.md) of returning to $i$ after its first departure. Transience means $r_i<1$; in particular $q_i>0$. By the [Strong Markov property](../../../../../../strong-markov-property.md), the number $N$ of visits, including the initial visit, has the [geometric distribution](../../../../../../geometric-distribution.md) $\mathbb P(N=n)=(1-r_i)r_i^{n-1}$, $n\ge1$. The [holding times](../../../../../../holding-time.md) of these visits are independent $\operatorname{Exp}(q_i)$ variables and are independent of the jump-chain return decisions.

For the total [occupation time of a continuous-time Markov chain](../../../../../../occupation-time-of-a-continuous-time-markov-chain.md) $T_i$ and $s\ge0$, summing over $N$ gives

$$
\mathbb E_i e^{-sT_i}
=\sum_{n\ge1}(1-r_i)r_i^{n-1}\left(\frac{q_i}{q_i+s}\right)^n
=\frac{q_i(1-r_i)}{s+q_i(1-r_i)}.
$$

Uniqueness of the [Laplace transform](../../../../../../laplace-transform.md) identifies

$$
\boxed{T_i\sim\operatorname{Exp}\bigl(q_i(1-r_i)\bigr)}.
$$

Starting elsewhere adds an atom at zero if the state might never be hit; the purely exponential conclusion uses the specified initial state $i$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
