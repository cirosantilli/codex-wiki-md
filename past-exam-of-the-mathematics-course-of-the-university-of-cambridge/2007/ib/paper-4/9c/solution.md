<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Communication is reflexive because $(P^0)_{ii}=1$, and symmetric by its definition. If $i\leftrightarrow j$ and $j\leftrightarrow k$, choose positive-probability paths $i\to j$ in $m$ steps and $j\to k$ in $n$ steps. The [Chapman-Kolmogorov equation](../../../../../chapman-kolmogorov-equation.md) gives

$$
(P^{m+n})_{ik}\ge(P^m)_{ij}(P^n)_{jk}>0.
$$

Combining the reverse paths gives a positive-probability path $k\to i$ as well. Thus communication is transitive and is an [equivalence relation](../../../../../equivalence-relation.md).

To transfer recurrence, first establish the [recurrence criterion by return probabilities](../../../../../recurrence-criterion-by-return-probabilities.md). Put $r_i=\mathbb P_i(T_i^+<\infty)$ and let $N_i=\sum_{n\ge0}\mathbf1_{\{X_n=i\}}$ under $\mathbb P_i$. After each return the [Strong Markov property](../../../../../strong-markov-property.md) restarts the chain at $i$, so $\mathbb P_i(N_i\ge k+1)=r_i^k$. Therefore

$$
\sum_{n\ge0}(P^n)_{ii}=\mathbb E_iN_i=\sum_{k\ge0}r_i^k.
$$

For $r_i<1$ this equals $(1-r_i)^{-1}$; for $r_i=1$ it is infinite. The [expectation](../../../../../expected-value.md) identity follows by summing the nonnegative indicators, so remains valid when the [expectation](../../../../../expected-value.md) is infinite. Consequently $i$ is a [recurrent state](../../../../../recurrent-state.md) exactly when its return-probability series diverges.

If $i\leftrightarrow j$, choose $a,b$ with $(P^a)_{ji}>0$ and $(P^b)_{ij}>0$. For every $n\ge0$,

$$
(P^{a+n+b})_{jj}\ge(P^a)_{ji}(P^n)_{ii}(P^b)_{ij}.
$$

Summing over $n$, recurrence of $i$ forces the return-probability series for $j$ to diverge. The proved criterion shows **$j$ is recurrent, so recurrence is a property of the [communicating class](../../../../../communicating-class.md)**.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
