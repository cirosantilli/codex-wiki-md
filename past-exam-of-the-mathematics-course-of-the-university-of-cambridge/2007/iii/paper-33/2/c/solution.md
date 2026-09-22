<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $S=1$, the strict inequality in question already fails at time zero, almost surely, since $X_0=0$. Its [probability](../../../../../../probability.md) is therefore zero, as required. Assume for the rest that $0<S<1$, so $M_0=S<1$.

Before time one the boundary inequality is equivalent to $M_t<1$. The process $M$ increases continuously between arrivals and has only downward jumps. Its first time $T<1$ of reaching level one must consequently be a continuous crossing, except possibly if an arrival occurs at the very same instant. All possible first crossing times belong to the finite deterministic set

$$
\left\{1-S+\sum_{i\in I}\theta_i:I\subseteq\{1,\ldots,n\}\right\}.
$$

A uniform arrival hits none of these times almost surely. Thus **$M_T=M_{T-}=1$ on $\{T<1\}$**. This finite candidate set also proves the stopping-time property directly: determining whether a crossing has occurred by time $t$ only uses the arrival history up to $t$. The boundary set always contains time one because $X_1=S$, so $T\leq1$.

For a deterministic $r<1$, the [martingale](../../../../../../martingale-split.md) is bounded on $[0,r]$ by $S/(1-r)$. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for a bounded [stopping time](../../../../../../stopping-time.md) therefore gives

$$
\mathbb E M_{T\wedge r}=S.
$$

Moreover $0\leq M_{T\wedge r}\leq1$: if $T\leq r$ its value is one, and otherwise no crossing has yet occurred. As $r\uparrow1$, the stopped value tends to one on $\{T<1\}$ and to zero on $\{T=1\}$, because after the last arrival the unstopped process is zero. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) now gives

$$
S=\mathbb P(T<1),\qquad\boxed{\mathbb P(1-S+X_t>t\text{ for every }t<1)=\mathbb P(T=1)=1-S.}
$$

This is the [finite-jump boundary crossing identity](../../../../../../finite-jump-boundary-crossing-identity.md). It uses uniform integrability of the bounded stopped values, not uniform integrability of the original family, which fails.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
