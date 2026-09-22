<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S_k=\sum_{\ell=1}^kY_\ell$, $S_0=0$, be the epochs of the [renewal process](../../../../../../renewal-process.md). The definition uses the next epoch at or after $n$, so $X_n=0$ at an epoch. If $X_n=i\ge1$, no renewal occurs before $n+i$ and necessarily $X_{n+1}=i-1$.

If $X_n=0$, time $n$ is a renewal epoch, and the next unused interarrival time is independent of the entire observed past with the original distribution. To justify the random index, condition on each possible number $k$ of renewals up to $n$: the event identifying $k$ depends only on $Y_1,\ldots,Y_k$, whereas $Y_{k+1}$ is independent of those variables. Summing over $k$ preserves that distribution and independence. Therefore the [residual lifetime Markov chain](../../../../../../residual-lifetime-markov-chain.md) has [transition probabilities](../../../../../../transition-probability.md)

$$
\boxed{P(i,j)=\begin{cases}1,&i\ge1,\ j=i-1,\\ \mathbb P(Y_1=j+1),&i=0,\ j\ge0,\\0,&\text{otherwise}.\end{cases}}
$$

Its reachable state space is $E=\{j\ge0:\mathbb P(Y_1>j)>0\}$, either an initial finite segment or all nonnegative integers. The conditional next-step law depends only on $X_n$, proving the [Markov property](../../../../../../markov-property.md). Initially $X_0=0$. The reset is $Y-1$, rather than $Y$, because one unit of time has elapsed by the next step.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
