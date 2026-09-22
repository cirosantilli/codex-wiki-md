<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Let $T_0=0$ and let $T_{r+1}$ be the first visit to $i$ strictly after $T_r$, with $T_{r+1}=\infty$ if there is none. Put $q=\mathbb P_i(T_1<\infty)$. The [Strong Markov property](../../../../../strong-markov-property.md) at each finite [first return time](../../../../../first-return-time.md) gives, by induction,

$$
\mathbb P_i(T_r<\infty)=q^r.
$$

The number of visits, including time zero, is $N=\sum_{r\geq0}\mathbf1_{\{T_r<\infty\}}=\sum_{n\geq0}\mathbf1_{\{X_n=i\}}$. By [Tonelli theorem](../../../../../tonelli-theorem.md) for nonnegative terms,

$$
\sum_{n=0}^{\infty}\mathbb P_i(X_n=i)=\mathbb E_iN
=\sum_{r=0}^{\infty}q^r.
$$

If $q<1$, this [geometric series](../../../../../geometric-series.md) is $1/(1-q)$, and $1-q$ is the probability of never returning. If $q=1$, every term of the final series is one and both sides are infinite. Thus

$$
\boxed{\sum_{n=0}^{\infty}\mathbb P_i(X_n=i)=
\frac1{\mathbb P_i(X_n\ne i\text{ for all }n\geq1)},}
$$

with the prescribed infinite-value convention. This covers both [transient states](../../../../../transient-state.md) and [recurrent states](../../../../../recurrent-state.md).

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
