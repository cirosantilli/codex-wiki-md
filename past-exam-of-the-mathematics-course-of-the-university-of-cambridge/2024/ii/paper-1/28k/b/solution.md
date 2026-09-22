<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The Markov property at deterministic times gives

$$
\mathbb P(Z_{n+1}=j\mid Z_0,\ldots,Z_n=i)
=\mathbb P_i(X_h=j).
$$

Thus $(Z_n)$ is a discrete-time Markov chain with transition [matrix](../../../../../../matrix.md)

$$
P(h)=(p_{ij}(h))_{i,j\in I};
$$

when the minimal chain is nonexplosive, $P(h)=e^{hQ}$.

For an irreducible chain, state $i$ is recurrent in continuous time exactly when

$$
\int_0^\infty p_{ii}(t)\,dt=\infty,
$$

and it is recurrent for the skeleton exactly when $\sum_{n\geq0}p_{ii}(nh)=\infty$. If $t\in[nh,(n+1)h]$, the event of staying at $i$ supplies

$$
e^{-q_i h}p_{ii}(nh)\leq p_{ii}(t)
\leq e^{q_i h}p_{ii}((n+1)h).
$$

Integrating over each interval shows that the [integral](../../../../../../integral.md) diverges exactly when the [series](../../../../../../series-mathematics.md) does. Irreducibility then makes recurrence equivalent for the two chains. This is [recurrence equivalence for a CTMC and its fixed-time skeleton](../../../../../../recurrence-equivalence-for-a-ctmc-and-its-fixed-time-skeleton.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
