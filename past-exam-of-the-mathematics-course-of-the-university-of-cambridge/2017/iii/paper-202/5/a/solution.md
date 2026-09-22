<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [locally defined stochastic process](../../../../../../locally-defined-stochastic-process.md) is a pair $(X,T)$, where $T$ is a lifetime [stopping time](../../../../../../stopping-time.md) and $X_t(\omega)$ is defined for $0\leq t<T(\omega)$, that is, on a [stochastic interval](../../../../../../stochastic-interval.md). For continuous local problems one uses [stopping times](../../../../../../stopping-time.md) $T_n\uparrow T$ with $T_n<T$ on $\{T>0\}$, so the process stopped at each $T_n$ has an ordinary continuous [adapted process](../../../../../../adapted-process.md) version. This is an [announcing sequence for a stopping time](../../../../../../announcing-sequence-for-a-stopping-time.md); no value at $T$ or after $T$ is implicit in the pair.

A [local solution of a stochastic differential equation](../../../../../../local-solution-of-a-stochastic-differential-equation.md) on an open domain $U$ takes its values in $U$ before $T$ and, on every such stopped interval, satisfies

$$
X_{t\wedge T_n}=X_0+\int_0^{t\wedge T_n}b(X_s)\,ds+\int_0^{t\wedge T_n}\sigma(X_s)\,dB_s,
$$

with the local integrability needed for the ordinary and [Itô integrals](../../../../../../ito-integral.md). A [maximal local solution of a stochastic differential equation](../../../../../../maximal-local-solution-of-a-stochastic-differential-equation.md) has no extension to a strictly later lifetime that agrees with it before $T$. For locally [Lipschitz continuous](../../../../../../lipschitz-continuity.md) coefficients on $U$, take a nested [compact exhaustion](../../../../../../compact-exhaustion.md) $K_n$ of $U$ and the successive exit times: their increasing limit is the maximal lifetime, and on $\{T<\infty\}$ the solution eventually leaves every compact subset of $U$. To obtain the announcing sequence with finite stops even when the path never exits a compact set, cap these exit times by $n$; the capped times still increase to the maximal lifetime. Thus **a finite maximal lifetime means exit from the domain or explosion; it need not mean divergence to infinity**. For $U=(0,\infty)$, reaching the boundary zero terminates the local solution even if an absorbing extension could be defined for a different domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
