<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the intended [random walk](../../../../../../random-walk.md) model, take $S_0$ to be deterministic, or [independent](../../../../../../independent-random-variables.md) of all the [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) $Y_j=S_j-S_{j-1}$. If $\nu$ is their common [probability distribution](../../../../../../probability-distribution.md), then $Y_{t+1}$ is [independent](../../../../../../independent-random-variables.md) of $\mathcal F_t=\sigma(S_0,Y_1,\ldots,Y_t)$. This supplies the [Markov property](../../../../../../markov-property.md) that the backward [dynamic programming](../../../../../../dynamic-programming.md) argument needs. Define the [transition operator](../../../../../../transition-operator.md)

$$
(Ph)(s)=\int_{\mathbb R}h(s+y)\,\nu(dy)
$$

and the deterministic [optimal stopping value function](../../../../../../optimal-stopping-value-function.md) recursively by

$$
V(T,s)=f(s),\qquad V(t,s)=\max\{f(s),(PV(t+1,\cdot))(s)\}.
$$

At any state where the conditional law is evaluated, [independence](../../../../../../independent-random-variables.md) gives

$$
\mathbb E[V(t+1,S_{t+1})\mid\mathcal F_t]=(PV(t+1,\cdot))(S_t).
$$

Backward induction, starting with $U_T=f(S_T)$, proves **the intended representation**

$$
\boxed{U_t=V(t,S_t).}
$$

Integrability along the actual [random walk](../../../../../../random-walk.md) makes the recursion finite at the states used by that process, up to null sets. If finite real-valued [value functions](../../../../../../value-function.md) on all of $\mathbb R$ are intended, a convenient sufficient convention is statewise integrability: $\mathbb E|f(s+Y_1+\cdots+Y_k)|<\infty$ for every $s$ and $0\leq k\leq T$. Indeed each stopping value is bounded in absolute value by the [expectation](../../../../../../expected-value.md) of the sum of the absolute rewards. This convention makes the displayed recursion finite and measurable everywhere; the source only assumes integrability from the given starting process.

The printed independence of the increments alone does not suffice if $S_0$ can reveal future increments. Here is a bounded finite-state counterexample, also with a [convex](../../../../../../convex-function.md) reward. Let $T=2$, let $\varepsilon_1,\varepsilon_2$ be [independent](../../../../../../independent-random-variables.md) fair signs, and set

$$
S_0=\varepsilon_2,\qquad S_1=\varepsilon_1+\varepsilon_2,
\qquad S_2=\varepsilon_1+2\varepsilon_2,\qquad f(s)=s^+.
$$

The two increments are exactly $\varepsilon_1,\varepsilon_2$, hence [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md). But $\mathcal F_1$ already knows both signs, so $U_1=\max\{S_1^+,S_2^+\}$. On the two positive-probability histories with $S_1=0$, its values are respectively $0$ and $1$. Thus no deterministic $V(1,0)$ can work. Adding independence of $S_0$ from the increments repairs this missing [Markov property](../../../../../../markov-property.md) hypothesis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
