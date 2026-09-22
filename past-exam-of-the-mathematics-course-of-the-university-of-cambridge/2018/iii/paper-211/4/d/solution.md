<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $p_K=C(T,K+1)-2C(T,K)+C(T,K-1)>0$ and $D_K=C(T+1,K)-C(T,K)$. Given $S_T=K$, the next value is one of $K-1,K,K+1$. The [martingale](../../../../../../martingale-split.md) property makes its upward and downward conditional probabilities equal; their sum is the conditional [variance](../../../../../../variance-split.md) of the increment, $\sigma^2(T,K)=2D_K/p_K$. Thus

$$
\boxed{\mathbb P(S_{T+1}=H\mid S_T=K)=\begin{cases}D_K/p_K,&H=K-1\text{ or }K+1,\\1-2D_K/p_K,&H=K,\\0,&\text{otherwise}.\end{cases}}
$$

The [discrete Dupire equation](../../../../../../discrete-dupire-equation.md) therefore recovers all positive-probability one-step conditional transitions from the [European call option](../../../../../../european-call-option.md) price surface. No [Markov property](../../../../../../markov-property.md) is required: these are conditional probabilities given the current value, not necessarily given the whole past.

**Recovery is impossible at a zero-probability state.** For example, $S_t\equiv S_0$ satisfies every stated assumption, but at $T\geq1$ a different integer $K$ can satisfy $|K-S_0|\leq T$ while $p_K=0$. Its conditional transitions can be specified arbitrarily without altering $C$. Thus the literal all-states claim needs the positive-probability qualification.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
