<h1 id="20d/solution">Solution</h1>

↑ **Parent:** [20D](../20d.md)

The transition row sums to one, since $p\sum_{k=0}^iq^k+q^{i+1}=1$. From any state the [Markov chain](../../../../../markov-chain.md) can reach zero, and from zero consecutive upward moves reach every state; hence it is irreducible. Its self-transition at zero has [probability](../../../../../probability.md) $q>0$, so it is [aperiodic](../../../../../aperiodic-markov-chain.md). It is the [reflected chain with geometric downward jumps](../../../../../reflected-chain-with-geometric-downward-jumps.md).

Put $h_0=1$ for the hitting problem. The first-step equations for $i\geq1$ are

$$
\boxed{h_i=q^{i+1}+p\sum_{j=1}^{i+1}q^{i-j+1}h_j.}
$$

Subtracting $q$ times the equation at $i-1$ gives the [linear recurrence relation](../../../../../linear-recurrence-relation.md), valid for $i\geq2$,

$$
\boxed{ph_{i+1}-h_i+qh_{i-1}=0.}
$$

The separate boundary equation at $i=1$ is $h_1=q^2+pqh_1+ph_2$. It must not be replaced by the [linear recurrence relation](../../../../../linear-recurrence-relation.md) with $h_0=1$: the absorbing hitting convention at zero is different from applying a first-step return equation there.

For $p\ne q$, the [linear recurrence relation](../../../../../linear-recurrence-relation.md) has roots $1$ and $r=q/p$, so $h_i=A+Br^i$ for $i\geq1$. The boundary equation gives $B=r(1-A)$. If $p<1/2$, then $r>1$ and boundedness of probabilities forces $B=0$, hence $A=1$. If $p=1/2$, the repeated-root solution is $A+Bi$; boundedness again gives $B=0$ and the boundary equation gives $A=1$.

For $p>1/2$, $r<1$ and the nonnegative harmonic candidate $\widetilde h_i=r^{i+1}$, together with $\widetilde h_0=1$, satisfies every first-step equation. Hitting-by-time-$n$ probabilities start from zero off the target and iterate those equations, so by induction they are bounded above by this candidate. Taking their increasing limit gives $h_i\leq r^{i+1}$. But the general bounded solution has limit $A\geq0$ as $i\to\infty$, forcing $A=0$ under that bound. Thus

$$
\boxed{h_i=\begin{cases}1,&p\leq1/2,\\(q/p)^{i+1},&p>1/2,\end{cases}\qquad i\geq1.}
$$

In particular the transient exponent is $i+1$, fixed by the original boundary equation.

The [probability](../../../../../probability.md) of a subsequent return to zero when starting there is $f_{00}=q+ph_1$. It is one for $p\leq1/2$, so the [Markov chain](../../../../../markov-chain.md) is recurrent there. For $p>1/2$ it equals $q+p(q/p)^2=q/p<1$, so the [irreducible Markov chain](../../../../../irreducible-markov-chain.md) is transient.

For a stationary [probability](../../../../../probability.md) [vector](../../../../../vector.md) $\pi$, balance at zero and one gives $\pi_1=(p/q)\pi_0$. Subtracting adjacent balance equations gives

$$
q\pi_{j+1}-\pi_j+p\pi_{j-1}=0\qquad(j\geq1),
$$

so this initial ratio propagates and $\pi_j=\pi_0(p/q)^j$. It can be normalized only when $p<q$. In that case

$$
\boxed{\pi_j=\left(1-\frac pq\right)\left(\frac pq\right)^j,\qquad j=0,1,2,\ldots.}
$$

Direct substitution verifies all balance equations, including $\pi_0=q\sum_i\pi_iq^i$. An [irreducible Markov chain](../../../../../irreducible-markov-chain.md) admitting this stationary [probability](../../../../../probability.md) law is [positive recurrent](../../../../../positive-recurrent-markov-chain.md), with mean return time $1/\pi_0=q/(q-p)$. At $p=q$ the [linear recurrence relation](../../../../../linear-recurrence-relation.md) and boundary relation force every $\pi_j$ equal; no such nonzero sequence is summable. The recurrent chain is therefore [null recurrent](../../../../../null-recurrent-state.md). In summary,

$$
\boxed{p<1/2:\ \text{positive recurrent};\qquad p=1/2:\ \text{null recurrent};\qquad p>1/2:\ \text{transient}.}
$$

## ↑ Ancestors (10)

1. [20D](../20d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
