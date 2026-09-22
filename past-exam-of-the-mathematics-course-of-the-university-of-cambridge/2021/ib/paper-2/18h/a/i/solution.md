<h1 id="18h/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A distribution $\pi$ is an [invariant distribution](../../../../../../../stationary-distribution.md) when

$$
\pi_j=\sum_{i\in I}\pi_i p_{ij}
$$

for every state $j$. The pair $(\pi,P)$ satisfies [detailed balance](../../../../../../../detailed-balance.md) when

$$
\pi_i p_{ij}=\pi_jp_{ji}
$$

for every $i,j$. Summing this identity over $i$ gives

$$
\sum_i\pi_i p_{ij}
=\sum_i\pi_jp_{ji}
=\pi_j\sum_i p_{ji}
=\pi_j,
$$

so detailed balance implies invariance.

For an irreducible positive recurrent [Markov chain](../../../../../../../markov-chain.md), [Kac's lemma](../../../../../../../kac-s-lemma.md) relates the invariant mass to the [mean recurrence time](../../../../../../../mean-recurrence-time.md):

$$
\boxed{\mathbb E_iT_i^+=\frac1{\pi_i}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [18H](../../../18h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
