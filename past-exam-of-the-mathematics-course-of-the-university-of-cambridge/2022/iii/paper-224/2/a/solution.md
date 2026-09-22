<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an independent identically distributed source with mass function $P$ on a finite alphabet and a fixed compression rate $R>H(P)$, the optimal probability of decoding error has exponent

$$
E(R)=\min_{Q:H(Q)\geq R}D(Q\Vert P),
$$

meaning that the best fixed-rate codes satisfy

$$
\lim_{n\to\infty}-\frac1n\log_2P_e^{(n)}=E(R)
$$

at continuity points of the exponent.

For the direct part, let $m=|A|$ and

$$
\eta_n=\frac{m\log_2(n+1)}n.
$$

Encode every sequence whose [type](../../../../../../type-information-theory.md) $Q$ satisfies $H(Q)\leq R-\eta_n$. The [method of types](../../../../../../method-of-types.md) bounds the number of such sequences by

$$
(n+1)^m2^{n(R-\eta_n)}=2^{nR},
$$

so they fit into a rate-$R$ codebook. The error probability obeys

$$
\begin{aligned}
P_e^{(n)}
&\leq\sum_{Q:H(Q)>R-\eta_n}P^{\otimes n}(T(Q))\\
&\leq(n+1)^m
2^{-n\min_{Q:H(Q)>R-\eta_n}D(Q\Vert P)}.
\end{aligned}
$$

Compactness of the probability simplex and continuity of entropy and relative entropy on the support of $P$ give

$$
\liminf_{n\to\infty}-\frac1n\log_2P_e^{(n)}
\geq\min_{Q:H(Q)\geq R}D(Q\Vert P)=E(R),
$$

which is the direct bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
