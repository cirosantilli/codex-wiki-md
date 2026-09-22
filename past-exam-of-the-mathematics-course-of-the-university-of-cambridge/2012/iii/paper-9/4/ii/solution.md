<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\mu=1+\varepsilon$, $p=\mu/n$, $q=1-p$, and let $T$ be the [total progeny](../../../../../../total-progeny-of-a-branching-process.md) of a [binomial branching process](../../../../../../binomial-branching-process.md). The preceding [binomial branching survival correction](../../../../../../binomial-branching-survival-correction.md) gives $\rho=(2+o(1))\varepsilon$. For a [branching process conditioned on extinction](../../../../../../branching-process-conditioned-on-extinction.md), the offspring [probability generating function](../../../../../../probability-generating-function.md) is $f((1-\rho)s)/(1-\rho)$, with mean

$$
f'(1-\rho)=(1+\varepsilon)(1-p\rho)^{n-1}
=1-\varepsilon+O(\varepsilon^2+\varepsilon/n)\leq1-\varepsilon/2
$$

for sufficiently large $n$. Summing expected generation sizes therefore gives $\mathbb E[T;T<\infty]=(1-\rho)/(1-f'(1-\rho))=O(1/\varepsilon)$.

Put $K=\lceil\varepsilon^{-3}\rceil$ and let $N_{\geq K}$ count [vertices](../../../../../../vertex-graph-theory.md) in [graph components](../../../../../../component-graph-theory.md) of order at least $K$. A [breadth-first exploration of a binomial random graph](../../../../../../breadth-first-exploration-of-a-binomial-random-graph.md) is dominated by $T$. The [Markov inequality](../../../../../../markov-inequality.md) applied to finite [total progeny](../../../../../../total-progeny-of-a-branching-process.md) gives

$$
\mathbb EN_{\geq K}\leq n\mathbb P(T\geq K)
\leq n\rho+O\left(\frac n{\varepsilon K}\right).
$$

Always $L_1\leq K+N_{\geq K}$. Since $n\varepsilon^4\geq n^{1/3}\to\infty$, we have $K=o(\varepsilon n)$ and $n/(\varepsilon K)=O(n\varepsilon^2)=o(\varepsilon n)$. Hence $\mathbb EL_1\leq(2+o(1))\varepsilon n$. This bound controls the [expected value](../../../../../../expected-value.md) directly, including rare large [graph components](../../../../../../component-graph-theory.md).

For the lower bound, use the [breadth-first exploration of a binomial random graph](../../../../../../breadth-first-exploration-of-a-binomial-random-graph.md) with $U_t$ unseen [vertices](../../../../../../vertex-graph-theory.md), $A_t$ active [vertices](../../../../../../vertex-graph-theory.md) and $t$ explored [vertices](../../../../../../vertex-graph-theory.md), starting from $U_0=n$, $A_0=0$. Let $b_t=\mathbf1_{\{A_{t-1}=0\}}$ indicate a new root. Conditional on the past, the newly discovered count $Z_t$ has a [binomial distribution](../../../../../../binomial-distribution.md) $\operatorname{Bin}(U_{t-1}-b_t,p)$. Put $D_t=Z_t-p(U_{t-1}-b_t)$. The unseen-count recursion gives

$$
A_t=F(t)+\sum_{j=1}^tq^{t-j+1}b_j+q^t M_t,
\quad F(t)=n-t-nq^t,\quad M_t=\sum_{j=1}^tq^{-j}D_j.
$$

Here $M_t$ is a [martingale](../../../../../../martingale-split.md). Up to $T_0=\lceil3\varepsilon n\rceil$, [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md) gives $\mathbb EM_{T_0}^2\leq C\varepsilon n$, since each conditional [variance](../../../../../../variance-split.md) is at most $np<2$ and $q^{-2T_0}$ is bounded.

Take $h=\sqrt\varepsilon+(n\varepsilon^3)^{-1/8}$. Then $h\to0$, $\varepsilon=o(h)$ and $h^2 n\varepsilon^3\to\infty$. The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) implies

$$
\mathbb P\left(\max_{t\leq T_0}|M_t|>h\varepsilon^2n/6\right)
\leq\frac{C}{h^2n\varepsilon^3}=o(1).
$$

The [Taylor expansion](../../../../../../taylor-expansion.md), uniformly for $t\leq T_0$, gives $F(t)=\varepsilon t-t^2/(2n)+O(\varepsilon^3n+\varepsilon)$. Thus $F(t)\geq h\varepsilon^2n/3$ throughout the integer interval $[\lceil h\varepsilon n\rceil,\lfloor(2-h)\varepsilon n\rfloor]$ for large $n$. The new-root sum is nonnegative, so on the preceding event $A_t>0$ throughout this interval. No [graph component](../../../../../../component-graph-theory.md) finishes there: all these explored [vertices](../../../../../../vertex-graph-theory.md) belong to one [graph component](../../../../../../component-graph-theory.md), of order at least $(2-2h)\varepsilon n-O(1)$, [with high probability](../../../../../../with-high-probability.md). Its [expected value](../../../../../../expected-value.md) is therefore at least $(2-o(1))\varepsilon n$. Combining both inequalities proves

$$
\boxed{\mathbb EL_1(G(n,p))=(2+o(1))\varepsilon n.}
$$

The [barely-supercritical largest-component expectation](../../../../../../barely-supercritical-largest-component-expectation.md) uses both a positive exploration window and a finite-progeny bound; a bare convergence-in-probability assertion would not by itself justify this expectation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
