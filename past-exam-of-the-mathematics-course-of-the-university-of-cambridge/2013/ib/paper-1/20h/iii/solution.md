<h1 id="20h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The chain is a [reversible Markov chain](../../../../../../reversible-markov-chain.md), so detailed balance makes the stationary path probability

$$
\pi_{i_0}P_{i_0i_1}\cdots P_{i_{m-1}i_m}
=\pi_{i_m}P_{i_mi_{m-1}}\cdots P_{i_1i_0}.
$$

A path contains an ordered occurrence of $a$ followed later by $b$ exactly when its reversal contains $b$ followed later by $a$. These occurrences need not be adjacent. Therefore $\Pr(\tau(a,b)\le m)=\Pr(\tau(b,a)\le m)$ for every $m$, and in particular the two finite expectations are equal. This is [ordered-state visit times in a reversible chain](../../../../../../ordered-state-visit-times-in-a-reversible-chain.md).

To decompose the expectations, distinguish the entrance time $h(i,j)$, which allows time zero and has $h(j,j)=0$, from the positive return convention $k(j,j)$ in part (i). The [Strong Markov property](../../../../../../strong-markov-property.md) at the first visit to $a$ or $b$ gives

$$
E\tau(a,b)=\sum_i\pi_i h(i,a)+k(a,b),\qquad
E\tau(b,a)=\sum_i\pi_i h(i,b)+k(b,a).
$$

Equating them yields the difference formula with $h$. Replacing $h$ by $k$ in the sum adds $\pi_a k(a,a)-\pi_b k(b,b)=1-1=0$, again by [Kac's lemma](../../../../../../kac-s-lemma.md). Hence

$$
\boxed{k(b,a)-k(a,b)=\sum_i\pi_i[k(i,a)-k(i,b)].}
$$

For a numerical consistency check, the other entrance times are $k(b,a)=15/11$ and $k(c,a)=16/11$, while $k(b,b)=3$. Both sides of the displayed identity equal $-6/11$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
