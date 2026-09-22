<h1 id="26i/solution">Solution</h1>

↑ **Parent:** [26I](../26i.md)

A [renewal process](../../../../../renewal-process.md) counts arrivals $N(t)=\max\{j:A_j\leq t\}$, where $A_0=0,A_j=S_1+\cdots+S_j$ and the holding times are [independent](../../../../../independent-random-variables.md), identically distributed positive random variables. Their sum tends to infinity almost surely, so the count is finite on bounded time intervals. Use $N(s)=X_s$ in the question's notation. The index $J=N(s)+1=\min\{j:A_j>s\}$ is a stopping index for the holding-time sequence. Conditional on $J=j$ and the first $j$ holding times, every later $S_{j+k}$ retains its original [probability distribution](../../../../../probability-distribution.md). Summing over $j$ proves

$$
\boxed{P(T_n>t)=P(S_1>t)\quad(n\geq2).}
$$

The straddling time $T_1=S_J$ is different. Let $\overline F(t)=P(S_1>t)$ and let $U$ be the [renewal measure](../../../../../renewal-measure.md) $U(B)=\sum_{j\geq0}P(A_j\in B)$. [Independence](../../../../../independent-random-variables.md) of the next [holding time](../../../../../holding-time.md) from its start gives

$$
P(T_1>t)=\int_{[0,s]}\overline F(\max(t,s-u))\,U(du),
\qquad1=\int_{[0,s]}\overline F(s-u)\,U(du).
$$

For two numbers in $[0,1]$, their minimum is at least their product. Since $\overline F(\max(t,a))=\min(\overline F(t),\overline F(a))$, subtracting $\overline F(t)$ times the second integral proves

$$
\boxed{P(T_1>t)\geq P(S_1>t).}
$$

These formulae handle holding-time atoms with the stated renewal convention $A_j\leq s<A_{j+1}$; sums may be interchanged by nonnegativity.

For rate-$\lambda$ exponentials, the [renewal process](../../../../../renewal-process.md) is Poisson. The elapsed age $B_s=s-A_{N(s)}$ has [probability distribution](../../../../../probability-distribution.md) $\min(E,s)$ with $E\sim\operatorname{Exp}(\lambda)$: for $0\leq b<s$, $P(B_s>b)$ is the [probability](../../../../../probability.md) of no arrivals in $(s-b,s]$, namely $e^{-\lambda b}$, with an atom $e^{-\lambda s}$ at $s$. The forward residual $R_s$ is an [independent](../../../../../independent-random-variables.md) rate-$\lambda$ exponential by [independent](../../../../../independent-random-variables.md) future increments. Thus $T_1=B_s+R_s$. Conditioning on the age gives the exact survival law

$$
\boxed{P(T_1>t)=e^{-\lambda t}\big[1+\lambda\min(s,t)\big],\qquad t\geq0.}
$$

For $s,t>0$ the extra term is strictly positive, proving strict inequality. For fixed $t$ and $s\to\infty$, the limit is $e^{-\lambda t}(1+\lambda t)$, which equals the survival [probability](../../../../../probability.md) of the sum of two [independent](../../../../../independent-random-variables.md) rate-$\lambda$ exponentials. This is the finite-time form of the [stochastic length bias of a renewal interval](../../../../../stochastic-length-bias-of-a-renewal-interval.md).

## ↑ Ancestors (10)

1. [26I](../26i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
