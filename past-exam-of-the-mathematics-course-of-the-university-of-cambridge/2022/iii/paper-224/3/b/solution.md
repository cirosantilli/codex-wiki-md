<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [type class](../../../../../../type-class.md) is

$$
T(P)=\{x_1^n:\widehat P_{x_1^n}=P\}.
$$

We first prove a multinomial-mode lemma. If $K=(K_a)_{a\in A}$ has the multinomial law with parameters $n$ and an $n$-type $P$, then $K=nP$ is a mode. Indeed, if $k_a<nP(a)$ and $k_b>nP(b)$, moving one count from $b$ to $a$ changes the probability by the factor

$$
\frac{P(a)}{P(b)}\frac{k_b}{k_a+1}\geq1.
$$

Repeated transfers reach $nP$ without decreasing probability. There are at most $(n+1)^m$ count vectors, so the modal vector has probability at least $(n+1)^{-m}$.

Every string in $T(P)$ has $P^{\otimes n}$-probability

$$
\prod_aP(a)^{nP(a)}=2^{-nH(P)}.
$$

The lemma therefore gives

$$
(n+1)^{-m}
\leq P^{\otimes n}(T(P))
=|T(P)|2^{-nH(P)},
$$

and hence

$$
\boxed{|T(P)|\geq(n+1)^{-m}2^{nH(P)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
