<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Disintegrate $Q$ successively as

$$
Q(dy)=Q_1(dy_1)Q_2(dy_2\mid y_1)\cdots Q_N(dy_N\mid y_{<N}).
$$

For each history $y_{<i}$, choose an optimal coupling of $P_i$ and $Q_i(\cdot\mid y_{<i})$. Sampling these couplings recursively produces a joint law of $(X,Y)$ with $Y\sim Q$. Its conditional $X_i$-marginal is always $P_i$ and is independent of the past, so $X\sim P_1\otimes\cdots\otimes P_N=P$. It is therefore a coupling $\pi\in\Pi(P,Q)$.

Write $c_i(y_{<i})$ for the conditional expected cost $w(X_i,Y_i)$ in the chosen coordinate coupling. The assumed one-coordinate [transport-entropy inequality](../../../../../transport-entropy-inequality.md) gives

$$
\phi(c_i(y_{<i}))
\leq D\bigl(Q_i(\cdot\mid y_{<i})\Vert P_i\bigr).
$$

By [Jensen inequality](../../../../../jensen-s-inequality.md) and the [chain rule for relative entropy](../../../../../chain-rule-for-relative-entropy.md),

$$
\sum_{i=1}^N\phi\bigl(\mathbb E_\pi w(X_i,Y_i)\bigr)
\leq\sum_{i=1}^N\mathbb E_Q\phi(c_i(Y_{<i}))
\leq\sum_{i=1}^N\mathbb E_QD(Q_i(\cdot\mid Y_{<i})\Vert P_i)
=D(Q\Vert P).
$$

Taking the infimum over all couplings proves the [tensorization of a transport-entropy inequality](../../../../../tensorization-of-a-transport-entropy-inequality.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 208](../../paper-208-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
