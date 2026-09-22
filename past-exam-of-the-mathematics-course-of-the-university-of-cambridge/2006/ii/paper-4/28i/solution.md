<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

A [martingale](../../../../../martingale-split.md) is an adapted [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) process with $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$. A [stopping time](../../../../../stopping-time.md) $T$ has $\{T\le n\}\in\mathcal F_n$ for every $n$. A precise bounded-time [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) says: if $S\le T\le N$ are [stopping times](../../../../../stopping-time.md), then $\mathbb E[M_T\mid\mathcal F_S]=M_S$. To prove it, write

$$
M_T-M_S=\sum_{k=0}^{N-1}(M_{k+1}-M_k)\mathbf1_{\{S\le k<T\}}.
$$

For $A\in\mathcal F_S$, the event $A\cap\{S\le k<T\}$ lies in $\mathcal F_k$. Every summand multiplied by its indicator therefore has expectation zero. Summing proves the conditional expectation identity. All terms are [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) since there are finitely many. Unbounded stopping requires an additional hypothesis such as [uniform integrability](../../../../../uniform-integrability.md) of the stopped [martingale](../../../../../martingale-split.md); it is not justified solely by almost-sure finiteness.

The [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) ensures a finite almost-sure limit if $\sup_n\mathbb E|M_n|<\infty$. [Uniform integrability](../../../../../uniform-integrability.md) also gives convergence in $L^1$. In particular bounded or nonnegative [martingales](../../../../../martingale-split.md) satisfy the almost-sure convergence criterion. A symmetric random walk is a [martingale](../../../../../martingale-split.md) but cannot have a finite limit, since each increment is $\pm1$ and does not tend to zero. Some hypothesis is therefore necessary.

If there are $j$ pessimists, the count increases with probability $(K-j)j/[K(K-1)]$ and decreases with the identical probability. The remaining outcomes leave it unchanged, so $P_n=j_n/K$ is a bounded [martingale](../../../../../martingale-split.md). It converges almost surely. From any nonunanimous state, there is a fixed positive probability, bounded uniformly over the finitely many states, of reaching unanimity within $K-1$ steps by letting each other individual copy a chosen seed. Repeating blocks shows eventual absorption has probability one. Thus the [finite voter-model consensus probability](../../../../../finite-voter-model-consensus-probability.md) is

$$
\boxed{P_\infty\in\{0,1\},\qquad \mathbb P(P_\infty=1)=P_0}.
$$

The last equality follows from bounded convergence and the constant [martingale](../../../../../martingale-split.md) expectation. The population eventually becomes wholly pessimistic or wholly optimistic, with probabilities equal to their respective initial proportions.

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
